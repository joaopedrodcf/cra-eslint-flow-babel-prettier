# cra-eslint-flow-babel-prettier

A project with CRA already configurated with eslint, flow, babel and prettier

## Getting Started

This project assumes that you use VSCODE

And is based on some tutorials from the web like this one , shot out to Sean Froff for is awesome tutorial
https://hackernoon.com/configure-eslint-prettier-and-flow-in-vs-code-for-react-development-c9d95db07213

First update your user settings (CTRL + ,)

```
"editor.formatOnSave": true,
"eslint.autoFixOnSave": true,
"eslint.alwaysShowStatus": true,
```

Install the following extension on VSCODE:

* [Eslint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)

Install yarn (Faster then NPM)
* [yarn](https://yarnpkg.com/en/)

## Using same project

If you want to use this project as a boilerplate just install flow-bin globaly
To prevent an error from flow extension

```
npm i flow-bin --global
```

## Using other project


```
npx install-peerdeps --dev eslint-config-airbnb
```

```
yarn add prettier --dev --exact
```

```
yarn add husky lint-staged --dev
```

```
yarn add babel-eslint eslint-config-prettier eslint-plugin-prettier --dev
```

```
yarn add flow-bin babel-preset-flow --dev
```

```
yarn add --dev stylelint stylelint-processor-styled-components stylelint-config-styled-components stylelint-config-standard
```

Then copy to your workspace the .babelrc , .eslintrc and .flowconfig

If you're using react-native don't use flowtype on the plugins of .eslintrc

## How to use flow

Add // @flow to any files you want to type check (for example, to src/App.js).
This ensures it will type check

```
const add = (a: string, b: string): string => a + b;

add(1, 2);
```

```
npm run flow  start
```

You should see errors in your vscode

## Deploy website to github
```
git checkout -b gh-pages
```

```
yarn add gh-pages --dev
```

```
  "scripts": {
      "predeploy": "npm run build",
      "deploy": "gh-pages -d build",
```

```
yarn run deploy
```
## my project setup

* [babel](https://github.com/babel/babel) - 🐠 Babel is a compiler for writing next generation JavaScript.
* [babel-eslint](https://github.com/babel/babel-eslint) - 🗼 A wrapper for Babel's parser used for ESLint
* [eslint](https://github.com/eslint/eslint) - A fully pluggable tool for identifying and reporting on patterns in JavaScript
* [eslint-config-prettier](https://github.com/prettier/eslint-config-prettier) - Turns off all rules that are unnecessary or might conflict with Prettier. 
* [eslint-plugin-flowtype](https://github.com/gajus/eslint-plugin-flowtype)- Flow type linting rules for ESLint.
* [eslint-plugin-react](https://github.com/yannickcr/eslint-plugin-react) - React specific linting rules for ESLint
* [eslint-plugin-jsx-a11y](https://github.com/evcohen/eslint-plugin-jsx-a11) - Static AST checker for a11y rules on JSX elements.
* [eslint-plugin-import](https://github.com/benmosher/eslint-plugin-import) - ESLint plugin with rules that help validate proper imports.
* [eslint-plugin-babel](https://github.com/babel/eslint-plugin-babel) - An ESlint rule plugin companion to babel-eslint
* [eslint-plugin-prettier](https://github.com/prettier/eslint-plugin-prettier) - ESLint plugin for prettier formatting
* [flow](https://github.com/facebook/flow) - Adds static typing to JavaScript to improve developer productivity and code quality.
* [flow-bin](https://github.com/flowtype/flow-bin) - Binary wrapper for Flow - A static type checker for JavaScript
* [gh-pages](https://github.com/tschaub/gh-pages) - General purpose task for publishing files to a gh-pages branch on GitHub
* [husky](https://github.com/typicode/husky) - 🐶 Git hooks made easy
* [javascript](https://github.com/airbnb/javascript) - JavaScript Style Guide
* [lint-staged](https://github.com/okonet/lint-staged) - 🚫💩 — Run linters on git staged files 
* [prettier](https://github.com/prettier/prettier) - Prettier is an opinionated code formatter.
* [stylelint](https://github.com/stylelint/stylelint) -  A mighty, modern CSS linter
* [stylelint-config-standard](https://github.com/stylelint/stylelint-config-standard) - The standard shareable config for stylelint 
* [stylelint-config-styled-components](https://github.com/styled-components/stylelint-config-styled-components) - The shareable stylelint config for stylelint-processor-styled-components
* [stylelint-processor-styled-components](https://github.com/styled-components/stylelint-processor-styled-components) - Lint your styled components with stylelint! 
