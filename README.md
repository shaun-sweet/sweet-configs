[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/) [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)


### Shaun's front end tooling configs

# Table of Contents
1. [Installation](#installation)
2. [Usage](#usage)
  a. [Typescript](#typescript)
  b. [Webpack Configs](#webpack-configs)
    - [Typescript Loader](#typescript-loader)


## Installation
`npm i -D sweet-configs`

## Usage

## Typescript
```json
{
  "include": ["./src/**/*"],
  "exclude": ["node_modules"],
  "compilerOptions": {
    "baseUrl": "./",
    "outDir": "./dist/"
  },
  "extends": "./node_modules/sweet-configs/typescript/tsconfig.json",
}
```

## Webpack Configs

### Typescript Loader
```javascript
const typescriptWebpack = require("./node_modules/sweet-default-configs/webpack/typescript.js");
const merge = require("webpack-merge");
module.exports = merge(typescriptWebpack, {
  entry: "./src/index.ts",  // Pass in your own entry point, can be .jsx
  output: {
    filename: "bundle.js",
    path: __dirname + "/dist"
  },
});
```