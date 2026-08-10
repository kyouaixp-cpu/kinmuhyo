# kinmuhyo プロジェクトルール

## プロジェクト概要
勤務表管理アプリ（Firebase Realtime Database + Google Auth + ExcelJS + ICS export）

## /task-diary コマンド
セッション終了時に実行する。以下の4点を振り返り task-diary.md に追記すること。

- ✅ うまくいったこと
- ❌ ダメだったこと
- 💡 発見・気づき
- 📌 次回への申し送り

追記先：~/Library/CloudStorage/Dropbox/claude/kinmuhyo/task-diary.md
形式：## YYYY-MM-DD のヘッダーのもとに箇条書き

## GitHub連携
リモートリポジトリ：https://github.com/kyouaixp-cpu/kinmuhyo （Public）
本体ファイル：index.html（旧kinmuhyo_v53_1.htmlと統合済み。以後このファイルはバージョン番号を付けずgit管理する）
認証：gh CLI（アカウント kyouaixp-cpu）でHTTPS認証済み

### push時のルール
- push は毎回ユーザーに確認してから実行する（自動pushはしない）
- 編集作業前には必ず `git pull` して最新化する（claude.ai側の別チャットからも同リポジトリにpushされる可能性があるため）
- **push実行後、変更したファイルをバージョン番号付きのファイル名にコピーしてユーザーに出力（送付）する**
  - 形式：[元のファイル名]_v[番号].[拡張子]（例：index_v54.html）
  - バージョン番号は都度ユーザーに確認する（ルート CLAUDE.md の既定ルールに準拠）
  - 元のリポジトリ内ファイル（index.html等）はバージョン番号を付けずそのまま維持する。バージョン番号付きコピーは出力用のみ

## 作業中のタスク

### 有給カードの残り日数表示
案1〜3を比較検討中、未決定。

- 案1：見出しの数字だけ換算後にする
- 案2：内訳に「-1時間年休換算1日」を明記する  
- 案3：日単位の残と時間年休込みの実質残を2段表示

次のステップ：案を決定後に実装着手
