<!-- Generated from tempi-tech/AGICockpit — do not edit directly. -->

# AGI Cockpitとは

AGI CockpitがどこでAIエージェントを動かし、タスク一覧とタスク詳細を通じて人の判断と成果確認をつなぐのかを説明します。

> AGI Cockpit 4.40.0で2026-07-29に確認済み。 [公式ドキュメントを表示](https://agi-labo.com/tools/cockpit/docs)

AGI Cockpitは、複数のAIエージェントへ仕事を渡し、進捗、判断要求、成果を一つの場所で監督するデスクトップアプリです。タスクを作るところから、結果を確認し、追加指示を送り、完了にするところまでを同じ作業単位で扱います。

## Cockpitが扱う仕事の流れ

1. タスクへ目的と作業場所を設定する
2. 選択したAIエージェントを動かす
3. タスク一覧で、実行中、確認待ち、完了、エラーを見分ける
4. タスク詳細で会話、確認要求、差分、ファイル、画面などを確認する
5. 追加指示、Askへの回答、再開、完了のいずれかへ進む

Cockpitが仕事そのものをクラウドへ移すのではありません。エージェントのプロセスと作業ファイルはCockpitを実行しているコンピューター側にあり、利用するエージェントや外部サービスの通信条件はそれぞれの設定に従います。

## 4つの利用面

| 利用面 | 役割 | 主な利用者 |
| --- | --- | --- |
| Desktop | タスクの作成、一覧、詳細、設定、成果確認の中心 | 利用者 |
| エージェントプロセス | 指示を実行し、会話や変更をタスクへ返す | AIエージェント |
| PWA | 別端末からタスク、Ask、Autorunを確認・操作する | 利用者 |
| `cockpit` CLI | タスク、Ask、Autorun、ブラウザーなどをCockpit経由で操作する | AIエージェントと利用者 |

PWAによるリモートアクセスとAutorunはAGIラボ会員向けです。基本的なタスク実行はゲスト利用でも始められます。

## 最初に読むページ

- 初回セットアップから結果確認まで進める: [インストールと最初のタスク](https://agi-labo.com/tools/cockpit/docs/getting-started)
- 複数の仕事を見分ける: [タスク一覧とタスク詳細](https://agi-labo.com/tools/cockpit/docs/tasks)
- エージェントから人へ判断を渡す: [Ask](https://agi-labo.com/tools/cockpit/docs/ask)
- 時刻や間隔に基づいて新しいタスクを起動する: [Autorun](https://agi-labo.com/tools/cockpit/docs/autorun)

## ゲスト利用とAGIラボ会員

| 利用方法 | この初期ドキュメントで扱う範囲 |
| --- | --- |
| ゲスト利用 | Desktopでタスクを作成し、エージェントを実行して結果と履歴ダッシュボードを確認する |
| AGIラボ会員 | ゲスト利用の範囲に加え、AutorunとPWAによるリモートアクセスを利用する |

機能の入口に鍵が表示される場合、その機能にはサインインが必要です。タスクの実行に使うClaude Code、Codexなどの認証は、AGIラボへのサインインとは別に管理されます。

## 次に進む

[AGI Cockpitをインストールして最初のタスクを実行する](https://agi-labo.com/tools/cockpit/docs/getting-started)と、タスクが一覧へ現れ、詳細から結果を確認できるところまで進めます。
