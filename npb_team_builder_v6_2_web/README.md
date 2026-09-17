# NPB TEAM BUILDER v6.2 — 公開用

このフォルダを静的ホスティング（GitHub Pages / Cloudflare Pages / Netlify 等）へ置けば、URLを共有するだけでスマートフォンから遊べます。

## GitHub Pages
1. 新しいリポジトリを作成
2. このフォルダ内の `index.html`, `manifest.webmanifest`, `icon.svg`, `sw.js` をリポジトリ直下へ配置
3. Settings → Pages → Deploy from a branch → `main` / `/ (root)`
4. 発行された `https://<user>.github.io/<repo>/` を共有

## 注意
- `file://` で直接開くより、HTTPSで公開して遊ぶ前提です。
- PWA対応済みなので、iPhone/Androidではブラウザの「ホーム画面に追加」も利用できます。
- 現在の能力値更新処理は外部の公開データ取得を試みます。公開先や外部サイト側のCORS制限により取得できない場合、アプリ内の保守的な値へフォールバックします。将来的には能力データを同一サイト内のJSONとして同梱する方式が最も安定します。
