[Go back to JavaScript](https://github.com/fabien-renaud/notes/blob/master/javascript)

# Get started with Husky 🐶

### What is Husky 🐶

[Husky](https://www.npmjs.com/package/husky) improves your commits and more 🐶 woof!

### Install Husky 🐶 as dev dependency

```sh
npm install -D husky
```

### Setup `.huskyrc`:

```json
{
    "hooks": {
        "pre-commit": "npm run validate",
        "pre-push": "npm run validate"
    }
}
```

`package.json` should looks like this:

```json
{
    "name": "husky",
    "version": "1.0.0",
    "description": "Get started with Husky",
    "main": "index.js",
    "scripts": {
        "start": "node src/index.js"
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
        "husky": "^4.2.5"
    }
}
```

### It works !

*Don't forget to give a* ⭐️ *if this markdown helped you !*
