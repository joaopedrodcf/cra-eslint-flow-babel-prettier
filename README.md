# cra-eslint-flow-babel-prettier

A project with CRA already configurated with eslint, flow, babel and prettier

## Getting Started

This project assumes that you use vscode

You also need npm version 5+

```
npm -v
```

And is based on some tutorials from the web like this one , shot out to Sean Froff for is awesome tutorial
https://hackernoon.com/configure-eslint-prettier-and-flow-in-vs-code-for-react-development-c9d95db07213

first update your user settings

```
"editor.formatOnSave": true,
"javascript.format.enable": false,
"javascript.validate.enable": false,
"prettier.eslintIntegration": true
```

## Using same project

If you want to use this project as a boilerplate just install flow-bin globaly
To prevent an error from flow extension

```
npm i flow-bin --global
```

Then add this extensions to your setup
https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint
https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode
https://marketplace.visualstudio.com/items?itemName=flowtype.flow-for-vscode
https://marketplace.visualstudio.com/items?itemName=dzannotti.vscode-babel-coloring

## Using other project

```
npx install-peerdeps --dev eslint-config-airbnb
```

```
npm install babel-eslint --save-dev
```

```
npm install prettier-eslint --save-dev
```

```
npm install --save-dev flow-bin babel-preset-flow
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
