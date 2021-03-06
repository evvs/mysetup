# scripts

npm run
```sh
  "dev": "cross-env NODE_ENV=development npx webpack --mode development",

  "build": "cross-env NODE_ENV=production npx webpack --mode production",

  "watch": "cross-env NODE_ENV=development npx webpack --mode development --watch",

  "start": "cross-env NODE_ENV=development npx webpack-dev-server --mode development --open"

  "lint": "npx eslint ."


```


# webpack

| Plugin | link |
| ------ | ------ |
| HtmlWebpackPlugin | [https://webpack.js.org/plugins/html-webpack-plugin](https://webpack.js.org/plugins/html-webpack-plugin/) |
| CleanWebpackPlugin | [https://www.npmjs.com/package/clean-webpack-plugin](https://www.npmjs.com/package/clean-webpack-plugin) |
| CopyWebpackPlugin | [https://webpack.js.org/plugins/copy-webpack-plugin](https://webpack.js.org/plugins/copy-webpack-plugin/) |
| MiniCssExtractPlugin | [https://webpack.js.org/plugins/mini-css-extract-plugin](https://webpack.js.org/plugins/mini-css-extract-plugin/) |
| OptimizeCssAssetsPlugin | [https://github.com/NMFR/optimize-css-assets-webpack-plugin](https://github.com/NMFR/optimize-css-assets-webpack-plugin/) |
| TerserPlugin | [https://webpack.js.org/plugins/terser-webpack-plugin](https://webpack.js.org/plugins/terser-webpack-plugin/) |




| Loader | link |
| ------ | ------ |
| css-loader | [https://webpack.js.org/loaders/css-loader](https://webpack.js.org/loaders/css-loader/) |
| babel-loader | [https://github.com/babel/babel-loader](https://github.com/babel/babel-loader) |
| file-loader | [https://webpack.js.org/loaders/file-loader](https://webpack.js.org/loaders/file-loader/) |
| less-loader | [https://webpack.js.org/loaders/less-loader](https://webpack.js.org/loaders/less-loader/) |
| sass-loader | [https://webpack.js.org/loaders/sass-loader](https://webpack.js.org/loaders/sass-loader/) |

  
   


# babel

Setup
```sh
npm install --save-dev babel-loader @babel/core
```

 Preset | link |
| ------ | ------ |
| @babel/preset-env | [https://babeljs.io/docs/en/babel-preset-env](https://babeljs.io/docs/en/babel-preset-env) |
| @babel/preset-react | [https://babeljs.io/docs/en/babel-preset-react](https://babeljs.io/docs/en/babel-preset-react) |

 Plugin | 
| ------ | 
| @babel/plugin-proposal-class-properties |

 Polyfill | link |
| ------ | ------ |
| @babel/polyfill | [https://babeljs.io/docs/en/babel-polyfill](https://babeljs.io/docs/en/babel-polyfill) |

# eslint

```sh
npm install eslint babel-eslint eslint-config-airbnb eslint-plugin-react eslint-plugin-react-hooks eslint-plugin-functional --save-dev
```
```sh
env:
  browser: true
  node: true

parser: babel-eslint

extends:
  - airbnb
  - "plugin:react/recommended"
  - "plugin:functional/external-recommended"
  - "plugin:functional/recommended"
  - "plugin:react-hooks/recommended"


plugins:
  - react
  - functional

rules: 
  import/extensions: 0
  react/prop-types: 0
  no-console: 0
  functional/no-conditional-statement: 0
  functional/no-expression-statement: 0
  functional/immutable-data: 0
  functional/functional-parameters: 0
  functional/no-try-statement: 0
  functional/no-throw-statement: 0
```
functional rules https://www.npmjs.com/package/eslint-plugin-functional#supported-rules