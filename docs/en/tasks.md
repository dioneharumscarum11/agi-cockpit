<!-- Generated from tempi-tech/AGICockpit — do not edit directly. -->

# Task list and task details

Understand the task list, Overview, task details, task states, waiting reasons, follow-up instructions, resume, and completion.

> Verified with AGI Cockpit 4.39.0 on 2026-07-28. [View the official documentation](https://agi-labo.com/en/tools/cockpit/docs/tasks)

The task list is where you choose what to look at next. Task details is where you understand and act on the selected work. Overview searches across tasks, projects, and agents.

## Three views

| View | Primary role |
| --- | --- |
| Task list | Keeps active work visible and sorts it by priority, status, creation time, or update time |
| Overview | Searches across tasks, projects, and agents, including completed work |
| Task details | Shows the conversation, progress, confirmation requests, composer, and entry points to results |

The task list can filter by agent and pin a task or project. Switching the selected task does not stop the other agents; each task continues independently.

## Task states

| State | Meaning | What to check next |
| --- | --- | --- |
| Running (`running`) | An agent or command is processing | Read the progress. Interrupt only when the direction must change immediately |
| Awaiting confirmation (`waiting_confirmation`) | A response ended, a question is open, or permission is required | Check the waiting reason, then reply or return the requested decision |
| Completed (`completed`) | A person marked the whole task complete | Confirm that every result you need has been saved |
| Error (`error`) | The agent or command failed to start | Read the error in task details |

**Awaiting confirmation** does not have a single meaning. An AI agent or the `cockpit` CLI should also inspect the waiting reason before acting.

| Waiting reason | Meaning |
| --- | --- |
| `turn_complete` | One response ended and the task can accept the next instruction |
| `permission` | A tool action needs to be allowed or rejected |
| `question` | The running agent needs an answer to its own question |
| `terminal_prompt` | The terminal is waiting for input |
| `runtime_error` | The runtime reported an error |
| `idle_timeout` | Idle detection considers the task ready for input |
| `unknown` | Cockpit cannot identify a safe, specific waiting reason |

`turn_complete` does not mean the whole task is complete. With the CLI, send a normal follow-up only when `readyForNextPrompt` is `true`. Handle a visible permission or question first when the reason is `permission` or `question`.

## Follow up, queue, interrupt, and resume

- **Follow-up instruction**: starts the next turn of a task that is awaiting confirmation.
- **Queue**: holds an instruction sent while a task is running and starts it after the current turn ends.
- **Interrupt current turn**: stops the current processing and switches to the new instruction.
- **Resume**: reconnects an unfinished task whose process stopped, such as after an app restart, to its saved session.

`needsResume` is not a task state. It is additional information indicating that an unfinished task lost its process and requires a resume action.

## Complete and delete

Complete moves a task out of active work and into completed work. Delete removes the task record from Cockpit. They are different operations.

Completing a task in a temporary folder deletes that working directory automatically. Completing a Git-worktree task in Desktop silently preserves the worktree. By contrast, `cockpit task complete <id>` deletes the worktree by default and preserves it only with `--keep-worktree`. Before completing a task from the CLI, confirm where the required changes are stored and which option you need.

## Inspect state from the CLI

```bash
cockpit task list
cockpit task get <id>
```

`task get` returns `status`, `waitingReason`, `readyForNextPrompt`, and `needsResume`, together with the latest conversation and terminal output.

## Related pages

- [Install and run your first task](https://agi-labo.com/en/tools/cockpit/docs/getting-started)
- [Ask](https://agi-labo.com/en/tools/cockpit/docs/ask)
- [Autorun](https://agi-labo.com/en/tools/cockpit/docs/autorun)
