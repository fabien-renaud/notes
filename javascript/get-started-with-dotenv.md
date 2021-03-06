[Go back to JavaScript](https://github.com/fabien-renaud/notes/blob/master/javascript)

# Get started with Dotenv 💻

### What is Dotenv 💻

[dotenv](https://www.npmjs.com/package/dotenv) is a zero-dependency module that loads environment variables from a .env file into process.env.
 
### Install Dotenv 💻 as dev dependency
 
```sh
npm install -D dotenv
```

### `.env` sample :

```json
# Server
SERVER_HOST=localhost
SERVER_PORT=10081

# Database
DATABASE_HOST=localhost
DATABASE_PORT=5432
DATABASE_NAME=test
DATABASE_USER=postgres
DATABASE_PASSWORD=postgres
```

`package.json` should looks like this:

```json
{
    "name": "dotenv",
    "version": "1.0.0",
    "description": "Get started with dotenv",
    "main": "index.js",
    "scripts": {
        "start": "node -r dotenv/config src/index.js"
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
        "dotenv": "^8.2.0"
    }
}
```

### It works !
*Don't forget to give a* ⭐️ *if this markdown helped you !*
