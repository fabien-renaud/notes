# How to install Babel ⚡

**Install Babel as dev dependency 💻**

`@babel/core` stand for babel `v7+`, meanwhile `babel/core` stand for older version. 
 
```sh
npm install --save-dev @babel/core @babel/cli @babel/preset-env @babel/node
```

**Adding scripts to package.json 📃**

```json
{ 
    "start": "nodemon --exec babel-node index.js"
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
    "@babel/preset-env": "^7.8.6"
  }
}


```

## It works !
*Don't forget to give a* ⭐️ *if this markdown helped you !*
