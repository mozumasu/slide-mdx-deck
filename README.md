# mdx-deck

> [!CAUTION]
> 2021 年より、開発が止まっているため使用を断念
> 使用する場合は deprecated になっているパッケージを使用する必要がある

[jxnblk/mdx-deck: ♠️ React MDX-based presentation decks](https://github.com/jxnblk/mdx-deck)

mdx-deck は mdx ベースのスライド作成 Node.js ライブラリ
Markdown 形式でスライドを作成し、React コンポーネントを埋め込むことが可能

## mdx とは

Markdown と JSX の記法を組み合わせたもの

---

## スライドを作成する

```sh
pnpm i -D mdx-deck
```

```sh
WARN  42 deprecated subdependencies found
```

```sh
pnpm update --latest
```

実行時に以下のエラーが出ることがある。

```sh
 WARN  Issues with peer dependencies found
.
└─┬ gatsby 2.32.13
  └─┬ gatsby-plugin-utils 0.9.0
    └── ✕ unmet peer graphql@^15.0.0: found 14.7.0
```

graphql のバージョンが合わないというエラーが出る場合は、以下のコマンドを実行する

```sh
pnpm install graphql@^15.0.0
```

````sh

実行すると以下のものが作成される

```text
node_modules/      package-lock.json  package.json
````

mdx ファイルを作成する
拡張子を.mdx としたファイルを作成する
