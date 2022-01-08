[Go back to JavaScript](https://github.com/fabien-renaud/notes/blob/master/javascript)

# Get started with Dotenv 💻

### What is Dotenv 💻

[dotenv](https://www.npmjs.com/package/dotenv) is a zero-dependency module that loads environment variables from a .env
file into process.env.

### Install Dotenv 💻 as dev dependency

```sh
npm install -D dotenv
```

### `.env` sample :

```dotenv
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

`package.json` should look like this:

```json
{
    "scripts": {
        "start": "node -r dotenv/config src/index.js"
    },
    "devDependencies": {
        "dotenv": "^8.2.0"
    }
}
```

### It works !

*Don't forget to give a* ⭐️ *if this markdown helped you !*
