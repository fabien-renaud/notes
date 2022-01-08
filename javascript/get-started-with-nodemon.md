[Go back to JavaScript](https://github.com/fabien-renaud/notes/blob/master/javascript)

# Get started with Nodemon 😈

### What is Nodemon 😈

[Nodemon](https://www.npmjs.com/package/nodemon) is a tool that helps develop node.js based applications by
automatically restarting the node application when file changes in the directory are detected.

### Install Nodemon 😈 as dev dependency

```sh
npm install -D nodemon
```

`package.json` should looks like this:

```json
{
    "scripts": {
        "start": "nodemon src/index.js"
    },
    "devDependencies": {
        "nodemon": "^2.0.7"
    }
}
```

### It works !

*Don't forget to give a* ⭐️ *if this markdown helped you !*
