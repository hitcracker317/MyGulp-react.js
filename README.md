# MyGulp-react.js

## 概要
React.jsの開発環境に適したGulp。

## 導入
以下のパッケージをnpmにインストール。
Bebelとbrowserifyを導入した開発環境。

### Bebel
ES2015,2016の記法をどのブラウザでも対応できるようにコンパイルしてくれる。

```
npm install --save-dev babelify
```

React用のbabelのプリセットをインストール

```
npm install --save babel-preset-react
```

### browserify
複数のjavascriptファイルの依存関係を克服して1つのjavascriptファイルにまとめてくれる。

```
npm install --save-dev browserify
```

### vinyl-source-stream
browserifyのbundle()で吐き出されたオブジェクトがvinylではないのでvinylに変換しなければならない。
gulpはvinylオブジェクトをイジイジしてファイルを書き出しているので、その過程でvinylオブジェクトが存在しなければならない。
そのため、このパッケージをインストールする必要がある。

```
$ npm install --save-dev vinyl-source-stream
```
