# Get started with Husky 🐶

#### What is Husky 🐶

[Husky](https://www.npmjs.com/package/husky) can prevent bad git commit, git push and more!
 
#### Install Husky 🐶 as dev dependency
 
```sh
npm install -D husky
```

#### Setup `package.json` husky hooks

```json
"husky": {
    "hooks": {
        "pre-commit": "npm run lint",
        "pre-push": "npm run lint"
    }
},
```

`package.json` should looks like this:

```json
{
  "name": "husky",
  "version": "1.0.0",
  "description": "Get started with Husky",
  "main": "index.js",
  "scripts": {
    "start": "nodemon src/index.js"
  },
  "repository": {
    "type": "git",
    "url": "git+https://github.com/fabien-renaud/note.git"
  },
  "husky": {
      "hooks": {
          "pre-commit": "npm run lint",
          "pre-push": "npm run lint"
      }
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

## It works !
*Don't forget to give a* ⭐️ *if this markdown helped you !*
