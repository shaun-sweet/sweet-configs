[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)

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