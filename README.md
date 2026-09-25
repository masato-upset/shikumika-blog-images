# shikumika-blog-images

シクミルの記事本文から、説明用の挿入画像を設計・生成するClaude Codeプラグインです。

## Claude Codeブラウザ版で使う

ブラウザ版では `/plugin` が利用できない場合があります。その場合は、このリポジトリをClaude Codeの作業リポジトリとして開き、記事本文と、あればサムネイル・使用予定のスクリーンショットを送ってください。

リポジトリ直下の `CLAUDE.md` から挿入画像スキルを読み込みます。

## Claude Code CLIへプラグインとして導入する

Claude Codeで次を実行します。

```text
/plugin marketplace add masato-upset/shikumika-blog-images
/plugin install shikumika-blog-images@shikumika-blog-images
```

インストール後は、記事本文と、あればサムネイル・使用予定のスクリーンショットを渡してください。画像生成に加えて、本文中の具体的な挿入位置とalt案を返します。

明示的に呼び出す場合は `/shikumika-blog-images:generate-blog-images` を使います。
