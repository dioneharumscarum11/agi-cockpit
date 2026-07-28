<!-- Generated from tempi-tech/AGICockpit — do not edit directly. -->

# AGI Cockpit release notes

English is the primary language for these generated release notes. Download the latest version from the [official AGI Cockpit page](https://agi-labo.com/en/tools/cockpit).

## v4.39.0 — 2026-07-27

**Type:** minor · **Platforms:** macOS, Linux

- Improved child-task listing, creation, and review with a dedicated workspace in the right side panel.
- Added keyboard controls to the in-app browser.
- Added file uploads to the in-app browser.
- Added Cockpit CLI commands to list, answer, and close Asks.
- Fixed file previews interfering with other controls.
- Improved file previews by centering the requested line when opened.
- Improved thinking-level controls by disabling unavailable levels and showing guidance when thinking is off.
- Fixed Claude Visual tasks sometimes failing to start on Windows.
- Fixed Codex Native UI sometimes failing to start on Windows.
- Fixed the production OAuth endpoint being configured incorrectly on Windows.
- Fixed Grok Visual tasks sometimes failing to start when the side panel was closed.
- Fixed running workflows ending when switching to a Grok task.
- Fixed Grok background work appearing to remain active after task completion.

<details>
<summary>日本語のリリースノート</summary>

- 子タスクを右サイドパネルの専用ワークスペースで一覧・作成・確認できるように改善
- アプリ内ブラウザにキーボード操作を追加
- アプリ内ブラウザでファイルをアップロードできるように対応
- Cockpit CLIからAskの一覧確認・回答・終了を行えるように対応
- ファイルプレビューが操作を妨げる問題を修正
- ファイルプレビューで指定行を中央に表示するよう改善
- 思考機能がオフのときに利用できない思考レベルを選択不可にし、案内を表示するよう改善
- WindowsでClaudeのビジュアルタスクが起動しない場合がある問題を修正
- WindowsでCodex Native UIが起動しない場合がある問題を修正
- Windowsで本番環境のOAuth接続先が正しく設定されない問題を修正
- サイドパネルを開いていない状態でGrokのビジュアルタスクが起動しない場合がある問題を修正
- Grokタスクへ切り替えた際に実行中のワークフローが終了する問題を修正
- Grokタスクの完了後もバックグラウンド処理が実行中と表示される問題を修正

</details>

## v4.38.3 — 2026-07-26

**Type:** patch · **Platforms:** macOS, Linux

- Improved Codex usage resets to show each reset window's expiration alongside the number of available resets.
- Fixed subagent output appearing in the parent task conversation during a Grok workflow.
- Improved selection by placing Grok Build near Claude and Codex on the new-task and Settings screens.

<details>
<summary>日本語のリリースノート</summary>

- Codexの使用量リセットについて、利用可能な回数に加えて各リセットの有効期限を確認できるように改善
- Grokワークフロー実行中にサブエージェントの出力が親タスクの会話へ混ざる問題を修正
- 新規タスク作成と設定画面でGrok BuildをClaude・Codexの近くに配置し、選択しやすく改善

</details>

## v4.38.2 — 2026-07-26

**Type:** patch · **Platforms:** macOS, Linux

- Fixed Codex tasks failing to start when the Windows user-folder path contained spaces.
- Added a per-file button for reverting changes from the diff side panel.

<details>
<summary>日本語のリリースノート</summary>

- Windowsでユーザーフォルダのパスに空白が含まれる場合もCodexタスクを正しく起動できるように修正
- 差分サイドパネルからファイル単位で変更を取り消せるボタンを追加

</details>

## v4.38.1 — 2026-07-25

**Type:** patch · **Platforms:** macOS, Linux

- Fixed Grok Visual tasks appearing to remain active after background work completed, and added workflow progress and status details.
- Fixed selection of Codex models that support Fast mode on mobile.
- Fixed the confirmation view losing focus during Japanese text input.
- Fixed text input in the in-app browser and file previews using paths relative to the home directory.
- Improved the task list's child-task layout and the composer's usage and context display.
- Fixed Codex tasks sometimes failing to start on Windows.

<details>
<summary>日本語のリリースノート</summary>

- Grokビジュアルタスクのバックグラウンド処理が完了後も実行中と表示される問題を修正し、ワークフローの進捗と状態を確認できる表示を追加
- モバイル版でCodexのFast対応モデルを正しく選択できるように修正
- 確認画面で日本語入力中にフォーカスが外れる問題を修正
- アプリ内ブラウザの文字入力と、ホームディレクトリ相対パスのファイルプレビューを修正
- タスク一覧の子タスク表示と、入力欄の利用状況・コンテキスト表示のレイアウトを改善
- WindowsでCodexタスクが正しく起動しない場合がある問題を修正

</details>

## v4.38.0 — 2026-07-25

**Type:** minor · **Platforms:** macOS, Linux

- Improved the in-app browser by preserving sessions, tabs, and sign-in state after task completion and app restarts, and by refining page control, waits, full-page screenshots, and Chrome-profile cookie imports.
- Added OAuth sign-in popups to the in-app browser.
- Added automatic Claude Visual model discovery from Claude Code and reflected new models, including Claude Opus 5, in desktop and mobile selectors.
- Fixed the Visual agent model picker failing to open on the new-task screen and fixed usage and mobile composer layouts on narrow screens.
- Changed Claude Code authentication guidance for the current subscription allowances.

<details>
<summary>日本語のリリースノート</summary>

- アプリ内ブラウザのセッション・タブ・ログイン状態をタスク完了後やアプリ再起動後も保持し、表示中ページの操作や待機、全ページ撮影、Chromeプロファイル指定のCookie取り込みを改善
- アプリ内ブラウザでOAuthログインのポップアップを開けるように対応
- Claudeビジュアルタスクで利用可能なモデルをClaude Codeから自動取得し、新しいモデルやClaude Opus 5をデスクトップ・モバイルのモデル選択に反映
- 新規タスク画面でビジュアルエージェントのモデル選択が開かない問題と、狭い画面で利用状況やモバイル入力欄が崩れる問題を修正
- Claude Code認証の案内を現在のサブスクリプション利用枠に合わせて更新

</details>

## v4.37.0 — 2026-07-24

**Type:** minor · **Platforms:** macOS, Linux

- Added Fast mode to Codex tasks and a default speed setting.
- Added imports of site cookies from Chrome on macOS so the in-app browser can reuse sign-in state.
- Added an in-app branch switcher and improved mobile Git-status visibility, including changed-file counts.
- Added task search by task ID.
- Fixed notification task navigation after browser loading and missing in-app browser tabs.

<details>
<summary>日本語のリリースノート</summary>

- CodexタスクでFastモード（速度優先モード）を選択できるようになり、設定でデフォルト速度も指定可能に
- アプリ内ブラウザでmacOSのChromeからサイトのCookieを取り込めるようになり、ログイン状態を引き継いで閲覧できるように対応
- タスクのブランチをアプリ内で切り替えられるブランチスイッチャーを追加し、モバイルでも変更ファイル数などのGit状態を確認しやすく改善
- タスク検索でタスクIDによる検索に対応
- 通知からのタスク移動がブラウザ読み込み後に効かない問題や、アプリ内ブラウザでタブが表示されない問題を修正

</details>

## v4.36.0 — 2026-07-24

**Type:** minor · **Platforms:** macOS, Linux

- Improved the chat composer with AI usage, time-to-reset, manual refresh, and account switching.
- Improved model, thinking level, and skill selection operations on desktop and mobile, making it easier to use even on narrow screens.
- Improved Cockpit Agent history recovery so visible conversations remain intact after a temporary retrieval failure.
- Added OpenCode Go provider support to Cockpit Agent.
- Added Grok tasks to Native UI by default and displayed Grok Build authentication status in Settings.
- Fixed issues with terminal display stopping and Japanese input flickering, moving tasks from notifications, and Git status display on mobile.

<details>
<summary>日本語のリリースノート</summary>

- チャット入力欄にAIの利用状況とリセットまでの時間を表示し、手動更新やアカウント切り替えをすばやく行えるように改善
- デスクトップとモバイルでモデル・思考レベル・スキルの選択操作を統一し、狭い画面でも使いやすく改善
- Cockpit Agentで履歴の取得が一時的に失敗した場合も、表示済みの会話が欠けずに復元されるように改善
- Cockpit AgentでOpenCode Goプロバイダーを利用できるように対応
- Grokタスクを標準でネイティブUIから利用できるようにし、設定画面にGrok Buildの認証状態を表示
- ターミナルの表示停止と日本語入力のちらつき、通知からのタスク移動、モバイルのGit状態表示に関する問題を修正

</details>

## v4.35.2 — 2026-07-23

**Type:** patch · **Platforms:** macOS, Linux

- Improved update checks and downloads so the latest release remains available after an earlier update was downloaded.
- Improved synchronization between update notifications and Settings, and prevented accidental dismissal actions.
- Fixed past conversations failing to reappear after switching Claude accounts.
- Fixed an issue where Codex tasks could keep returning to running after waiting.

<details>
<summary>日本語のリリースノート</summary>

- 新しいアップデートが公開された際、以前の更新をダウンロード済みでも最新バージョンを正しく確認・取得できるように改善
- アップデート通知と設定画面の表示を同期し、通知を誤操作なく閉じられるように改善
- Claudeのアカウント切り替え後も、過去の会話を正しく再表示できるように修正
- Codexタスクが待機後に実行中へ戻り続けることがある問題を修正

</details>

## v4.35.1 — 2026-07-23

**Type:** patch · **Platforms:** macOS, Linux

- Improved the usage screen with Grok Build account, plan, sign-in, and retrieval-error details.
- Improved usage loading so a slow service does not delay results from other services.
- Improved the stability of Claude account display and Grok Build usage and credit retrieval.
- Improved work-status visibility by grouping branch, pull-request, and diff information near the composer.

<details>
<summary>日本語のリリースノート</summary>

- 利用状況画面でGrok Buildのアカウントとプランを確認でき、ログイン状態や取得エラーも分かりやすく表示
- 各サービスの使用量を個別に読み込むことで、一部の取得が遅い場合でも他の使用量をすばやく確認できるように
- Claudeのアカウント表示とGrok Buildの使用量・クレジット取得の安定性を改善
- タスクのブランチ・PR・差分情報を入力欄の近くにまとめ、作業状態を確認しやすく改善

</details>

## v4.35.0 — 2026-07-22

**Type:** minor · **Platforms:** macOS, Linux

- Added multiple Codex accounts with selection during task creation, execution, and Autorun.
- Added per-account Codex usage and Cursor usage to the usage screen, and improved scannability.
- Improved Grok Build tool readability by showing context usage and background work.
- Added PWA messaging to Grok Build and improved copy reliability.
- Improved retention of sign-in state and remote-access settings across updates.
- Improved in-app browser authentication compatibility for more reliable access to sign-in-required sites.
- Improved task and report notification destinations to prevent incorrect navigation and notification loops.
- Improved Antigravity completion detection, Claude background logs, Codex session detection, and notification handling.
- Fixed the working-folder picker disappearing from the new-task screen in the light theme.

<details>
<summary>日本語のリリースノート</summary>

- Codexで複数アカウントを登録し、タスク作成時・実行中・オートランで使い分けられるように
- 利用状況画面でCodexのアカウント別使用量とCursorの使用量を確認でき、一覧性も向上
- Grok Buildのコンテキスト使用量とバックグラウンド処理を表示し、ツール実行の内容を読み取りやすく改善
- PWAからGrok Buildへメッセージを送信できるようにし、コピー操作の安定性も改善
- アップデート後もサインイン状態とリモートアクセス設定を保持するように
- アプリ内ブラウザの認証互換性を改善し、ログインが必要なサイトをより安定して利用できるように
- タスク通知のクリック先とレポート通知を改善し、誤った画面遷移や通知の連鎖を防止
- Antigravityの完了判定、Claudeのバックグラウンドログ表示、Codexのセッション検出と通知処理を改善
- ライトテーマで新規タスク画面の作業フォルダ選択が見えなくなる問題を修正

</details>

## v4.34.0 — 2026-07-21

**Type:** minor · **Platforms:** macOS, Linux

- Added image attachments to confirmation answers and improved large-media transfers in Desktop and the PWA.
- Added PWA control of right-side-panel terminals and automatic resumption of stopped tasks.
- Added OS notifications and Dock or taskbar badges for tasks that need attention.
- Added task-list filtering by agent type.
- Added Codex goal progress to desktop and PWA task headings.
- Added error reasons for process startup failures and fixed terminals failing to start after prolonged macOS use.
- Improved terminal copying with a context menu and failure guidance.
- Improved Claude permission checks and terminal waiting detection to prevent duplicate notifications and status flickering.
- Added working-folder selection from the project name on the new-task screen.
- Changed Linux update notifications to open the download page for reliable installation.
- Fixed bugs related to formula display, external links in display HTML, history loading, Windows file selection, and parent-child task structure.

<details>
<summary>日本語のリリースノート</summary>

- 確認依頼への回答に画像を添付でき、デスクトップとPWAで大容量メディアも安定して送受信できるように
- PWAから右サイドパネルのターミナルを切り替えて操作でき、停止したタスクの自動再開にも対応
- 対応が必要なタスクをOS通知とDock・タスクバーバッジで確認できるように
- タスク一覧をエージェントの種類で絞り込めるように
- Codexのゴール進行状態をデスクトップとPWAのタスク見出しに表示
- プロセスの起動失敗を理由付きのエラーとして表示し、macOSで長時間利用した際にターミナルが起動できなくなる問題を修正
- ターミナルのコピー操作を改善し、右クリックメニューと失敗時の案内を追加
- Claudeの権限確認とターミナルの待機判定を改善し、重複通知や状態のちらつきを防止
- 新規タスク画面のプロジェクト名から作業フォルダを選択できるように
- Linuxでは更新通知からダウンロードページを開く方式に変更し、更新を確実に適用できるように
- 数式表示、表示用HTMLの外部リンク、履歴の読み込み、Windowsのファイル選択、親子タスク構造に関する不具合を修正

</details>

## v4.33.0 — 2026-07-18

**Type:** minor · **Platforms:** macOS, Linux

- Added readable inline and block LaTeX rendering to AI chat.

<details>
<summary>日本語のリリースノート</summary>

- AIチャットでLaTeX形式のインライン数式とブロック数式も読みやすく表示できるように

</details>

## v4.32.1 — 2026-07-18

**Type:** patch · **Platforms:** macOS, Linux

- Added automatic setup of Creative Studio picture-book tools on Windows and Linux.
- Fixed the Cockpit Ask window changing size as its content changed.

<details>
<summary>日本語のリリースノート</summary>

- WindowsとLinuxでもCreative Studioの絵本制作に必要なツールを自動セットアップできるように
- Cockpit Askウィンドウの内容が変わる際にサイズが揺れる問題を修正

</details>

## v4.32.0 — 2026-07-17

**Type:** minor · **Platforms:** macOS, Linux

- Added OpenRouter credit balance and usage for Cockpit models to the usage menu.
- Improved formula rendering in AI chat.
- Added project renaming, folder opening, and name reset actions to the task list.
- Added simultaneous review and answering of multiple Cockpit Asks in separate windows.
- Fixed accidental Ask submission with Enter during Japanese input and delivery of Ask answers to Grok Visual.

<details>
<summary>日本語のリリースノート</summary>

- OpenRouter経由のCockpitモデルのクレジット残高と使用量を使用量メニューで確認できるように
- AIチャットで数式を読みやすく表示できるように
- タスク一覧からプロジェクト名の変更、フォルダを開く操作、名前のリセットができるように
- 複数のCockpit Askをそれぞれ独立したウィンドウで同時に確認・回答できるように
- 日本語入力中のEnterによるAskの誤送信と、Grok VisualへのAsk回答の配信不具合を修正

</details>

## v4.31.0 — 2026-07-17

**Type:** minor · **Platforms:** macOS, Linux

- Added Talk Room for real-time conversations among multiple agents and users.
- Added Talk Room access from the PWA for reviewing and joining conversations away from Desktop.
- Added Ultra reasoning to Codex Visual Sol and Terra models for automatic delegation of complex work to subagents.
- Fixed Grok Visual Cockpit actions targeting the wrong task when several tasks used the same folder.

<details>
<summary>日本語のリリースノート</summary>

- 複数のエージェントとユーザーがリアルタイムに会話できるTalk Roomを追加
- PWAからTalk Roomを開き、外出先でも会話への参加や確認ができるように
- Codex VisualのSol・Terraモデルで、複雑なタスクをサブエージェントへ自動委譲するUltra推論を選べるように
- 同じフォルダで複数タスクを実行しても、Grok VisualからのCockpit操作が正しいタスクに届くように

</details>

## v4.30.0 — 2026-07-16

**Type:** minor · **Platforms:** macOS, Linux

- Added Native UI launch and in-app progress and result review for Grok Build.
- Added Grok Build usage to the usage popover.
- Changed the in-app browser to follow Cockpit appearance settings.
- Improved long-running stability and immediate display of Visual history.
- Added shared agent skills to every agent.

<details>
<summary>日本語のリリースノート</summary>

- Grok BuildをネイティブUIから起動し、生成状況や結果をCockpit内で確認できるように
- Grok Buildの利用状況を使用量ポップオーバーで確認できるように
- アプリ内ブラウザがCockpitの外観モードに追従するように
- Visualの履歴をすぐに表示し、長時間利用時の安定性を改善
- 共有エージェントスキルをすべてのエージェントで利用できるように

</details>

## v4.29.0 — 2026-07-14

**Type:** minor · **Platforms:** macOS, Linux

- Added persistent agent confirmation requests that can be answered after an app restart to resume the task.
- Improved hierarchy and progress visibility by arranging child tasks vertically.
- Added screenshots of off-screen tabs in the in-app browser.
- Fixed Max reasoning-effort selection for supported Codex Visual models.
- Changed the official website messaging and release history to make information easier to find.

<details>
<summary>日本語のリリースノート</summary>

- エージェントからの確認依頼を永続化し、アプリ再起動後も回答してタスクを再開できるように
- 子タスクを縦に並べて、階層と進行状況を確認しやすく
- アプリ内ブラウザで画面外のタブもスクリーンショットを取得できるように
- Codex Visual で対応モデルの Max 推論エフォートを正しく選択できるように
- 公式サイトのメッセージとリリース履歴ページを刷新し、情報を見つけやすく

</details>

## v4.28.0 — 2026-07-13

**Type:** minor · **Platforms:** macOS, Linux

- Added model and reasoning-effort selection to cockpit CLI task creation and exposed both values in task information.
- Added header back and forward buttons for navigating task history.
- Added import of external Claude Code and Codex sessions as Cockpit tasks.
- Added remote Autorun control from the PWA and cockpit CLI.
- Added Claude account profile selection to Autorun.
- Improved PWA task creation and messaging with desktop options including model, effort, approval mode, branch, profile, and skills.
- Added a recent-instructions bar to the PWA with navigation to remote task views.
- Added Fast fallback for GPT-5.6 models in Codex Visual.
- Added Cmd+Backspace line deletion to macOS terminal input.
- Removed unread badges from running tasks.
- Changed Terminal UI and PWA conversations to follow the chat font-size setting.
- Improved Codex usage display and reset handling.
- Changed preview and report links to open in the operating system default browser.
- Improved status display while running /compact or /clear and fixed missing status after switching tasks.
- Added npm installation instructions when installing Codex CLI.
- Fixed Tailscale appearing uninstalled while it was running.
- Fixed global shortcuts failing to persist across restarts and Meta or Windows key recording on Windows and Linux.
- Fixed an issue that could cause a crash when opening a terminal.
- Fixed text overflow in terminal.
- Fixed automatic conversation scrolling interrupting manual scrolling.
- Changed the directory picker to stay in front of the main window.
- Removed background browser windows from Mission Control.

<details>
<summary>日本語のリリースノート</summary>

- cockpit CLI からタスク作成時にモデルと推論エフォートを指定し、タスク情報から確認できるように
- ヘッダーに戻る・進むボタンを追加し、タスク間の移動履歴をたどれるように
- Claude Code / Codex の外部セッションを Cockpit のタスクとして取り込めるように
- オートランを PWA や cockpit CLI からリモート操作できるように
- オートランに Claude アカウントプロファイルを指定できるように
- PWA のタスク作成とメッセージ送信をデスクトップ版と同等機能に拡張（モデル・エフォート・承認モード・ブランチ・プロファイル・スキル等）
- PWA に最新指示バーを追加し、リモートタスク表示へジャンプできるように
- Codex Visual: GPT-5.6 モデルで Fast フォールバックに対応
- macOS のターミナル入力で Cmd+Backspace の行削除に対応
- 実行中タスクでは未読バッジを表示しないように
- チャットのフォントサイズ設定をターミナル UI と PWA の会話表示にも適用
- Codex の使用量表示とリセット処理を改善
- プレビューやレポートのリンクを OS の既定ブラウザで開くように
- /compact・/clear 実行中のステータス表示を改善し、タスク切り替え時の表示漏れを修正
- Codex CLI インストール時に npm での導入案内を追加
- Tailscale が動作しているのに未インストールと誤表示される問題を修正
- グローバルショートカットが再起動後に保持されない問題と Windows/Linux の Meta/Win キー記録を修正
- ターミナルを開いた際にクラッシュすることがある問題を修正
- ターミナルのテキストはみ出しを修正
- 会話表示で手動スクロール中に自動スクロールが割り込む問題を修正
- ディレクトリ選択ダイアログがメインウィンドウの手前に表示されるように
- バックグラウンドのブラウザウィンドウが Mission Control に表示されないように

</details>

## v4.27.0 — 2026-07-10

**Type:** minor · **Platforms:** macOS, Linux

- Added available usage-reset actions to the Codex usage popover.
- Added GPT-5.6 Sol, Terra, and Luna model selection to Codex Visual and improved required CLI-update guidance.

<details>
<summary>日本語のリリースノート</summary>

- Codex の使用量ポップオーバーから、利用可能な使用量リセットを実行できるように
- Codex Visual で GPT-5.6 Sol / Terra / Luna モデルを選択できるようにし、必要な Codex CLI 更新案内を改善

</details>

## v4.26.1 — 2026-07-10

**Type:** patch · **Platforms:** macOS, Linux

- Fixed the agent Settings tab overflowing its container.

<details>
<summary>日本語のリリースノート</summary>

- エージェント設定タブの表示がはみ出す問題を修正

</details>

## v4.26.0 — 2026-07-10

**Type:** minor · **Platforms:** macOS, Linux

- Added Grok Build task creation, startup, trust confirmation, and terminal control.
- Added multiple Claude account profiles with per-task selection and switching.
- Improved per-account Claude status and usage visibility in the header and usage popover.
- Added Claude account listing and per-task account switching to Cockpit CLI.
- Improved in-app browser address selection and Grok Build terminal scrolling.

<details>
<summary>日本語のリリースノート</summary>

- Grok Build エージェントを追加し、タスク作成から起動・信頼確認・ターミナル操作まで扱えるように
- Claude の複数アカウントプロファイルに対応し、タスクごとに使用するアカウントを選択・切り替えられるように
- ヘッダーと使用量ポップオーバーで Claude アカウントごとの状態と使用量を確認しやすく
- cockpit CLI にアカウント一覧とタスクの Claude アカウント切り替えコマンドを追加
- アプリ内ブラウザのアドレス選択と Grok Build ターミナルのスクロール操作を改善

</details>

## v4.25.0 — 2026-07-08

**Type:** minor · **Platforms:** macOS, Linux

- Added skill completion in the chat composer and resolution to the correct skill reference on send.
- Improved in-app browser tab handling with compact display for many tabs and less rendering of hidden tabs.
- Changed environment guidance for agents to stabilize decisions on in-app browser usage and branch creation.

<details>
<summary>日本語のリリースノート</summary>

- チャット入力でスキル候補を補完し、送信時に正しいスキル参照へ解決できるように
- アプリ内ブラウザのタブ操作を改善し、タブが多いときの表示崩れと非表示タブの不要な描画を抑制
- エージェント向けの環境ガイダンスを更新し、アプリ内ブラウザ利用やブランチ作成の判断を安定化

</details>

## v4.24.0 — 2026-07-07

**Type:** minor · **Platforms:** macOS, Linux

- Added system-prompt presets to Native UI tasks with per-agent defaults in Settings.
- Fixed an issue where the cockpit CLI could not be used from agents running in a sandbox.
- Improved Cockpit CLI guidance for agents and organized cockpit help by command.

<details>
<summary>日本語のリリースノート</summary>

- ネイティブUIタスクでシステムプロンプトのプリセットを選択できるように（エージェントごとの既定値は設定から変更可能）
- サンドボックス内で動くエージェントから cockpit CLI が使えないことがある問題を修正
- エージェント向けの cockpit CLI ガイダンスを拡充し、cockpit help をコマンド単位に整理

</details>

## v4.23.0 — 2026-07-05

**Type:** minor · **Platforms:** macOS, Linux

- Added in-app release history.
- Added /compact to the Claude Visual slash menu.
- Added a chat minimap and terminal prompt-history rails for navigating long conversations and output.
- Improved Claude and Codex usage display to match OAuth sign-in information.
- Fixed an issue where completion reports were sometimes not sent for self-resumed tasks.

<details>
<summary>日本語のリリースノート</summary>

- アプリ内からバージョン履歴を確認できるように
- Claude Visual のスラッシュメニューから /compact を実行できるように
- チャットのミニマップとターミナルのプロンプト履歴レールを追加し、長い会話や出力をたどりやすく
- Claude / Codex の使用量表示をOAuthログイン情報に合わせて安定化
- 自己再開したタスクで完了レポートが送られないことがある問題を修正

</details>

## v4.22.3 — 2026-07-03

**Type:** patch · **Platforms:** Linux

- Fixed occasional app freezes when opening external links, including support links.

<details>
<summary>日本語のリリースノート</summary>

- サポートリンクなどの外部リンクを開いた際にアプリが停止することがある問題を修正

</details>

## v4.22.2 — 2026-07-03

**Type:** patch · **Platforms:** Linux

- Fixed the app stopping after interaction when launched in the background from a terminal.
- Improved display in light mode.

<details>
<summary>日本語のリリースノート</summary>

- ターミナルからバックグラウンドで起動した際に、操作するとアプリが停止する問題を修正
- ライトモードの表示を改善

</details>

## v4.22.1 — 2026-07-03

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Fixed an issue where browser login could not be started on Linux.
- Added login URL copy for environments where the browser cannot be opened automatically.
- Fixed per-task model selection overwriting the default model in Settings.

<details>
<summary>日本語のリリースノート</summary>

- Linuxでブラウザログインが開始できない問題を修正
- ブラウザを自動で開けない環境向けにログインURLコピーを追加
- タスクごとのモデル選択が、設定のデフォルトモデルを上書きしてしまう問題を修正

</details>

## v4.22.0 — 2026-07-03

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added Linux support with x64 and arm64 AppImage and .deb packages.

<details>
<summary>日本語のリリースノート</summary>

- Linuxに対応（AppImage / .deb、x64・arm64）

</details>

## v4.21.0 — 2026-07-02

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added cockpit task run and wait for command-driven task creation and completion waiting.
- Improved parent-task delivery of child-task results by persisting task reports.
- Added Native UI and Terminal selection to Creative Studio task creation.
- Improved diagnostics by saving main-process exception logs.
- Improved chat readability in the light theme.

<details>
<summary>日本語のリリースノート</summary>

- cockpit task run / wait を追加し、タスク作成から完了待機までをコマンドで実行できるように
- タスクレポートを永続化し、親タスクから子タスクの結果を安定して受け取れるように
- Creative Studioでも新規タスク作成時にNative UI / Terminalを選べるように
- メインプロセスの例外ログを保存し、問題発生時の原因を追いやすく
- ライトテーマのチャット表示をより見やすく調整

</details>

## v4.20.5 — 2026-07-02

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added Native UI and Terminal selection to new-task creation.
- Fixed Sonnet 5 missing from the Claude Visual model picker.

<details>
<summary>日本語のリリースノート</summary>

- 新規タスク作成時にNative UI / Terminalを選べるように
- Claude Visualのモデル選択でSonnet 5が表示されない問題を修正

</details>

## v4.20.4 — 2026-07-02

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added Fable 5 weekly usage, remaining runs, and reset time.
- Improved Antigravity usage retrieval.

<details>
<summary>日本語のリリースノート</summary>

- Fable 5の週間使用量・残り回数・リセット時刻を確認できるように
- Antigravityの使用量取得を安定化

</details>

## v4.20.3 — 2026-07-01

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added shortcuts for new-task creation and terminal opening and closing.
- Fixed a blank view after reopening the cockpit browser in the right side panel.
- Improved review of long output by retaining more PWA terminal history.

<details>
<summary>日本語のリリースノート</summary>

- 新規タスク作成とターミナル開閉のショートカット設定に対応
- cockpit browser の右サイドパネルを開き直したときの空白表示を修正
- PWAのターミナル履歴表示を増やし、長い出力を確認しやすく

</details>

## v4.20.2 — 2026-06-30

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added character-sheet and confirmation-frequency settings to Creative Studio picture-book generation.
- Improved closing image previews in cockpit ask.

<details>
<summary>日本語のリリースノート</summary>

- Creative Studioの絵本生成でキャラクターシートと確認頻度の設定に対応
- cockpit ask の画像プレビューを閉じる操作を改善

</details>

## v4.20.1 — 2026-06-27

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added bulk expand and collapse actions to the child-task panel.
- Added bulk resumption of child tasks that require resumption.
- Fixed completed Visual Runtime tasks reverting to an earlier state.

<details>
<summary>日本語のリリースノート</summary>

- 子タスクパネルで一括展開・折りたたみ操作を追加
- 子タスクパネルから再開が必要な子タスクをまとめて再開できるように
- Visual Runtimeタスクの完了状態が意図せず復帰する問題を修正

</details>

## v4.20.0 — 2026-06-26

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added adjustable task-list sidebar width.
- Added resizing and collapsing to the child-task panel.
- Added decision-source information to cockpit task waiting reasons for clearer status checks.

<details>
<summary>日本語のリリースノート</summary>

- タスクリストのサイドバー幅を調整できるように
- 子タスクパネルの幅調整と折りたたみに対応
- cockpit task の待機理由表示に判定元情報を追加し、状態確認を改善

</details>

## v4.19.2 — 2026-06-26

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Improved cockpit task conversation output, duplicate Visual Runtime entries, and Visual Runtime history display.

<details>
<summary>日本語のリリースノート</summary>

- cockpit task の会話出力を安定化し、Visual Runtimeタスクの重複表示と履歴表示を改善

</details>

## v4.19.1 — 2026-06-25

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Improved cockpit task waiting-reason detection.
- Fixed image attachments missing from the first task created in the PWA.
- Improved Antigravity usage and quota display.
- Improved cockpit skill guidance for image and video generation workflows.
- Fixed display and controls in Creative Studio, the model picker, and Cockpit popovers.
- Improved Codex Visual by carrying priority-execution settings to Fast-compatible models.

<details>
<summary>日本語のリリースノート</summary>

- cockpit task によるタスクの待機理由表示をより正確に判定するよう改善
- PWAで初回タスク作成時の画像添付が正しく反映されるよう修正
- Antigravityの使用量とquota表示を改善
- 画像・動画生成ワークフロー向けのcockpit スキル案内を改善
- Creative Studio、モデル選択画面、Cockpitポップアップ周りの表示と操作を修正
- Codex Visualの優先実行設定をfast対応モデルへ引き継ぐよう改善

</details>

## v4.19.0 — 2026-06-24

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added the cockpit gen-image command for Codex, Antigravity, and Grok Build.
- Added the cockpit gen-video command for Grok Build.
- Added KDP Paperback publishing settings to Picture Book Studio.
- Improved KDP PDF package generation and review-file reliability.

<details>
<summary>日本語のリリースノート</summary>

- cockpit gen-image コマンドを追加（Codex / Antigravity / Grok Build）
- cockpit gen-video コマンドを追加（Grok Build）
- 絵本制作スタジオでKDP Paperback向けの出版設定を指定できるように
- KDP向けPDFパッケージ生成とレビュー用ファイルの安定性を改善

</details>

## v4.18.1 — 2026-06-19

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Improved Picture Book Studio packaging and task display.

<details>
<summary>日本語のリリースノート</summary>

- 絵本制作スタジオのパッケージ化とタスク表示を改善

</details>

## v4.18.0 — 2026-06-18

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added a picture-book production mode to Content Studio.
- Improved task creation, review, and PWA display for picture-book production.
- Added the OpenRouter Fusion model preset.
- Improved the readability of image-preview prompts.
- Improved the organization of task action buttons and Content Studio UI.
- Fixed Claude usage display and terminal paste behavior on Windows.
- Fixed Markdown numbered list display.

<details>
<summary>日本語のリリースノート</summary>

- Content Studioに絵本制作モードを追加
- 絵本制作ワークフローのタスク作成、レビュー、PWA表示を改善
- OpenRouter Fusionのプリセットモデルを追加
- 画像プレビューのプロンプト表示を見やすく改善
- タスク操作ボタンとContent Studio周りのUIを整理
- WindowsでのClaude使用量表示とターミナル貼り付け動作を修正
- Markdownの番号付きリスト表示を修正

</details>

## v4.17.1 — 2026-06-12

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added agent CLI installation-status checks and an in-app installation guide.
- Improved guidance for uninstalled agent CLIs during task creation.
- Added Terminal task creation to Master workspaces.
- Improved right-side-panel controls so they do not shift focus to the task.
- Improved resizing of the right side panel and terminal tabs while displaying iframes and webviews.
- Improved terminal support for copy shortcuts.

<details>
<summary>日本語のリリースノート</summary>

- エージェントCLIのインストール状態確認とアプリ内インストール導線を追加
- タスク作成時に未インストールのエージェントCLIを分かりやすく案内
- マスターWorkspaceでもTerminalタスクを作成できるように
- 右サイドパネルの操作でタスクにフォーカスが移らないよう改善
- iframeやwebview表示中の右サイドパネルとターミナルタブのリサイズ操作を安定化
- ターミナルでコピー系ショートカットを使えるよう改善

</details>

## v4.17.0 — 2026-06-11

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added Creative Studio for creating and reviewing 3D-model production tasks.
- Added preview, animation playback, and model-download options to the 3D-model review screen.
- Added managed CadQuery and Blender toolchains.
- Added output exports by version and exports that preserve the file structure.
- Added Creative Studio output review to the PWA.
- Added Creative Studio actions to Cockpit CLI.
- Improved detection of Claude Code trust confirmation dialogs.
- Fixed date and time editing for one-time Autoruns.
- Improved help for the cockpit display command.

<details>
<summary>日本語のリリースノート</summary>

- Creative Studioを追加し、3Dモデル制作タスクを作成・確認できるように
- 3Dモデルのレビュー画面でプレビュー、アニメーション再生、自動回転、拡大表示に対応
- CadQueryとBlenderのマネージドツールチェーンに対応
- 生成物のバージョン別エクスポートとファイル構造を保った書き出しに対応
- PWAからCreative Studioの生成物をレビューできるように
- Creative Studio関連のcockpit CLI操作を追加
- Claude Codeの信頼確認ダイアログ検出を改善
- オートランの一回実行日時編集を修正
- cockpit displayコマンドのヘルプ表示を改善

</details>

## v4.16.2 — 2026-06-10

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added Claude Fable 5 selection to Claude Visual.
- Added legacy-format support to Codex priority-execution settings.

<details>
<summary>日本語のリリースノート</summary>

- Claude Visual で Claude Fable 5 を選択できるように
- Codex の優先実行設定で従来形式の設定にも対応

</details>

## v4.16.1 — 2026-06-09

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added the cockpit display command.
- Added update checks and installation to Settings.
- Added a collapsible task list.
- Added shortcut settings for the right side panel and task list.
- Improved right-side-panel open and close controls and tooltips.
- Improved Cockpit CLI authentication and side-panel controls on Windows.
- Improved accuracy of restoring Codex sessions.

<details>
<summary>日本語のリリースノート</summary>

- cockpit display コマンドを追加
- 設定画面からアップデート確認とインストールを実行できるように
- タスク一覧を折りたたみできるように
- 右サイドパネルとタスク一覧のショートカット設定を追加
- 右サイドパネルの開閉操作とツールチップを改善
- Windows版 cockpit CLI の認証とサイドパネル操作を改善
- Codexセッションの復元精度を改善

</details>

## v4.15.1 — 2026-06-05

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Fixed the task diff view showing outdated changes.
- Removed the application menu from the Windows version.

<details>
<summary>日本語のリリースノート</summary>

- タスクの差分表示で現在の変更内容が正しく表示されるよう修正
- Windows版でアプリケーションメニューを非表示に

</details>

## v4.15.0 — 2026-06-05

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added Project Explorer.
- Added file editing and previews to Project Explorer.
- Improved terminal tabs and send actions in the right side panel.
- Added the cockpit side-panel command.
- Added cockpit task goto and current commands.

<details>
<summary>日本語のリリースノート</summary>

- プロジェクトエクスプローラーを追加
- プロジェクトエクスプローラーでファイル編集とプレビューに対応
- 右サイドパネルのターミナルタブと送信操作を改善
- cockpit side-panel コマンドを追加
- cockpit task goto/current コマンドを追加

</details>

## v4.14.0 — 2026-06-04

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added the in-app browser through cockpit browser.
- Improved the chat message UI.
- Fixed theme rendering in the Ask window.
- Improved waiting-state detection in the Claude terminal.

<details>
<summary>日本語のリリースノート</summary>

- アプリ内ブラウザを追加（cockpit browser）
- チャットメッセージUIを改善
- Askウィンドウのテーマ表示を修正
- Claudeターミナルの待機状態判定を改善

</details>

## v4.13.2 — 2026-06-04

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Improved light-theme rendering across the app.

<details>
<summary>日本語のリリースノート</summary>

- ライトモードでの各画面の表示をさらに改善

</details>

## v4.13.1 — 2026-06-03

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Changed status sorting to place running tasks first.
- Improved navigation to parent tasks.
- Fixed the appearance of screen display and task name editing in light mode.
- Improved running-task display in the PWA.
- Fixed the AI message copy-button position.

<details>
<summary>日本語のリリースノート</summary>

- ステータス並び替えで実行中のタスクを上部に表示
- 親タスクへのナビゲーション表示を分かりやすく改善
- ライトモードでの画面表示とタスク名編集の見た目を修正
- PWAでの実行中タスクの表示を調整
- AIメッセージのコピーボタンの位置を修正

</details>

## v4.13.0 — 2026-06-03

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Improved light-theme rendering and terminal theme settings.
- Added creation-date and update-date sorting to the task list.
- Improved task activity display and attention scoring.
- Improved restoration when opening completed Terminal tasks.
- Improved the selected task-group display in the PWA.
- Fixed PowerShell CLI submission and Claude resume status on Windows.

<details>
<summary>日本語のリリースノート</summary>

- ライトテーマの表示とターミナルテーマ設定を改善
- タスクリストに作成日・更新日の並び替えを追加
- タスクの活動表示と注目度スコアを改善
- 完了済みターミナルタスクを開いたときの復元動作を改善
- PWAで選択中のタスクグループを分かりやすく表示
- Windows環境のPowerShell CLI送信とClaude再開ステータスを修正

</details>

## v4.12.0 — 2026-06-02

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Improved Windows behavior and packaging.
- Added task and workspace pinning to the Cockpit CLI.
- Added a child-task action menu.
- Improved state retention and diff display in the right side panel.
- Improved handling of completed Terminal tasks.

<details>
<summary>日本語のリリースノート</summary>

- Windows版の動作とパッケージングを改善
- Cockpit CLI からタスク・ワークスペースをピン留めできるように
- 子タスクの操作メニューを追加
- 右サイドパネルの状態保持と差分表示を改善
- 完了済みターミナルタスクの扱いを改善

</details>

## v4.11.6 — 2026-05-30

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Improved default model selection in Claude Visual.
- Added Claude Opus 4.8 support.

<details>
<summary>日本語のリリースノート</summary>

- Claude Visual のデフォルトモデル選択を改善
- Claude Opus 4.8 に対応

</details>

## v4.11.5 — 2026-05-30

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Improved file-change diff display.

<details>
<summary>日本語のリリースノート</summary>

- ファイル変更差分の表示を改善

</details>

## v4.11.4 — 2026-05-30

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Improved performance.

<details>
<summary>日本語のリリースノート</summary>

- パフォーマンス改善

</details>

## v4.11.3 — 2026-05-30

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Improved Codex Visual task startup speed.

<details>
<summary>日本語のリリースノート</summary>

- Codex Visual タスクの起動を高速化

</details>

## v4.11.2 — 2026-05-30

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added collapsing to project headers.
- Improved file-change updates in the right side panel.
- Changed the new-task menu to close when clicking outside it.
- Fixed bugs.

<details>
<summary>日本語のリリースノート</summary>

- プロジェクトヘッダーを折りたたみ可能に
- 右サイドパネルのファイル変更の更新を改善
- 新規タスク作成のドロップダウンを外側クリックで閉じるように
- バグ修正

</details>

## v4.11.1 — 2026-05-29

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Changed HTML Mode to a free-form design.
- Fixed the HTML Mode toolbar in maximized and inline views.
- Fixed sent text remaining in the terminal input field.

<details>
<summary>日本語のリリースノート</summary>

- HTML Mode をフリーフォームデザインに刷新
- HTML Mode のツールバーを固定表示（最大化時・インライン表示の両方）
- ターミナル入力欄にプログラム送信後の入力が残る問題を修正

</details>

## v4.11.0 — 2026-05-29

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added status sorting to the task list and PWA search.
- Improved workspace selection for master tasks.
- Added folder creation to the directory picker.
- Improved performance by sharing the Codex Visual app server across tasks.
- Added per-agent defaults for approval mode.
- Improved task status detection in Cursor.

<details>
<summary>日本語のリリースノート</summary>

- タスクリストにステータスソートを追加（PWA では検索にも対応）
- マスタータスクのワークスペース選択を統合
- ディレクトリピッカーでフォルダを新規作成できるように
- Codex Visual の app-server を複数タスクで共有しパフォーマンスを改善
- 承認モードの初期値をエージェントごとに設定できるように
- Cursor のタスクステータス検出を改善

</details>

## v4.10.0 — 2026-05-24

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added Cursor CLI as an agent.
- Improved the agent selector on the task-creation screen and restored default-agent selection.
- Improved agent icon presentation.
- Fixed chat scroll tracking, Cockpit model-selector stacking, AVIF image attachments, Cursor CLI status restoration, and Master task directory behavior.

<details>
<summary>日本語のリリースノート</summary>

- Cursor CLI エージェントに対応
- タスク作成画面のエージェント選択 UI を改善（デフォルトエージェント選択を復活）
- エージェントアイコンの UI を整理
- 複数のバグ修正（チャットスクロールの追従、Cockpit モデルセレクタの重ね順、AVIF 画像添付、Cursor CLI のタスクステータス復元、マスタータスクのディレクトリ挙動）

</details>

## v4.9.2 — 2026-05-21

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Fixed Visual task completion detection, Claude usage retrieval, the file-change diff panel, and HTML Mode code-block display.

<details>
<summary>日本語のリリースノート</summary>

- 複数のバグ修正（Visual タスクの完了判定、Claude 使用量取得、ファイル変更差分パネル、HTML Mode コードブロックの表示など）

</details>

## v4.9.1 — 2026-05-21

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Changed Gemini agents to Antigravity throughout the app.
- Added descriptions to Cockpit Ask choices.
- Added free-form input alongside multi-select Cockpit Ask questions.
- Improved Cockpit Ask UI and selection controls.
- Fixed Antigravity history and usage dashboards.

<details>
<summary>日本語のリリースノート</summary>

- Gemini エージェントを Antigravity に完全移行
- Cockpit ask の選択肢に説明を表示できるように
- Cockpit ask の複数選択質問で自由記入も併用可能に
- Cockpit ask の UI と選択操作を改善
- Antigravity の履歴・使用量ダッシュボードを修正

</details>

## v4.9.0 — 2026-05-20

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added Antigravity CLI by integrating the Gemini agent as Antigravity.
- Added multi-select Cockpit Ask questions and Shift+Enter for free-form input.
- Added a task-specific terminal to the right side panel.
- Added Cmd+J and Ctrl+J shortcuts for the terminal and right side panel.
- Added QR-code configuration for PWA connections.
- Improved per-task retention and restoration of right-side-panel state.

<details>
<summary>日本語のリリースノート</summary>

- Antigravity CLI に対応（Gemini エージェントを Antigravity として統合）
- Cockpit ask が複数選択質問に対応、自由記入で Shift+Enter が使えるように
- 右サイドパネルにタスク専用ターミナルを追加
- 右サイドパネルにショートカットキー（Cmd-J: ターミナル開閉、Ctrl-J: 右パネル開閉）を追加
- PWA との接続を QR コードで設定可能に
- 右サイドパネルの状態をタスクごとに保持・復元

</details>

## v4.8.1 — 2026-05-19

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Improved long-press behavior for PWA tasks.
- Improved PWA task display width.
- Improved Autorun badge display by simplifying it.
- Fixed child-task rail scrolling, duplicate Git summaries, and long inline-code wrapping in the PWA.

<details>
<summary>日本語のリリースノート</summary>

- PWAでタスクを長押しした時の動作を改善
- PWAでのタスク表示幅を最適化
- Autorun バッジ表示を簡素化
- PWA の不具合を複数修正（子タスクレールのスクロール、git サマリーの重複表示、長いインラインコードの折り返し）

</details>

## v4.8.0 — 2026-05-18

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added HTML Mode for rendering assistant responses as HTML and returning button actions to tasks, including in the PWA.
- Added Attention Overview for an overlay summary of tasks that need attention.
- Added Master Agent to guest mode.
- Removed Kanban and Pixel modes.
- Added multiple-question support to Master Agent and Cockpit Ask.
- Added skill picker to PWA terminal mode.
- Added agi-worker to AGI Labo skills.
- Changed Visual Runtime history to paginated loading for large histories.
- Added zoom controls to Settings.
- Improved task display and attention-ranking actions in Overview and Focus modes.
- Improved PWA task layout.
- Improved chat drawing performance.
- Fixed Visual Runtime stalls, completion status, tool approval, history persistence, overlapping headers, and long-URL wrapping.

<details>
<summary>日本語のリリースノート</summary>

- HTML Mode に対応：アシスタントの返答を HTML として描画し、ボタンクリックでタスクにアクションを返せるように（PWA でも利用可能）
- Attention Overview を追加：注目タスクを俯瞰できるオーバーレイ表示
- ゲストユーザーでも Master Agent を利用可能に
- Kanban / Pixel モードを廃止
- Master Agent / Cockpit ask が複数質問に対応
- PWA ターミナルモードにスキルピッカーを追加
- AGI Lab スキルに agi-worker を追加
- Visual Runtime の履歴をページング読み込みに変更し、大量履歴でも快適に
- 設定にズーム調整を追加
- オーバービュー / フォーカスモードのタスク表示と注目ランクのアクションを磨き込み
- PWA のタスクレイアウト改善
- チャット描画パフォーマンスを向上
- その他、複数のバグ修正（Visual ランタイムの固まり・完了状態・ツール承認・履歴永続化・ヘッダーの重なり・長URL折り返しなど）

</details>

## v4.6.0 — 2026-05-11

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Changed the mobile PWA task-creation screen to match Desktop features, including Master Agent switching, file attachments, and skill selection.
- Changed the default display to Focus mode.
- Changed display-mode selection for Terminal and Visual to Settings.
- Removed completed child tasks from the right side panel.
- Improved Claude background-task visualization by excluding regular Bash results, retaining pre-start notifications, and fixing occasional missing completion states.

<details>
<summary>日本語のリリースノート</summary>

- PWA（モバイル）のタスク作成画面を刷新し、デスクトップ版と同等の機能（Master Agent 切替・ファイル添付・スキル選択）に対応
- 表示モードのデフォルトをフォーカスモードに変更
- 表示モード選択（ターミナル / ビジュアル）を設定画面に移動
- 完了した子タスクを右サイドパネルから非表示に
- Claude のバックグラウンドタスクの可視化を強化（通常 Bash 結果の誤検出を除外、起動前に届いた通知の取りこぼしを防止、完了状態が稀に反映されない問題を修正）

</details>

## v4.5.1 — 2026-05-11

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added Claude Visual background Bash task status and output to composer chips and the log panel.

<details>
<summary>日本語のリリースノート</summary>

- Claude Visual モードで Bash のバックグラウンドタスクを可視化（状態・出力を入力欄のチップとログパネルから確認できるように）

</details>

## v4.5.0 — 2026-05-11

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added completed tasks to Focus mode attention ranking with bulk deletion.
- Added follow-up messages to completed tasks.
- Improved Focus mode by preserving group expansion and preferring the next task in the same directory after closing a task.
- Added line-number support to file-preview links.
- Fixed the task-name editor position on the task-creation screen.

<details>
<summary>日本語のリリースノート</summary>

- フォーカスモードの注目ランクに完了タスクを表示し、まとめて削除できるように
- 完了したタスクにも続けてメッセージを送れるように
- フォーカスモードのグループ展開状態を保持し、タスクを閉じた後は同じディレクトリ内の次タスクを優先表示
- ファイルプレビューのリンクが行番号に対応
- タスク作成画面のタスク名エディタの表示位置を修正

</details>

## v4.4.3 — 2026-05-08

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Fixed image pasting from the clipboard in Visual mode.
- Added initial Visual-task attachments to chat.
- Improved Visual-mode performance with large diffs or image data.
- Improved the recency score in attention ranking.

<details>
<summary>日本語のリリースノート</summary>

- Visual モードで画像のクリップボード貼り付けが効かない問題を修正
- Visual タスクの初期添付ファイルがチャットに表示されるように
- 巨大な diff や画像データで Visual モードの動作が重くなる問題を改善
- 注目ランクの最近度スコアを調整

</details>

## v4.4.2 — 2026-05-06

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Fixed AskUserQuestion answers failing to send in Claude Visual mode.
- Improved stability of equal-rank task ordering in attention ranking.

<details>
<summary>日本語のリリースノート</summary>

- Claude Visual モードで AskUserQuestion の回答が正しく送信されない問題を修正
- 注目ランクの同順位タスクの並び順を安定化

</details>

## v4.4.1 — 2026-05-03

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added task pinning to Focus mode.
- Fixed missing result reports while Codex was idle.
- Fixed duplicate reports during status playback.
- Changed Autorun to run only while AGI Cockpit is open and removed operating-system scheduler registration.

<details>
<summary>日本語のリリースノート</summary>

- フォーカスモードでタスクをピン留めできるように
- Codex がアイドル状態のときに結果が報告されない問題を修正
- ステータス再生時に同じ報告が重複する問題を修正
- Autorun を AGI Cockpit 起動中のみ動作するように変更（OS スケジューラ登録を廃止）

</details>

## v4.4.0 — 2026-04-30

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Changed the task-creation screen design.
- Added Visual and Terminal mode selection to Autorun.
- Fixed Visual-mode Autoruns failing to start or detect completion correctly.
- Fixed Autorun starting through the operating-system scheduler after AGI Cockpit exited.
- Fixed AGI Cockpit moving to the foreground during Autorun execution.
- Added Autorun badges to Focus mode attention ranking.
- Added links to plugin-provided skill chips in chat.

<details>
<summary>日本語のリリースノート</summary>

- タスク作成画面を刷新
- Autorun で Visual / Terminal モード選択に対応
- Visual mode の Autorun が正しく起動・完了判定されない問題を修正
- Autorun が AGI Cockpit 終了後も OS スケジューラから起動してしまう問題を修正
- Autorun 実行時に AGI Cockpit が前面へ移動してしまう問題を修正
- フォーカスモードの注目ランクに自動実行バッジを表示
- チャット内のプラグイン由来スキルチップをクリック可能に

</details>

## v4.3.1 — 2026-04-30

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Improved visual-chat display and resumption performance with large command output.

<details>
<summary>日本語のリリースノート</summary>

- 大きなコマンド出力を含むビジュアルチャットの表示・再開が重くなる問題を軽減

</details>

## v4.3.0 — 2026-04-30

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added local voice input to the chat composer when mlx-whisper and ffmpeg are installed.
- Added Anthropic API-key authentication to Claude Visual.
- Improved large-image handling in Codex and Claude image generation and previews.
- Fixed the usage popover remaining black.
- Improved directory display during task creation by abbreviating the home directory as ~.

<details>
<summary>日本語のリリースノート</summary>

- チャット入力欄にローカル音声入力を追加（mlx-whisper と ffmpeg を導入すると利用可能）
- Claude Visual で Anthropic API key 認証を選べるように
- Codex / Claude の画像生成・画像プレビューで大きな画像を扱う際の安定性を改善
- 使用量ポップオーバーが黒いまま表示される問題を修正
- 新規タスク作成時のディレクトリ表示を見やすく（ホームディレクトリを ~ 表示）

</details>

## v4.2.1 — 2026-04-28

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added first-launch onboarding for Cockpit skill and CLI setup.
- Added task unread-state synchronization between the PWA and Desktop.
- Added clickable file paths in inline code and improved command-line detection.
- Improved the PWA task-details layout.
- Removed horizontal task swiping from the PWA and standardized navigation through the task list.
- Fixed PWA task synchronization status failing to update.

<details>
<summary>日本語のリリースノート</summary>

- 初回起動時に Cockpit スキル / CLI のセットアップを案内するオンボーディング画面を追加
- PWA とデスクトップ間でタスクの未読状態を同期
- インラインコード内のファイルパスをクリック可能に（コマンドライン誤認識も改善）
- PWA タスク詳細画面のレイアウトを改善
- PWA でタスク間の横スワイプ移動を廃止（タスク一覧から戻る動線に統一）
- PWA のタスク同期状態が正しく反映されない問題を修正

</details>

## v4.2.0 — 2026-04-27

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added image, video, and PDF file previews.
- Added a Finder action to file previews.
- Added collapsible tree previews for JSON files.
- Added a scroll-to-bottom button to chat.
- Improved file-name and path recognition for Unicode characters, spaces, and folder paths.
- Changed the Visual context display.
- Improved attention-ranking display in Focus mode.
- Improved skill-reference display and grouping.
- Fixed Visual agents failing to start with certain command settings.
- Fixed conversation retrieval in Gemini tasks.
- Fixed Codex Visual turn ordering after compaction.
- Fixed slash-command message display.

<details>
<summary>日本語のリリースノート</summary>

- ファイルプレビューで画像・動画・PDF を開けるように
- ファイルプレビューを Finder で表示できるように
- JSON ファイルを折りたたみ可能なツリー形式でプレビュー
- チャット下部にスクロールボタンを追加
- ファイル名・パスの認識を強化（Unicode 文字・スペース・フォルダパスに対応）
- ビジュアル表示のコンテキスト情報を刷新
- フォーカスモードの注目ランク表示を改善
- スキル参照の表示とグルーピングを改善
- ビジュアルエージェントが特定のコマンド設定で起動しない問題を修正
- Gemini タスクで会話が正しく取得できない問題を修正
- Codex のビジュアルでコンパクション後にターン順序がずれる問題を修正
- スラッシュコマンドのメッセージ表示を修正

</details>

## v4.1.3 — 2026-04-27

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Fixed a false “Claude Code Not Found” message during Claude sign-in.

<details>
<summary>日本語のリリースノート</summary>

- Claude にログイン時に「Claude Code が見つかりません」と表示される問題を修正

</details>

## v4.1.2 — 2026-04-26

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Changed Claude Code sign-in to a terminal flow for more reliable authentication.
- Fixed Claude Visual showing incomplete task-wide diffs.
- Fixed Claude Code appearing missing when its configured command included arguments.

<details>
<summary>日本語のリリースノート</summary>

- Claude Code のサインインをターミナル形式に変更し、認証操作を安定化
- Claude のビジュアル表示でタスク全体の差分が正しく表示されない問題を修正
- 引数付きのClaude Codeコマンド設定で、Claude Codeが見つからないと表示される問題を修正

</details>

## v4.1.0 — 2026-04-25

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added Claude Code and Codex sign-in management to Settings.
- Added immediate sending of the next message while an agent is responding.

<details>
<summary>日本語のリリースノート</summary>

- Claude Code / Codex のサインインを設定画面で管理できるように
- エージェントの応答中でも次のメッセージを「今すぐ送信」できるように

</details>

## v4.0.0 — 2026-04-25

**Type:** major · **Platforms:** Windows, macOS, Linux

- Added Native UI for Codex, Claude, and Gemini with readable tool execution, file diffs, and approvals.
- Changed Native UI to the default while retaining Terminal in Settings.
- Changed the Settings screen design.
- Added cockpit skill installation to Settings.
- Added parallel work on multiple tasks in separate windows.
- Added file diffs and previews to the right side panel.
- Added chat file-name and path links that open previews.
- Added inline Codex image-generation results with one-click download and Finder actions.
- Added a chat font-size setting.
- Added queued messages while an agent responds, persisted per task across restarts.
- Added parent-child result reporting beyond Master Agent tasks.
- Added Native UI for Codex, Claude, and Gemini to the mobile PWA.
- Added authentication to Tailscale access.

<details>
<summary>日本語のリリースノート</summary>

- Codex / Claude / Gemini にネイティブ UI を追加 — ツール実行・ファイル差分・承認などを見やすく表示
- ネイティブ UI をデフォルトに設定（設定でターミナルも引き続き利用可能）
- 設定画面を刷新
- 設定画面から cockpit スキルをインストールできるように
- マルチウィンドウで複数タスクを並行作業できるように
- 右サイドパネルでファイル差分とファイルプレビューを表示
- チャット内のファイル名・パスをクリックするとプレビューが開くように
- Codex の画像生成結果をチャット内にインライン表示、ワンクリックでダウンロード・Finder で表示
- チャットのフォントサイズを設定で変更できるように
- エージェントの応答中でも次のメッセージを予約送信できるように（タスクごとに保存、再起動後も保持）
- マスターエージェント以外にも親子タスクとして結果を報告できるように
- PWA（モバイル）で Codex / Claude / Gemini のネイティブ UI に対応
- Tailscale 経由のアクセスに認証を追加してセキュリティを強化

</details>

## v3.3.0 — 2026-04-18

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added Japanese and English localization.
- Fixed Claude Agent resume failures.
- Added left and right arrow navigation back to task cards.

<details>
<summary>日本語のリリースノート</summary>

- 多言語対応（日本語・英語）
- Claude エージェントの resume が失敗するバグを修正
- タスクカードの左右矢印ナビゲーションを復活

</details>

## v3.2.1 — 2026-04-15

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Improved attention ranking by grouping child tasks under the Master task.

<details>
<summary>日本語のリリースノート</summary>

- 注目ランクで子タスクをマスタータスクの下にまとめて表示するよう改善

</details>

## v3.2.0 — 2026-04-15

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added AGI Labo account sign-in through OAuth SSO.
- Changed the first launch after the update to require a one-time sign-in.

<details>
<summary>日本語のリリースノート</summary>

- AGIラボ (agi-labo.com) アカウントでログインできるように（OAuth SSO対応）
- 初回起動時に1度だけ再ログインが必要

</details>

## v3.1.1 — 2026-04-12

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Fixed unread badges reappearing on tasks awaiting confirmation.

<details>
<summary>日本語のリリースノート</summary>

- 確認待ちタスクで未読バッジが再表示されるバグを修正

</details>

## v3.1.0 — 2026-04-11

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added attention ranking with unread tracking and Focus mode.
- Added a Focus tab and attention panel to the PWA.
- Added origin validation to the PWA API and WebSocket.
- Fixed OpenCode binary support on Windows.

<details>
<summary>日本語のリリースノート</summary>

- 注目ランク機能を追加（未読追跡・フォーカスモード）
- PWAにフォーカスタブと注目パネルを追加
- PWA APIとWebSocketのオリジン検証を追加
- Windowsでのopencodeバイナリ対応を修正

</details>

## v3.0.2 — 2026-04-07

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added inline Cockpit Agent conversations to the terminal view.
- Fixed Master task detection and the isYou flag in the task list.

<details>
<summary>日本語のリリースノート</summary>

- Cockpit Agentの会話をターミナルビューにインライン表示
- タスクリストのマスタータスク判定とisYouフラグの修正

</details>

## v3.0.1 — 2026-04-07

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added cockpit as an official task, Autorun, and default-agent option for Master Agent.
- Changed Master Agent help and operations guidance to use consistent cockpit agent options.

<details>
<summary>日本語のリリースノート</summary>

- マスターエージェントの task / autorun / defaultAgent から cockpit を正式に選択可能に
- master 向け help と運用ガイドで cockpit エージェントの選択肢表示を統一

</details>

## v3.0.0 — 2026-04-07

**Type:** major · **Platforms:** Windows, macOS, Linux

- Added Cockpit Agent to the same board as Claude Code, Codex, and Gemini.
- Added Cockpit task creation, conversations, and permission responses to the PWA.
- Improved Cockpit session resumption, task-specific settings, master linkage, and completion processing.

<details>
<summary>日本語のリリースノート</summary>

- Cockpitエージェントを正式追加し、Claude Code・Codex・Geminiと同じボード上で一元管理可能に
- PWAからCockpitタスクの作成・会話・権限応答に対応し、モバイル運用を強化
- Cockpitのセッション再開・タスク別設定・マスター連携・完了処理まわりを安定化

</details>

## v2.15.0 — 2026-03-30

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Changed the Settings panel to a two-column grid.
- Added a shortcut settings dialog for task exit, navigation, and completion keys.
- Changed the AI agent selector to a dropdown.
- Improved terminal color-theme settings with a three-row inline layout.
- Added full-screen media previews to the Ask window.
- Added a confirmation dialog for closing with Cmd+W.
- Fixed the server lifecycle on macOS.

<details>
<summary>日本語のリリースノート</summary>

- 設定パネルを2カラムグリッドレイアウトに刷新
- ショートカット設定ダイアログを追加（タスク終了・ナビゲーション・完了のキーカスタマイズ）
- AIエージェントセレクターをドロップダウンに変更
- ターミナルカラーテーマ設定のUI改善（3行インラインレイアウト）
- askウィンドウにフルスクリーンメディアプレビューを追加
- ⌘Wでの閉じる確認ダイアログを追加
- macOSでのサーバーライフサイクル修正

</details>

## v2.14.0 — 2026-03-26

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added hover previews to task cards.
- Added links to Ask URLs in the PWA.
- Fixed the header drag area.
- Fixed Master Agent display in Autorun.

<details>
<summary>日本語のリリースノート</summary>

- タスクカードのホバープレビューを追加
- PWA askのURLをクリッカブルに
- ヘッダードラッグ領域の修正
- オートランのマスターエージェント表示を修正

</details>

## v2.13.0 — 2026-03-25

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added image, audio, and video attachments to cockpit ask.
- Added server-side caching to Tailscale device discovery.

<details>
<summary>日本語のリリースノート</summary>

- cockpit askでメディア添付（画像・音声・動画）をサポート
- Tailscaleデバイス検出のサーバーサイドキャッシュを追加

</details>

## v2.12.1 — 2026-03-24

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Changed the in-app API endpoint to api.agi-labo.com.
- Changed release distribution to releases.agi-labo.com.

<details>
<summary>日本語のリリースノート</summary>

- アプリ内のAPI参照先を api.agi-labo.com に切り替え
- リリース配信先を releases.agi-labo.com に更新

</details>

## v2.12.0 — 2026-03-21

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added file and folder attachments to Terminal.
- Improved the Terminal details header layout.

<details>
<summary>日本語のリリースノート</summary>

- ターミナルにファイル・フォルダ添付機能を追加
- ターミナル詳細ヘッダーレイアウトの改善

</details>

## v2.11.4 — 2026-03-21

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Changed Pixel Office rooms to group by repository.

<details>
<summary>日本語のリリースノート</summary>

- PixelOfficeの部屋をリポジトリごとにグループ化

</details>

## v2.11.3 — 2026-03-20

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Changed Cockpit tasks to group by repository.

<details>
<summary>日本語のリリースノート</summary>

- Cockpitタスクをリポジトリごとにグループ化

</details>

## v2.11.2 — 2026-03-20

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added Cockpit server switching to the PWA.
- Added a device-discovery cache to the remote-access panel.

<details>
<summary>日本語のリリースノート</summary>

- PWAにCockpitサーバー切替機能を追加
- リモートアクセスパネルにデバイス検出キャッシュを追加

</details>

## v2.11.1 — 2026-03-19

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added automatic Tailscale network-device discovery to the remote-access panel.

<details>
<summary>日本語のリリースノート</summary>

- リモートアクセスパネルにTailscaleネットワークデバイス自動検出を追加

</details>

## v2.11.0 — 2026-03-19

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Fixed terminal scroll jumps.
- Changed the update notification position to the left of the toolbar icon.
- Fixed status handling for resumed tasks.
- Improved PWA task details with larger buttons and automatic text-area resizing.
- Added an exit confirmation dialog to prevent accidental app closure.
- Fixed PWA WebSocket reconnection recovery.

<details>
<summary>日本語のリリースノート</summary>

- ターミナルのスクロールジャンプを修正
- アップデート通知をツールバーアイコンの左側に移動
- 再開タスクのステータスハンドリングを修正
- PWAタスク詳細の操作性を改善（ボタン拡大・テキストエリア自動リサイズ）
- アプリ誤終了防止の終了確認ダイアログを追加
- PWA WebSocket再接続復旧の修正

</details>

## v2.10.0 — 2026-03-18

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added an Ask tab to the PWA and improved mobile responses to pending confirmations.
- Improved Ask context by showing the task title and starting-directory name.
- Improved Cockpit CLI runtime discovery so Ask and Autorun commands work outside Master Agent shells.
- Changed PWA Autorun tasks to use the regular task list and match the Desktop Kanban layout.

<details>
<summary>日本語のリリースノート</summary>

- PWAにask確認タブを追加し、保留中の確認リクエストへモバイルから応答可能に改善
- askダイアログにタスクタイトルと起動ディレクトリ名を表示し、確認内容の文脈を強化
- cockpit CLIがruntime情報を自動解決するようになり、master agent外のshellからask/autorun系コマンドを実行可能に改善
- PWAでもautorun実行タスクを通常タスク一覧へ統合し、desktop Kanbanと表示構成を統一

</details>

## v2.9.1 — 2026-03-18

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Fixed the macOS menu bar becoming unresponsive while the Ask dialog was open.

<details>
<summary>日本語のリリースノート</summary>

- askダイアログ表示時にmacOSメニューバーが操作不能になるバグを修正

</details>

## v2.9.0 — 2026-03-18

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Changed Autorun tasks from a dedicated right-side list to the main Kanban board.
- Added Autorun badges to running and completed tasks.
- Fixed Claude usage retrieval failing in installed builds because of PATH or the initial trust prompt.

<details>
<summary>日本語のリリースノート</summary>

- autorunタスクを右側の専用リストからメインKanbanボードへ統合
- autorunタスクに自動実行バッジを追加し、進行中・完了タスク上で識別しやすく改善
- インストール版でClaude usage取得がPATHや初回trust promptの影響で失敗する問題を修正

</details>

## v2.8.0 — 2026-03-18

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added an on-demand usage popover for Claude, Codex, and Gemini.
- Improved shell-based agent startup by passing prompts safely as arguments.
- Improved Claude usage retrieval and fixed packaged apps failing immediately after startup.

<details>
<summary>日本語のリリースノート</summary>

- オンデマンド使用量ポップオーバーを追加し、Claude/Codex/Gemini の使用量確認に対応
- AIエージェント起動時にプロンプトを引数として安全に渡すようにし、シェル経由の起動を安定化
- Claude usage 取得フローを安定化し、packaged app で起動直後に失敗する問題を修正

</details>

## v2.7.1 — 2026-03-18

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Fixed Claude usage retrieval ending immediately in installed builds.

<details>
<summary>日本語のリリースノート</summary>

- インストール版でClaude usage取得が即終了する問題を修正

</details>

## v2.7.0 — 2026-03-18

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Changed the usage display to a toolbar popover.
- Changed usage retrieval to on-demand and removed periodic polling.
- Added detailed usage display for Claude, Codex, and Gemini.

<details>
<summary>日本語のリリースノート</summary>

- 使用量表示を右上ツールバーのポップアップUIに刷新
- 使用量取得をオンデマンド化し、定期ポーリングを廃止
- Claude / Codex / Gemini の詳細 usage 表示を追加

</details>

## v2.6.0 — 2026-03-17

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added task and autorun subcommands to Cockpit CLI.
- Added task creation, listing, details, completion, deletion, renaming, and remote operations to cockpit task.
- Added creation, updating, deletion, toggling, and immediate execution to cockpit autorun.

<details>
<summary>日本語のリリースノート</summary>

- cockpit CLIにtask/autorunサブコマンドを統合
- cockpit task: タスクの作成・一覧・詳細・完了・削除・リネーム・リモート操作に対応
- cockpit autorun: 定期実行タスクの作成・更新・削除・トグル・即時実行に対応

</details>

## v2.5.0 — 2026-03-17

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added real-time user confirmations from agents through cockpit ask.
- Added choices and free-form input to the always-on-top floating window.
- Added dynamic window sizing based on content.

<details>
<summary>日本語のリリースノート</summary>

- cockpit ask: エージェントからユーザーへのリアルタイム確認機能
- 常に最前面に表示されるフローティングウィンドウで選択肢・自由入力に対応
- コンテンツ量に応じたウィンドウの動的サイズ調整

</details>

## v2.4.2 — 2026-03-16

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Fixed names not carrying over to tasks created by Autorun.

<details>
<summary>日本語のリリースノート</summary>

- autorunで作成されたタスクに名前が引き継がれないバグを修正

</details>

## v2.4.1 — 2026-03-10

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Fixed orphan Pixel Office characters not being assigned to rooms.

<details>
<summary>日本語のリリースノート</summary>

- Pixel Officeで部屋に配属されない孤児キャラクターが発生するバグを修正

</details>

## v2.4.0 — 2026-03-10

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added remote task control through Tailscale device discovery.
- Added persistent device aliases.
- Improved worktree cleanup.
- Fixed zombie PTY processes after task completion.
- Changed the SyncServer body-size limit.

<details>
<summary>日本語のリリースノート</summary>

- Tailscaleデバイス検出によるリモートタスク制御
- デバイスエイリアスの永続化
- worktree クリーンアップの改善
- タスク完了時のゾンビPTYプロセス防止
- SyncServerのボディサイズ制限調整

</details>

## v2.3.3 — 2026-03-08

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Fixed new-task click handling.
- Changed Pixel Office button placement.

<details>
<summary>日本語のリリースノート</summary>

- 新規タスクのクリックハンドリング修正
- Pixel Officeボタンの配置変更

</details>

## v2.3.2 — 2026-03-06

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Fixed minor bugs.

<details>
<summary>日本語のリリースノート</summary>

- 軽微なバグ修正

</details>

## v2.3.1 — 2026-03-06

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Fixed minor bugs.

<details>
<summary>日本語のリリースノート</summary>

- 軽微なバグ修正

</details>

## v2.3.0 — 2026-03-06

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added Pixel Office, an interactive office view that represents tasks as characters.
- Added initial task status based on agent type.
- Fixed a 32-bit setTimeout overflow that duplicated monthly or longer cron runs.
- Changed idle timeouts by agent type.
- Improved Pixel Office usability, performance, and layout density.

<details>
<summary>日本語のリリースノート</summary>

- Pixel Office UI の統合 — タスクをキャラクターとして可視化するインタラクティブなオフィスビュー
- エージェントタイプに基づく初期タスクステータスの設定
- setTimeout 32bitオーバーフロー修正（月次以上のcronで重複実行が発生する問題）
- エージェントタイプ別のアイドルタイムアウト調整
- Pixel Office の操作性・パフォーマンス・レイアウト密度の改善

</details>

## v2.2.5 — 2026-03-04

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Fixed duplicate Autorun triggers after app restarts or operating-system resume.

<details>
<summary>日本語のリリースノート</summary>

- アプリ再起動・OS復帰時にautorunが重複発火する問題を修正

</details>

## v2.2.4 — 2026-03-04

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added an execution lock to prevent infinite Autorun spawning.
- Improved Autorun enabled checks, lock safety, and one-time cleanup.
- Fixed an execution-lock leak after a manual kill.
- Added a CLI installation button to the Settings panel.

<details>
<summary>日本語のリリースノート</summary>

- autorun無限スポーン防止（実行ロックの導入）
- autorunのenabled チェック・ロック安全性・once タイプのクリーンアップを強化
- 手動キル時のロックリーク修正
- 設定パネルにCLIコマンドインストールボタンを追加

</details>

## v2.2.3 — 2026-02-28

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Improved and fixed minor issues.

<details>
<summary>日本語のリリースノート</summary>

- 軽微な改善・修正

</details>

## v2.2.2 — 2026-02-28

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Fixed startup freezes with many sessions by making getGitInfo asynchronous and removing countPathLines.
- Added per-agent terminal color-theme settings.

<details>
<summary>日本語のリリースノート</summary>

- 多数のセッションがある場合の起動フリーズ修正（getGitInfoの非同期化、countPathLinesの除去）
- エージェントごとのターミナルカラーテーマ設定を追加

</details>

## v2.2.1 — 2026-02-18

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Improved and fixed minor issues.

<details>
<summary>日本語のリリースノート</summary>

- 軽微な改善・修正

</details>

## v2.2.0 — 2026-02-18

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Changed internal structure and version organization.

<details>
<summary>日本語のリリースノート</summary>

- 内部リファクタリングとバージョン整理

</details>

## v2.1.0 — 2026-02-18

**Type:** minor · **Platforms:** Windows, macOS, Linux

- Added CRUD prompt templates for Master Agent.
- Added template-variable chips and required indicators.
- Added a task-server watchdog and automatic restart flow.
- Fixed weekday plist generation for macOS launchd cron schedules.
- Removed task-server token authentication and standardized port 19280.
- Changed the settings version check to be non-blocking.
- Improved terminal snapshots by optimizing the dirty flag.
- Added an independent task-server port for development mode.

<details>
<summary>日本語のリリースノート</summary>

- マスターエージェント向けプロンプトテンプレート機能（CRUD対応）
- テンプレート変数チップの表示と必須インジケーター
- タスクサーバーのwatchdogと自動再起動フロー
- macOSのlaunchd cron曜日指定のplist生成修正
- タスクサーバーからトークン認証を廃止、固定ポート19280に統一
- 設定のバージョンチェックをノンブロッキング化
- ターミナルスナップショットのdirtyフラグ最適化
- 開発モード用の独立タスクサーバーポート

</details>

## v2.0.14 — 2026-02-16

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Fixed the terminal loading spinner continuing with empty history or a disconnected WebSocket.
- Added a loading spinner while the PWA retrieves terminal data.

<details>
<summary>日本語のリリースノート</summary>

- 空の履歴やWebSocket切断時にターミナルのローディングスピナーが止まらなくなるバグを修正
- PWAでターミナルデータ取得中にローディングスピナーを表示

</details>

## v2.0.13 — 2026-02-14

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added --directory and --name filters to cockpit task list.
- Added task-delegation guidance to Master Agent AGENTS.md.

<details>
<summary>日本語のリリースノート</summary>

- task list コマンドに --directory / --name フィルターオプションを追加
- マスターエージェントのAGENTS.mdにタスク委任ガイドラインを追記

</details>

## v2.0.12 — 2026-02-14

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Fixed Ctrl+V paste support and nested Claude Code detection.
- Added Windows cloud-signing hooks and signature preflight and verification scripts.
- Fixed Windows terminal PATH resolution and the app icon.

<details>
<summary>日本語のリリースノート</summary>

- Ctrl+V ペーストサポートとネストされたClaude Code検出の修正
- Windowsクラウド署名フックと署名プリフライト/検証スクリプト
- WindowsターミナルのPATH解決とアプリアイコンの修復

</details>

## v2.0.11 — 2026-02-12

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Improved Windows support comprehensively.
- Fixed Windows PATH handling by using EncodedCommand to avoid cmd.exe quoting issues.
- Improved tool detection by reading the Windows PATH from the registry.
- Added a guard against duplicate Autorun execution.

<details>
<summary>日本語のリリースノート</summary>

- 包括的なWindows対応の改善
- Windows PATH修正（EncodedCommandによるcmd.exeのクォート問題回避）
- レジストリからWindowsのPATHを取得して確実にツールを検出
- autorun重複実行防止のガードを追加

</details>

## v2.0.7 — 2026-02-11

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added Master Agent support to Autorun.
- Added an isYou marker to the task list.
- Changed Windows Terminal to PowerShell.

<details>
<summary>日本語のリリースノート</summary>

- autorunでのマスターエージェントサポート
- task list に isYou マーカーを追加
- WindowsターミナルをPowerShellに切り替え

</details>

## v2.0.6 — 2026-02-11

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added npm, pnpm, and cargo to the Windows Terminal PATH.
- Added safeStorage for ARM64 Windows.

<details>
<summary>日本語のリリースノート</summary>

- WindowsターミナルのPATHにnpm/pnpm/cargoを追加
- ARM64 WindowsのsafeStorageリリース

</details>

## v2.0.4 — 2026-02-11

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added a skills panel and folder skill badges.
- Added a skill-details dialog with SKILL.md display and deletion.
- Fixed Windows agent-version detection.
- Removed the Python 3 dependency from the Master Agent script and added a Windows .cmd wrapper.
- Added Windows SystemSounds support for notification sounds.
- Improved Windows support for __dirname paths, status watchers, and hook integration.

<details>
<summary>日本語のリリースノート</summary>

- スキルパネルとフォルダスキルバッジの追加
- スキル詳細モーダル（SKILL.md表示・削除機能）
- Windowsエージェントバージョン検出の修正
- masterAgentスクリプトからpython3依存を除去、Windows用.cmdラッパー追加
- 通知サウンドのWindows対応（SystemSounds）
- 包括的なWindows対応（__dirnameパス・ステータスウォッチャー・フック統合）

</details>

## v2.0.3 — 2026-02-08

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Changed Master Agent commands to use relative paths.

<details>
<summary>日本語のリリースノート</summary>

- マスターエージェントのコマンドを相対パスに統一

</details>

## v2.0.2 — 2026-02-08

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Added a sound when status changes to waiting_confirmation.
- Added an on/off notification-volume setting.
- Added a child-task panel to the Master Agent terminal dialog.
- Removed temporary directories from the workspace list.
- Fixed blank terminals for completed tasks.

<details>
<summary>日本語のリリースノート</summary>

- waiting_confirmationステータス変更時のサウンド通知
- 通知音量設定（ON/OFFトグル）
- マスターエージェントのターミナルモーダルに子タスクパネルを追加
- ワークスペース一覧から一時ディレクトリを除外
- 完了タスクのターミナルが空白になる問題を修正

</details>

## v2.0.1 — 2026-02-07

**Type:** patch · **Platforms:** Windows, macOS, Linux

- Fixed duplicate report-back notifications to the parent Master Agent.
- Changed image delivery to child tasks to reset lastNotifiedStatus.

<details>
<summary>日本語のリリースノート</summary>

- 親マスターへのreport-back通知の重複を修正
- 子タスクへの画像送信時にlastNotifiedStatusをリセット

</details>

## v2.0.0 — 2026-02-07

**Type:** major · **Platforms:** Windows, macOS, Linux

- Added simultaneous management of multiple Master Agents on the Kanban board.
- Added Gemini CLI as an agent type.
- Added guest mode.
- Added report-back notifications for Master Agent.
- Added abbreviated task IDs.
- Added Master configuration management to Cockpit CLI.
- Added persistent cross-session notes through memory.md.
- Added per-agent Kanban card label colors.
- Improved task creation with directory selection and description input.
- Changed Master, task, and Autorun navigation to separate sections.
- Added automatic default-agent selection during task creation.

<details>
<summary>日本語のリリースノート</summary>

- マルチマスターエージェント対応 — 複数のマスターをKanbanボード上で同時管理
- Gemini CLIをエージェントタイプとして追加
- ゲストモード対応
- マスターエージェントのreport-back通知機能
- 短縮タスクID表示
- Cockpit CLI（./cockpit）によるマスター設定管理
- memory.mdによるセッション横断の永続メモ
- エージェント別のKanbanカードラベルカラー
- タスク作成UXの改善（ディレクトリ選択・説明入力）
- マスター/タスク/autorunのナビゲーション分離
- タスク作成時のデフォルトエージェント自動適用

</details>

