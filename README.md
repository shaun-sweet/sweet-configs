[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)


### Shaun's front end tooling configs

# Table of Contents
1. [Installation](#installation)
2. [Typescript](#typescript)

## Installation
`npm i -D sweet-configs`

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