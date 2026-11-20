# deadlock-guide

Deadlock（Valve）初心者向け「試合タイミング早見表」を GitHub Pages で公開する専用リポジトリ。

## 公開ページ

- `index.html` — 試合タイミング早見表（パワースパイクのソウル節目、時間で解禁される要素、キャンプ出現、ブリッジバフ等の一覧）
- GitHub Pages: Settings → Pages で `main` ブランチ / ルートを公開元に設定

## データの出典

- 数値の正本: [Deadlock Wiki](https://deadlock.wiki/)
- 日本語の立ち回り・目安: [DeadlockTimesJP](https://deadlocktimes.jp/)
- 取得・照合日: 2026-11-20（新パッチ後は再確認が必要）

元データのキャッシュは別途 `TIMINGS.md` として管理している（このリポジトリには含まない）。

## 編集の運用（2026-11-20〜）

- 編集マスターはローカルの `~/workspace/deadlock-guide/site/index.html`（このフォルダ）。
- ページの実装変更は Claude Code（`~/workspace/bin/claude-vm`）に依頼し、Muse が指示する（司令塔ルール）。ブラウザ操作などは Muse が直接行う。
- 反映は `gh_push.py` で main へ push して簡潔に報告する。このプロジェクトのページ確認は Mikami 本人が行うため、Muse 側の公開版検証はしない（2026-11-20設定）。
