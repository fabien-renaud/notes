# How to install mongodb on docker 🔨🐳

**Install and run docker image 🐳**
```sh
cmd		docker pull mongo
cmd		docker run -d -p 27017:27017 --name mongodb -e MONGO_INITDB_ROOT_USERNAME=root -e MONGO_INITDB_ROOT_PASSWORD=password mongo
```

**.env file 🌳️**
```dotenv
# Database
DB_HOST=localhost
DB_PORT=27017
DB_NAME=
DB_USER=root
DB_PASSWORD=password
```

**URI 🌺**
```js
const uri = `mongodb://${DB_USERNAME}:${DB_PASSWORD}@${DB_HOST}:${DB_PORT}`;
```

## It works !
*Don't forget to give a* ⭐️ *if this markdown helped you !*
