[Go back to JavaScript](https://github.com/fabien-renaud/notes/blob/master/javascript)

# Get started with Babel, ESLint, Prettier, Dotenv and Nodemon 🍻

## Installation

## Babel ⚡

**What is Babel ⚡**

[Babel](https://www.npmjs.com/package/babel) allow you to use latest JavaScript functionalities, and transpile your code
in older version.</br>
`@babel/core` stand for babel `v7+`, meanwhile `babel/core` stand for older version.

**Install Babel ⚡ as dev dependency**

```sh
npm install -D @babel/core @babel/cli @babel/preset-env @babel/node @babel/plugin-proposal-throw-expressions
```

**Create `.babelrc` file**

```json
{
    "plugins": ["@babel/plugin-proposal-throw-expressions"],
    "presets": ["@babel/preset-env"]
}
```

## ESLint 🔮

**What is ESLint 🔮**

[ESLint](https://www.npmjs.com/package/eslint) find and fix problems in your JavaScript code. It focus on code errors
and best practices.

**Install ESLint 🔮 as dev dependencies**

```sh
npm install -D eslint eslint-config-node eslint-plugin-node
npx install-peerdeps -D eslint-config-airbnb
```

**Create `.eslintrc` file**

```json
{
  "extends": ["airbnb", "prettier"],
  "plugins": ["prettier"],
  "rules": {
    "prettier/prettier": ["error"]
  }
}
```

## Prettier 🌟

**What is Prettier 🌟**

[Prettier](https://www.npmjs.com/package/prettier) format your code to keep it clean.

**Install Prettier 🌟 as dev dependencies**

```sh
npm install -D prettier eslint-config-prettier eslint-plugin-prettier
```

**Create `.prettierrc` file**

```json
{
  "semi": true,
  "proseWrap": "always",
  "arrowParens": "avoid",
  "trailingComma": "all",
  "quoteProps": "as-needed",
  "singleQuote": true,
  "jsxSingleQuote": true
}
```

## Dotenv 💻

**What is Dotenv 💻**

[Dotenv](https://www.npmjs.com/package/dotenv) allow you to load environment variables in runtime, using a `.env` file.

**Install Dotenv 💻 as dev dependency**

```sh
npm install -D dotenv
```

**Create `.env` file**

```text
# App
PORT=10080

# API
USER_API_URL=http://localhost:10081/users
POST_API_URL=http://localhost:10082/posts
```

## Nodemon 😈

**What is Nodemon 😈**

[Nodemon](https://www.npmjs.com/package/nodemon) is a tool that helps develop node.js based applications by
automatically restarting the node application when file changes in the directory are detected.

**Install Nodemon 😈 as dev dependency**

```sh
npm install -D nodemon
```

## Setup `package.json` scripts start

```json
"scripts": {
    "start": "nodemon --exec babel-node -r dotenv/config index.js"
}
```

`package.json` should looks like this:

```json
{
  "name": "todo",
  "version": "1.0.0",
  "description": "Because I'm sick of notepad++",
  "main": "index.js",
  "scripts": {
    "start": "nodemon --exec babel-node -- src/index.js"
  },
  "repository": {
    "type": "git",
    "url": "git+https://github.com/fabien-renaud/note.git"
  },
  "author": "tenrah",
  "license": "ISC",
  "bugs": {
    "url": "https://github.com/fabien-renaud/note/issues"
  },
  "homepage": "https://github.com/fabien-renaud/note#readme",
  "dependencies": {
  },
  "devDependencies": {
    "@babel/cli": "^7.8.4",
    "@babel/core": "^7.8.6",
    "@babel/node": "^7.8.4",
    "@babel/plugin-proposal-throw-expressions": "^7.8.3",
    "@babel/preset-env": "^7.8.6",
    "dotenv": "^8.2.0",
    "eslint": "^6.8.0",
    "eslint-config-airbnb": "^18.0.1",
    "eslint-config-node": "^4.0.0",
    "eslint-config-prettier": "^6.10.0",
    "eslint-plugin-node": "^11.0.0",
    "eslint-plugin-prettier": "^3.1.2",
    "prettier": "^1.19.1"
  }
}
```

## It works !

*Don't forget to give a* ⭐️ *if this markdown helped you !*
