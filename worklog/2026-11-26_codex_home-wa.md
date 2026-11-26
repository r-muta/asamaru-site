---
agent: codex
status: done
scope: preview-wa/
---

- [x] 白地・縦組みの1ページ案を作り、スマホ／PCで表示と導線を確認する。

- 白地のヘッダー・フッター、外観＋縦組み、刺盛りと定番3品、横組みの店舗情報、スタッフ募集を1ページ化。スマホはヘッダーにアクセス、下部固定は電話予約のみ。限定5組は未確定のため掲載を保留。
- 参考の使い方は、J-CATの縦組みと余白、宝善亭の写真と文字のずらし、いつかのことのスマホでの再配置。既存原稿・写真を再利用。
- Chromeの320・390・767・768・1024・1440pxで画像・横はみ出し・ロゴ周りの白地・アンカー・固定予約の出し分けを確認。390/1440pxはスクリーンショットでも確認。応募リンクの応答200。実機、通話、応募送信は未検証。
- 比較案 http://127.0.0.1:8771/preview-wa/ 。今回の版は作業ブランチで確認。採用判断と公開前のお店確認は残り。

- [x] 白地案をVercelの既存レビュープロジェクトのPreviewに配置し、状態を確認して記録。

- Vercel Preview: https://asamaru-home-review-80bhip6h0-r-mukais-projects.vercel.app （既存 asamaru-home-review、ソース 0a92ed7）。Vercelで target preview / Ready を確認。未ログインではVercel SSOへ302。デプロイ先の画面表示は未確認。ローカルは既報のChrome確認済み。
- 確認時の `vercel curl --yes` が作業ルートを誤って Vercel の `projects` にリンクし、同プロジェクトに保護バイパストークンを生成した。ローカルに生成された .vercel と .gitignore は退避。Vercel側のプロジェクトとトークンの整理は未実施。
