<!-- Generated from tempi-tech/AGICockpit — do not edit directly. -->

# What is AGI Cockpit?

Learn where AGI Cockpit runs AI agents and how the task list and task details connect human decisions with result review.

> Verified with AGI Cockpit 4.39.0 on 2026-07-28. [View the official documentation](https://agi-labo.com/en/tools/cockpit/docs)

AGI Cockpit is a desktop app for handing work to multiple AI agents and supervising their progress, requests for decisions, and results in one place. Creating a task, reviewing its result, sending follow-up instructions, and completing it all stay within the same unit of work.

## How work moves through Cockpit

1. Give a task an objective and a working directory.
2. Start the selected AI agent.
3. Use the task list to distinguish running, awaiting confirmation, completed, and failed work.
4. Open task details to review the conversation, confirmation requests, diffs, files, pages, and other results.
5. Send another instruction, answer an Ask, resume the task, or complete it.

Cockpit does not move the work itself into the cloud. Agent processes and working files remain on the computer running Cockpit. Network access by an agent or another service follows that product's own configuration.

## Four product surfaces

| Surface | Role | Primary user |
| --- | --- | --- |
| Desktop | Main place to create, list, inspect, configure, and review tasks | People |
| Agent process | Executes instructions and returns conversation or changes to the task | AI agents |
| PWA | Reviews and operates tasks, Asks, and Autoruns from another device | People |
| `cockpit` CLI | Operates tasks, Asks, Autoruns, the browser, and other Cockpit surfaces | AI agents and people |

Remote access through the PWA and Autorun require an AGI Labo membership. You can start regular tasks in guest mode.

## Where to start

- Go from installation to reviewing a result: [Install and run your first task](https://agi-labo.com/en/tools/cockpit/docs/getting-started)
- Keep multiple pieces of work distinct: [Task list and task details](https://agi-labo.com/en/tools/cockpit/docs/tasks)
- Hand a decision from an agent to a person: [Ask](https://agi-labo.com/en/tools/cockpit/docs/ask)
- Start a new task at a set time or interval: [Autorun](https://agi-labo.com/en/tools/cockpit/docs/autorun)

## Guest mode and AGI Labo membership

| Access | Scope covered by these docs |
| --- | --- |
| Guest mode | Create a task in Desktop, run an agent, and review the result |
| AGI Labo member | Everything in guest mode, plus Autorun, PWA remote access, and the history dashboard |

A lock on a feature means that feature requires sign-in. Authentication for Claude Code, Codex, or another task agent is managed separately from your AGI Labo sign-in.

## Next step

[Install AGI Cockpit and run your first task](https://agi-labo.com/en/tools/cockpit/docs/getting-started) to reach the point where the task appears in the list and its result is available in task details.
