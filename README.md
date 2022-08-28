# purescript-webapp-template

ゆきくらげが PureScript で Web アプリを作る時のテンプレートです。

## 使い方

ビルドされた js ファイルは public/index.js に出力されます。

これを変更するには、package.json の

```
OUTPUT=
```

の部分二か所を変更してください。

### 初期設定

npm が使える環境でリポジトリをクローンして

```
npm run init
```

を実行してください。

### フォーマット

```
npm run format
```

で全 purs ファイルのフォーマットができます。

### watch

常に変更を監視し差分をコンパイルするので毎回ビルドするより高速です。

```
npm run watch
```

### build

ビルドし、minify されたものが出力されます。

```
npm run build
```

## VSCode の設定

VSCode で作業している場合は次の設定でより便利になります。

### PureScript IDE 拡張機能を導入

https://marketplace.visualstudio.com/items?itemName=nwolverson.ide-purescript

### フォーマッタを purs-tidy に変更し、保存時に自動的にフォーマットする

settings.json に設定を追加します。

```
"purescript.formatter": "purs-tidy",
"[purescript]": {
  "editor.formatOnSave": true,
},
```
