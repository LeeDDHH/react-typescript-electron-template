## 動作環境

|         |         |
| ------- | ------- |
| node.js | 12.21.0 |
| npm     | 6.14.11 |
| yarn    | 1.22.4  |

### install

nodebrew での方法を記載

```zsh
nodebrew install-binary 12.21.0
nodebrew use 12.21.0

(CSS ModuleのDefinitly Typedファイル生成のためのコマンドをグローバルインストールする)
yarn global add typed-css-modules
```

[Quramy/typed-css-modules: Creates .d.ts files from CSS Modules .css files](https://github.com/Quramy/typed-css-modules)

## プロジェクトに必要なライブラリをインストールする

```
(ElectronとTypeSciprt関連)
yarn -D add electron typescript ts-node @types/node

(React)
yarn add react react-dom
(React型定義)
yarn -D add @types/react @types/react-dom

(ESLint と Prettier)
yarn -D add eslint prettier eslint-config-prettier
(TypeScript用ESLint)
yarn -D add @typescript-eslint/parser @typescript-eslint/eslint-plugin
(React関連プラグイン)
yarn -D add eslint-plugin-react eslint-plugin-react-hooks

(Webpack)
yarn -D add webpack webpack-cli webpack-dev-server @types/webpack-dev-server
(Webpackローダー)
yarn -D add ts-loader css-loader
(プラグインとその型定義ファイル)
yarn -D add mini-css-extract-plugin copy-webpack-plugin @types/mini-css-extract-plugin @types/copy-webpack-plugin
(バンドルされたJavaScriptファイルをHTMLの<script>タグに差し込むためのプラグイン)
yarn -D add html-webpack-plugin @types/html-webpack-plugin

(CSSリセッター)
yarn add reseter.css

(Electron devtools関連)
yarn -D add electron-devtools-installer

(ユーティリティ)
yarn -D add rimraf cross-env npm-run-all
```
