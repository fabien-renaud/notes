[Go back to JavaScript](https://github.com/fabien-renaud/notes/blob/master/javascript)

# Get started with Nodemon 😈

### What is Nodemon 😈

[Nodemon](https://www.npmjs.com/package/nodemon) is a tool that helps develop node.js based applications by automatically restarting the node application when file changes in the directory are detected.

### Install Nodemon 😈 as dev dependency

```sh
npm install -D nodemon
```

`package.json` should looks like this:

```json
{
    "name": "nodemon",
    "version": "1.0.0",
    "description": "Get started with Nodemon",
    "main": "index.js",
    "scripts": {
        "start": "nodemon src/index.js"
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
        "nodemon": "^2.0.7"
    }
}
```

### It works !
*Don't forget to give a* ⭐️ *if this markdown helped you !*
