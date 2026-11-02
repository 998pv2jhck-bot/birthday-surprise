# 誕生日サプライズサイト（GitHub Pages用）

## ファイル
- `index.html` : サイト本体。HTML/CSS/JavaScriptをまとめています。
- `media/` : 写真・動画を入れるフォルダ。

## 写真・動画がまだなくても大丈夫
最初は写真・動画ファイルがなくてもサイトを公開できます。写真・動画の枠には「あとから追加できます」という仮表示が出ます。後日、mediaフォルダにファイルを入れて、下のCONFIGのファイル名を合わせれば表示されます。

## 最初に変更するところ
`index.html` の下の方にある `const CONFIG = { ... }` を編集します。

### パスワード
`password: "HAPPY2026"` を好きな合言葉に変更します。

### 写真・動画
`media` フォルダに写真や動画を入れ、`src` のファイル名を合わせます。
例：
- `media/photo01.jpg`
- `media/movie01.mp4`
- `media/photo02.jpg`

ギフトを増やす場合は `gifts` 配列に同じ形式の項目を追加します。
`type` は `image` / `video` / `message` のいずれかです。

## GitHub Pagesで公開
1. GitHubアカウントにログイン
2. New repository から新しいリポジトリを作る
3. リポジトリ名は例として `birthday-surprise`、Visibilityは Public
4. `index.html` と `media` フォルダをアップロードして Commit
5. リポジトリの Settings → Pages
6. Build and deployment の Source を `Deploy from a branch`
7. Branch を `main`、Folder を `/(root)` にして Save
8. 数分後に表示される `https://ユーザー名.github.io/birthday-surprise/` を開く

## 大事な注意
GitHub FreeでGitHub Pagesを使う場合、リポジトリはPublicです。
アップロードした写真・動画・HTMLは、パスワード画面を通らなくてもファイルURLなどから見られる可能性があります。
このパスワードはサプライズ演出用で、セキュリティ機能ではありません。
個人情報や、公開されたら困る写真・動画はアップロードしないでください。

GitHub Pagesの公開サイト上限は1GBです。GitHubの通常ファイルは1ファイル100MBが上限なので、動画は圧縮するか、YouTubeの限定公開など外部動画サービスへの埋め込みを検討してください。限定公開URLも転送されれば見られます。
