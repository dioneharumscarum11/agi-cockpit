<!-- Generated from tempi-tech/AGICockpit — do not edit directly. -->

# Task list and task details

Understand the task list, Overview, task details, task states, follow-up instructions, quotes, attachments, resume, and completion.

> Verified with AGI Cockpit 4.41.0 on 2026-07-29. [View the official documentation](https://agi-labo.com/en/tools/cockpit/docs/tasks)

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

## Conversation, quotes, and inter-task messages

Selecting text in the chat reveals **Quote selection**. Activating it inserts the selected content into the composer as a Markdown quote. Cockpit preserves the selection while task progress updates.

A message sent by another Cockpit task is labeled **Sent from another task** and shows the source task name or short ID. When the source task still exists in the current list, select its name to navigate to it.

In the PWA, a down-arrow button appears above the composer after you scroll away from the latest message. Select it to jump to the end of the conversation and resume following new output.

## Attach files

In Desktop and the PWA, the new-task screen and task-details composer can attach images, text, source code, JSON, CSV, PDFs, audio, video, and office documents. When the selected agent supports a format natively, Cockpit sends it as a native attachment. Otherwise, Cockpit supplies its local path and metadata for the name, MIME type, and size. Handling varies by agent, UI mode, and model, so not every combination can interpret every format directly.

Attachments have these limits:

- Up to eight files, 512 MB per file, and 1 GB in total
- JSON files are limited to 25 MB each
- Archives and executable formats are not supported
- Cockpit validates the extension, MIME type, actual size, and content, then stores the upload under a randomized name rather than its original file name

An attachment's name and content are not automatically trusted instructions. State which file the agent should use and what result you expect in the message itself.

## History dashboard

The history dashboard in the header is available in guest mode. Alongside Cockpit activity, it can show local external sessions from Claude Code and Codex CLI and import them as tasks. Autorun and PWA remote access still require an AGI Labo membership.

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
