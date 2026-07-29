<!-- Generated from tempi-tech/AGICockpit — do not edit directly. -->

# Autorun

Learn how Autorun starts a new task from a one-time, interval, or cron schedule and keeps the result as a regular Cockpit task.

> Verified with AGI Cockpit 4.41.0 on 2026-07-29. [View the official documentation](https://agi-labo.com/en/tools/cockpit/docs/autorun)

Autorun starts a new task automatically at a specified time, interval, or cron schedule. It does not coordinate several agents inside one run. It is an independent way to start the same kind of work when it is needed.

## Requirements

Autorun requires an AGI Labo membership. Cockpit verifies membership not only at the Desktop entry point, but also in the PWA, `cockpit autorun`, the local API, and each scheduled execution. Requests from guests and inactive members return an explicit error. Cockpit also rejects an operation safely when a network or API failure prevents verification, but it does not cache that failure and block a member after service recovers. Existing members can use the CLI while signed in to AGI Labo in Desktop.

Schedules run inside the AGI Cockpit app process. They do not fire while Cockpit is closed, and the operating-system scheduler does not launch Cockpit for them.

## Schedule types

| Type | Setting | Behavior |
| --- | --- | --- |
| Once (`once`) | Date and time | Starts once, then disables itself |
| Interval (`interval`) | Minutes, hours, or days | Starts after the selected interval from the previous scheduling pass |
| Cron (`cron`) | `minute hour day month weekday` | Starts at the next time that matches the cron expression |

In the cron weekday field, `0` means Sunday. For example, `0 9 * * 1-5` runs at 9:00 a.m. on weekdays.

## Create an Autorun task

1. Open **Autorun Tasks** at the top of Desktop.
2. Select **New Autorun**.
3. Enter a name and the instruction to send when the task starts.
4. Choose the working directory. When running as the Master Agent, Cockpit uses the Master's working location.
5. Select an agent and, when shown, review its UI mode, account, model, reasoning effort, service tier, system prompt, and approval mode.
6. Choose **Once**, **Interval**, or **Cron** and configure the timing.
7. Save the Autorun and confirm that the list shows its next run time.

Autorun keeps the runtime settings from the time it is saved as a snapshot. Changing global settings later does not silently change an existing Autorun's model, reasoning effort, service tier, system prompt, approval mode, account, or UI mode. If a saved model or account becomes unavailable, Cockpit does not substitute another setting. It disables that Autorun and marks it as needing attention.

Desktop and the PWA show only settings supported by the selected agent and UI mode. The CLI and API use the same capability data and reject unsupported combinations with an explicit error before saving.

Cursor Autoruns can use **Native UI** or **Terminal**. Native UI exposes Cursor's available model and approval mode in Desktop, the PWA, and CLI-backed creation. Cursor does not expose reasoning-effort, service-tier, system-prompt, or account-profile settings.

## Review a run

When Autorun fires, it creates a new task in the same form as any regular task. Select it from the task list, then use task details to review its conversation, confirmation requests, errors, and results. The new task keeps a reference to the Autorun ID that created it.

The Autorun manager supports:

- enable and disable
- edit
- delete
- **Run Now**
- previous and next run times

Cockpit does not start another scheduled run while the previous execution turn from the same Autorun is still processing. Visual Runtime, shown as Native UI in the app, releases the lock when the turn completes, the runtime settles it, or a runtime error occurs. Terminal UI and the Terminal agent release it when the launched process exits or is cleaned up. The lock does not wait for a person to mark the Cockpit task **Completed**. Startup failures and cleanup paths also release it, and a 24-hour expiry is the final safeguard against an abandoned lock.

## Working directory and failures

The Desktop form requires a directory unless the Autorun runs as the Master Agent. If the CLI omits the directory, Cockpit creates an `agi-cockpit` directory inside the operating-system temporary folder.

If the agent fails to start, the task remains in the task list with an **Error** state. A one-time Autorun still becomes disabled; an interval or cron Autorun remains enabled and calculates its next run. Open the created task details to inspect the cause.

If Cockpit confirms that the account is a guest or has an inactive membership when a run is due, a one-time Autorun does not start and becomes disabled. An interval or cron Autorun remains enabled and checks again at its next scheduled time. If a temporary network or API failure prevents verification, Cockpit does not start the run and checks again one minute later. It keeps a one-time Autorun enabled and persists the retry time, so a temporary outage does not consume its only run.

## Create from the CLI

```bash
cockpit autorun create \
  --name "Weekday progress review" \
  --instruction "Review the unfinished work in this project and summarize it in priority order." \
  --directory /path/to/project \
  --agent-type codex \
  --ui-mode visual \
  --model gpt-5.4 \
  --effort high \
  --service-tier fast \
  --approval-mode accept-edits \
  --type cron \
  --expression "0 9 * * 1-5"
```

```bash
cockpit autorun list
cockpit autorun get <id>
cockpit autorun run <id>
cockpit autorun toggle <id>
```

## Related pages

- [Task list and task details](https://agi-labo.com/en/tools/cockpit/docs/tasks)
- [Ask](https://agi-labo.com/en/tools/cockpit/docs/ask)
