<!-- Generated from tempi-tech/AGICockpit — do not edit directly. -->

# AGI Cockpit

**Run multiple coding agents in parallel. Keep every task, decision, and result in one cockpit.**

AGI Cockpit is a cross-platform parallel coding agent manager for coordinating Claude Code, OpenAI Codex, Cursor, Grok, and other terminal-based agents. It gives each piece of work a persistent task, lets you supervise multiple agents without mixing their context, and keeps human approvals close to the work.

> This repository contains generated public documentation, screenshots, and release notes. The AGI Cockpit application source code is not included.

[Download AGI Cockpit](https://agi-labo.com/en/tools/cockpit) · [Read the official documentation](https://agi-labo.com/en/tools/cockpit/docs) · [View release notes](./RELEASES.md)

![AGI Cockpit showing parallel agent tasks and a task conversation](./assets/cockpit-main-visual.png)

## Why AGI Cockpit

- **Parallel coding agent manager** — Run isolated tasks side by side, see which agents are working or waiting, and return to any result without losing context.
- **Multi-agent by design** — Use Claude Code, OpenAI Codex, Cursor, Grok, Antigravity, or a terminal task from the same interface.
- **Human decisions stay explicit** — Agents can send an Ask when they need a choice or confirmation. Review and answer it from the desktop app or mobile PWA.
- **Mobile PWA supervision** — Check progress, answer Asks, send follow-up instructions, and operate Autoruns from another device.
- **Cross-platform** — Available for Windows, macOS, and Linux.
- **Local working environment** — Agent processes and project files remain on the computer running Cockpit. Each agent or connected service uses its own network and authentication settings.

## One workspace for every agent

AGI Cockpit treats a task as the durable unit of work. A task contains the objective, working directory, selected agent, conversation, approvals, changed files, previews, and result. You can run several tasks at once while keeping their histories and project scope separate.

The desktop app supports Claude Code, OpenAI Codex, Grok Build, Antigravity, Cursor, Cockpit Agent, and ordinary terminal commands. Supported agents can run in a native task UI or a full terminal.

## Supervise from mobile

The mobile PWA connects to the Cockpit running on your computer. It is designed for supervision rather than moving your development environment to a hosted service.

| Task supervision | Human approval |
| --- | --- |
| ![AGI Cockpit mobile task list](./assets/cockpit-mobile-tasks.png) | ![AGI Cockpit mobile Ask](./assets/cockpit-mobile-ask.png) |

PWA remote access and Autorun require an AGI Labo membership. Regular desktop tasks can be started in guest mode.

## Get started

1. [Download AGI Cockpit](https://agi-labo.com/en/tools/cockpit) for Windows, macOS, or Linux.
2. Open the app and select a project workspace or temporary folder.
3. Choose an installed coding agent.
4. Create a task with a clear objective.
5. Review the result, answer any Ask, and send follow-up instructions from the same task.

See [Install and run your first task](https://agi-labo.com/en/tools/cockpit/docs/getting-started) for the complete walkthrough.

## Documentation

| Guide | English | 日本語 |
| --- | --- | --- |
| Product overview | [What is AGI Cockpit?](./docs/en/overview.md) | [AGI Cockpitとは](./docs/ja/overview.md) |
| First task | [Install and run your first task](./docs/en/getting-started.md) | [インストールして最初のタスクを実行する](./docs/ja/getting-started.md) |
| Task management | [Task list and task details](./docs/en/tasks.md) | [タスク一覧とタスク詳細](./docs/ja/tasks.md) |
| Human approval | [Ask](./docs/en/ask.md) | [Ask](./docs/ja/ask.md) |
| Scheduled work | [Autorun](./docs/en/autorun.md) | [オートラン](./docs/ja/autorun.md) |
| Releases | [Release history](./docs/en/releases.md) | [リリース履歴](./docs/ja/releases.md) |

The canonical, web-rendered documentation is available at [agi-labo.com/en/tools/cockpit/docs](https://agi-labo.com/en/tools/cockpit/docs).

## Releases

The generated [release notes](./RELEASES.md) follow the versions distributed for AGI Cockpit. Download links and platform availability are maintained on the [official product page](https://agi-labo.com/en/tools/cockpit).

## Feedback

Use [GitHub Issues](https://github.com/tempi-tech/agi-cockpit/issues) for bug reports and feature requests. Do not open pull requests against generated files: changes must be made in the private canonical repository and will replace this repository on the next sync.

## About this repository

Everything here is generated from the private [`tempi-tech/AGICockpit`](https://github.com/tempi-tech/AGICockpit) repository. Do not edit generated files directly.
