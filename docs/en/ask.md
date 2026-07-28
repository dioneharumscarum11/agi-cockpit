<!-- Generated from tempi-tech/AGICockpit — do not edit directly. -->

# Ask

Learn how Ask safely hands a confirmation or decision from an AI agent to a person and resumes the same task after the answer.

> Verified with AGI Cockpit 4.40.0 on 2026-07-29. [View the official documentation](https://agi-labo.com/en/tools/cockpit/docs/ask)

Ask lets an AI agent pause its work and hand a confirmation or decision to a person. Cockpit returns the answer to the original task as a structured event, then resumes that same task from where it stopped.

## When to use Ask

- A person must make the final decision before publishing, deleting, purchasing, or taking another consequential action.
- Several approaches have clear trade-offs.
- A person needs to inspect an image, listen to audio, or watch a video before deciding.
- Several related decisions should be reviewed together.

Ask is more than a notification. The question remains available until it is answered, and a person can respond in the dedicated Desktop Ask window or from **Asks** in the PWA.

## How Ask differs from other confirmations

| Mechanism | Purpose | After the response |
| --- | --- | --- |
| Ask | An agent explicitly hands a decision to a person | The answer returns to the original task and resumes it automatically |
| Normal reply | A person sends the next instruction to a task | The task starts a new turn |
| Agent-specific question | The running agent asks for input | The response answers that agent's question |
| Tool approval | Decides whether a file change, command, or other tool action may run | Returns an allow, always allow, or reject decision |
| `cockpit display` | Puts information in front of the person | Does not wait for a response or resume the task |

An Ask answer is not itself permission to operate on the OS or an external service. An action that needs permission can still trigger a separate tool approval after the person confirms the direction through Ask.

## Question and answer formats

Ask can combine:

- single choice
- multiple choice
- free-form input
- several related questions
- an outcome or trade-off description for each choice
- image, audio, or video attached to the question
- images, text, source code, JSON, CSV, PDFs, audio, video, or office documents attached to an answer

Free-form input is available by default even when choices are provided. Write the question so it can stand on its own: identify the subject, the current state, and the result of each choice.

## What happens before and after an answer

1. The agent creates an Ask.
2. Cockpit saves the question and displays it in Desktop or the PWA.
3. A person answers with a choice, text, and optional supported file attachments.
4. Cockpit delivers a `cockpit.ask.resolved` event to the original task.
5. The agent receives the answer and continues the same work.

Dismissing an Ask without answering removes the Ask, but it does not resume the original task automatically. A person can resume the task later with a normal message if needed.

## Constraints

- A task can hold only one active Ask at a time.
- A completed task cannot create an Ask.
- Ask is available to resumable AI-agent tasks, not Terminal tasks.
- After creating an Ask, the agent waits and does not continue work that depends on the answer.
- A question can attach up to eight files, with a limit of 512 MB per file and 1 GB in total.
- Answer attachments have the same eight-file, 512 MB per-file, and 1 GB total limits. A JSON file is limited to 25 MB.
- Archives and executable formats are rejected. Cockpit validates the extension, MIME type, actual size, and content, and stores the upload under a randomized name rather than its original file name.
- Cockpit does not expand attachment contents into the prompt automatically. The agent receives a local path and metadata for the name, MIME type, and size.

## Create an Ask from the CLI

```bash
cockpit ask \
  --summary "The production release is ready. All tests passed and only documentation changed. Publish it?" \
  --choice "Publish" \
  --choice-description "Commit, push, and deploy to production" \
  --choice "Revise" \
  --choice-description "Do not publish and wait for another instruction"
```

When the command succeeds, it returns an Ask ID. The agent ends its turn at that point and does not poll for the answer.

## Operate open Asks from the CLI

Starting with v4.39.0, the CLI can list, answer, or close open Asks in addition to creating them.

```bash
cockpit ask list
cockpit ask list --task <task-id>
cockpit ask answer <ask-id> --choice "Publish"
cockpit ask close <ask-id>
```

`list` inspects the question, choices, and attached-media metadata. `answer` acts on the user's behalf and resumes the task that created the Ask. Use it only when the answering agent has both the context and the authority to relay the decision, such as a voice agent conveying an explicit answer from the user. Do not answer an Ask with media until the user or proxy has actually inspected that media.

`close` removes an unanswered Ask without resuming its originating task. Use it to clear a stale Ask, not to bypass a decision that still needs an answer.

## Related pages

- [Task list and task details](https://agi-labo.com/en/tools/cockpit/docs/tasks)
- [Autorun](https://agi-labo.com/en/tools/cockpit/docs/autorun)
