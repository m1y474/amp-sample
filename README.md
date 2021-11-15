# amp-sample

- 先頭に `<!doctype html>` の記述が必要
- 最上位階層に `<html ⚡>` or `<html amp>` が必要(AMPコンテンツとして識別する)
- `<head>` `<body>` が必須
- `<head>` の最初の子要素に `<meta charset="utf-8">` を設置
- `<head>` の2番目の子要素に `<script async src="https://cdn.ampproject.org/v0.js"></script>` を設置
- `<head>` の子要素に `<link rel="canonical" href="$SOME_URL">` を設置
- `<meta name="viewport" content="width=device-width,initial-scale=1">`を設置する (※`initial-scale=1`はあくまで推奨)
- `<img />` は使用できず、 `<amp-img></amp-img>` を使用する必要がある
- スタイルは `<head>` の中の `<style amp-custom></style>` に書く
- `<script>`タグは`type`属性が `application/ld+json` または `application/json` のタグのみ設置可能

### 参考
- https://amp.dev/ja/documentation/guides-and-tutorials/start/create/basic_markup/
- https://amp.dev/ja/documentation/guides-and-tutorials/develop/style_and_layout/style_pages/
