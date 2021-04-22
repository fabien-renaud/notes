# Get started with Babel ⚡

### What is Babel ⚡

[Babel](https://www.npmjs.com/package/@babel/core) is a toolchain that is mainly used to convert ECMAScript 2015+ code into a backwards compatible version of JavaScript in current and older browsers or environments.
 
### Install Babel ⚡ as dev dependency
 
```sh
npm install -D @babel/core @babel/cli @babel/preset-env @babel/node @babel/plugin-proposal-throw-expressions
```

### Setup `.babelrc`:

```json
{
    "plugins": ["@babel/plugin-proposal-throw-expressions"],
    "presets": ["@babel/preset-env"]
}
```

`package.json` should looks like this:

```json
{
    "name": "babel",
    "version": "1.0.0",
    "description": "Get started with Babel",
    "main": "index.js",
    "scripts": {
        "start": "babel-node src/index.js"
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
        ...
    },
    "devDependencies": {
        ...
        "@babel/cli": "^7.8.4",
        "@babel/core": "^7.8.6",
        "@babel/node": "^7.8.4",
        "@babel/plugin-proposal-throw-expressions": "^7.8.3",
        "@babel/preset-env": "^7.8.6"
    }
}
```

### It works !
*Don't forget to give a* ⭐️ *if this markdown helped you !*
