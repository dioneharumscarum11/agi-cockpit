<!-- Generated from tempi-tech/AGICockpit — do not edit directly. -->

# Install and run your first task

Install AGI Cockpit, choose a working directory and agent, review the result of your first task, and mark the task complete.

> Verified with AGI Cockpit 4.40.0 on 2026-07-29. [View the official documentation](https://agi-labo.com/en/tools/cockpit/docs/getting-started)

By the end of this guide, you will be able to open AGI Cockpit, run your first task, review its result, and complete the task.

## 1. Install AGI Cockpit

Open the [AGI Cockpit download page](https://agi-labo.com/en/tools/cockpit) and choose the package for your operating system.

| OS | Package | Architecture |
| --- | --- | --- |
| Windows | Microsoft Store | x64 / arm64 |
| macOS | `.dmg` | Apple Silicon |
| Linux | AppImage / `.deb` | x64 / arm64 |

On Windows, install AGI Cockpit from Microsoft Store. On macOS, open the `.dmg` and move AGI Cockpit to Applications. On Linux, use the distributed AppImage or `.deb` package.

After launch, choose guest mode if you want to continue without an account. Sign in as an AGI Labo member if you need Autorun or remote access from another device.

AGI Cockpit stores credentials and API keys in encrypted operating-system storage such as Keychain or a keyring. If encrypted storage is unavailable, Cockpit does not fall back to plaintext. It rejects the save and shows recovery guidance. Enable the operating-system Keychain or keyring, then sign in again.

Remote access defaults to Tailscale-only mode. When Tailscale HTTPS is enabled but its certificate is unavailable, Cockpit does not silently downgrade to HTTP and does not start the connection. Local Wi-Fi mode is unencrypted, so Cockpit enables it only after an explicit confirmation and keeps a warning visible while it is active. Do not use local Wi-Fi mode on a public network.

## 2. Prepare an agent

The new-task screen can start Claude Code, Codex CLI, Grok Build, Antigravity CLI, Cursor CLI, Cockpit Agent, or Terminal. If Cockpit cannot find an agent, the screen shows **Install** or **Open Settings**.

If the screen shows **Install**, use it to install the corresponding CLI. If it shows **Open Settings**, confirm the launch command in Settings. Return to the new-task screen after installation; the agent is ready when it becomes selectable.

When you use Claude Code, Codex, or Grok Build in Native UI, you can start before authenticating. Task details then shows sign-in guidance, and Cockpit retries the first instruction in the same task after authentication succeeds. This guidance and automatic retry do not apply to Terminal UI or the Terminal agent. In those modes, complete the CLI's sign-in flow inside the terminal, then resume or recreate the task.

An AI agent's subscription and authentication are separate from your AGI Labo sign-in. Signing in as an AGI Labo member does not authenticate Claude Code, Codex, or another task agent.

## 3. Create your first task

1. Open **New task** at the top of the window.
2. Choose **Project workspace** or **Temporary folder**. For an existing project, select only the directory you intend the agent to inspect.
3. Select an AI agent.
4. For supported agents, choose **Native UI** or **Terminal** as the UI mode.
5. For this first check, choose **Supervised** approval mode and enter a short request with a clear completion condition.
6. Create the task.

The settings shown depend on the agent and UI mode. Desktop, PWA, CLI, and Autorun use the same capability data. An unsupported combination of model, reasoning effort, service tier, system prompt, account, or approval mode is hidden or rejected with an explicit error before creation.

A read-only request is a safe first check.

```text
Inspect this folder and describe its main files and their roles in no more than five points. Do not change any files.
```

A temporary folder is deleted automatically when the task is completed. Before starting in an existing project, make sure you understand that the agent can operate on files in that directory.

## 4. Confirm the successful state

The new task appears in the task list and normally starts as **Running**. The task details view shows the instruction you sent and the agent's progress or response.

After one response finishes, the task moves to **Awaiting confirmation**. This does not mean the entire task is complete. It means the task can accept another instruction or decision. If the result is incomplete, send a follow-up instruction from the composer in task details.

When the work is finished, select **Complete** in task details. Completed tasks move out of the active list and do not accept regular follow-up instructions.

## 5. Update AGI Cockpit

Check for a new version from the update notice in the header or **Check for Updates** in Settings. On platforms where Cockpit downloads the update, use the on-screen action to restart and install it when ready. On Linux, the notice opens the download page that matches the current display language.

When Cockpit requires a newer version before continuing, the screen shows release notes and a download destination in the app's current language. Review the Japanese guidance in the Japanese UI or the English guidance in the English UI before updating.

## 6. If the task does not start

| Message or state | What to check |
| --- | --- |
| The agent is not installed | Use **Install**, or select **Open Settings** and check the launch command for that CLI |
| Native UI requires sign-in | Complete the guidance in task details and wait for Cockpit to retry the same instruction |
| Terminal UI or Terminal requires sign-in | Complete that CLI's sign-in flow in the terminal, then resume or recreate the task |
| The task shows **Error** | Read the startup error at the top of task details, then check the directory, command, and authentication |
| The composer says **Resume the task to continue** | Select **Resume** to reconnect to the saved session |
| You need a result from a temporary folder | Save the result to a persistent location before completing the task |

## Create a task from an AI agent

If the `cockpit` command is installed from Cockpit settings, an AI agent can create the same kind of task:

```bash
cockpit task create \
  --instruction "Inspect this folder and describe its structure in no more than five points. Do not change any files." \
  --directory /path/to/project
```

If the command omits the directory, Cockpit starts the task in an operating-system temporary folder.

## Related pages

- [Task list and task details](https://agi-labo.com/en/tools/cockpit/docs/tasks)
- [Ask](https://agi-labo.com/en/tools/cockpit/docs/ask)
- [Autorun](https://agi-labo.com/en/tools/cockpit/docs/autorun)
- [Release history](https://agi-labo.com/en/tools/cockpit/docs/releases)
