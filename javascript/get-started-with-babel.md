[Go back to JavaScript](https://github.com/fabien-renaud/notes/blob/master/javascript)

# Get started with Babel ⚡

### What is Babel ⚡

[Babel](https://www.npmjs.com/package/@babel/core) is a toolchain that is mainly used to convert ECMAScript 2015+ code
into a backwards compatible version of JavaScript in current and older browsers or environments.

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

`package.json` should look like this:

```json
{
    "scripts": {
        "start": "babel-node src/index.js"
    },
    "devDependencies": {
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
