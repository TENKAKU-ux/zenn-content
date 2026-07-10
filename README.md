# zenn-content

[Zenn](https://zenn.dev/tenkaku_ux) で公開する記事を管理するリポジトリです。

## 構成

- `articles/` — 記事の Markdown（1ファイル1記事）

## ローカルプレビュー

```bash
npm install      # 初回のみ（zenn-cli を入れる）
npx zenn preview # http://localhost:8000 で確認
```

## 公開の流れ

1. `articles/<slug>.md` を書く（`published: false` で下書き）。
2. 公開前に秘密スキャンを通し、内容を確認する。
3. 問題なければ `published: true` にして main に push すると、GitHub 連携で Zenn に反映される。

`published: false` の下書きも、push した時点でこの public リポジトリ上では誰でも読めます。秘密や個人情報は最初から書かない前提で扱ってください。

## ライセンス

記事本文の著作権は作者に帰属します。
