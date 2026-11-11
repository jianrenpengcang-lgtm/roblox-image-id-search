# Roblox 画像IDサーチ

Robloxの公開画像アセットを検索し、プレビュー、IDコピー、お気に入り管理、ID照合を行う日本語Webアプリです。

## 構成

- GitHub Pages: 静的なWeb画面
- Replit API: Roblox検索・画像プレビューのAPI
- お気に入り、検索履歴、コピー履歴: 利用者のブラウザー内に保存

## Pages用ビルド

GitHub Pagesの公開パスに合わせて `BASE_PATH=/roblox-image-id-search/` を設定し、`VITE_API_URL` にはReplit APIの公開URLのホスト部分（`/api`を付けない）を指定してビルドします。

`PORT=5000 BASE_PATH=/roblox-image-id-search/ VITE_API_URL=https://<Replitの公開ホスト> pnpm --filter @workspace/roblox-id-search run build`

生成された `artifacts/roblox-id-search/dist/public` の内容をPages用ブランチへ公開します。
