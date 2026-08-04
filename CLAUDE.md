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

## 作業中のタスク

### 有給カードの残り日数表示
案1〜3を比較検討中、未決定。

- 案1：見出しの数字だけ換算後にする
- 案2：内訳に「-1時間年休換算1日」を明記する  
- 案3：日単位の残と時間年休込みの実質残を2段表示

次のステップ：案を決定後に実装着手
