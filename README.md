# The English Reading Companion

哲学・分析美学の英語論文(特に SEP)を読みこなすための12ヶ月学習プラン。

## 構成

- `index.html` — トップページ(全体概要)
- `phase1.html` — Phase I 基礎体力作り(月1〜3)
- `phase2.html` — Phase II 橋渡し(月4〜6)
- `phase3.html` — Phase III SEP 本丸(月7〜12)
- `principles.html` — 全フェーズ共通の原則と FAQ
- `style.css` — 共通スタイルシート
- `.nojekyll` — GitHub Pages の Jekyll 処理回避用

## GitHub Pages へのデプロイ手順

1. GitHub で新しいリポジトリを作成(例: `reading-companion`)。
2. このフォルダの中身を**そのまま**リポジトリのルートに push する。
   ```
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
3. リポジトリの **Settings → Pages** へ。
4. **Source** を `Deploy from a branch` に設定。
5. **Branch** を `main`、フォルダを `/ (root)` に設定して **Save**。
6. 数分待つと `https://<your-username>.github.io/<repo-name>/` でアクセス可能になる。

## トラブルシューティング

- **404 が出る**: `index.html` がリポジトリ直下にあることを確認。サブフォルダに入れていないか?
- **CSS が当たらない**: ブラウザで Ctrl+F5(強制リロード)。GitHub Pages のキャッシュは数分で更新される。
- **Private リポジトリで Pages が使えない**: 無料プランでは Public リポジトリのみ。Public にするか、Pro プランへ。
- **Jekyll エラーが出る**: `.nojekyll` ファイルが直下に存在するか確認。

## ローカルでの確認

ブラウザで直接 `index.html` を開けば動作する(外部依存は Google Fonts のみ)。
