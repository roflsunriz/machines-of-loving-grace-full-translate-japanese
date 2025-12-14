# GitHub Pages 公開手順

このリポジトリは `machines-of-loving-grace.html` を中心にした静的な翻訳資料で構成されているため、特別なビルド手順なしに GitHub Pages で公開できます。以下の手順で誰でもブラウザで閲覧できるようになります。

## 前提

- このリポジトリを GitHub に push してあること
- 公開に利用するブランチが `main` など既存のブランチであること
- `machines-of-loving-grace.html` と `style.css`、`favicon.png` など静的ファイルがルートにあること（既に満たされています）

## 公開手順

1. GitHub 上の本リポジトリページにアクセスし、右上の「Settings（設定）」タブを開きます。
2. 左側の「Pages」または「Pages (GitHub Pages)」セクションを選択します。
3. 「Source（ソース）」欄でブランチを `main`、フォルダーを `/ (root)` に設定し、「Save（保存）」をクリックします。
4. 数秒待つと、ページ上部に「Your site is published at https://<ユーザー名>.github.io/ai-2027/」のような URL が表示されます。
5. 表示された URL をブラウザで開くと、`machines-of-loving-grace.html` が自動的に表示されます。必要なら、`machines-of-loving-grace.html` を直接参照（例: `https://roflsunriz.github.io/machines-of-loving-grace-full-translate-japanese/machines-of-loving-grace.html`）して実装内容を確認します。

## 更新の流れ

- 内容を編集したら `git add/commit/push` で `main` に反映すると、数分以内に GitHub Pages 上も自動で更新されます。
- キャッシュが残って表示が古い場合はブラウザ側のキャッシュをクリアするか、URL にクエリ（例: `?v=2`）を付けて再読み込みすると最新状態を確認できます。

## カスタムドメインや HTTPS

- `Settings > Pages` から「Custom domain」を設定すると独自ドメインでも公開できます。
- HTTPS を有効化する場合は自動的に `Enforce HTTPS` にチェックを入れ、DNS 設定で `CNAME`（カスタムドメイン利用時）や `A` レコードを GitHub の指示通りに設定します。

## 補足

- さらに細かいセクションや翻訳パートを追加したい場合は、HTML 内に `section` や `nav` を加えて構成し、`style.css` を調整した上で再度 push すれば、最新のドキュメントがそのまま公開されます。
