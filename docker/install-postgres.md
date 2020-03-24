# How to install postgres on docker 🔨🐳

**Install and run docker image 🐳**
```sh
cmd		docker pull postgres
cmd		docker run -d -p 5432:5432 --name postgres -e POSTGRES_PASSWORD=postgres postgres
```

**Open docker shell 💻**
```sh
cmd		docker exec -it postgres bash
```

**Login as postgres user 👨‍✈️**
```sh
root#		psql -U postgres
```

**Create a new database ✏️**
```sql
postgres#	CREATE DATABASE $DB_NAME;
```

**.env file 🌳️**
```dotenv
# Database
DB_HOST=localhost
DB_PORT=5432
DB_NAME=
DB_USER=postgres
DB_PASSWORD=postgres
```

**dbConfig 🌺**
```js
const dbConfig = new Sequelize({
    host: process.env.DB_HOST || 'localhost',
    port: Number(process.env.DB_PORT) || 5432,
    database: process.env.DB_NAME || '',
    username: process.env.DB_USER || '',
    password: process.env.DB_PASSWORD || '',
    dialect: 'postgres',
    dialectOptions: {
        connectTimeout: 2000
    },
    timezone: '+01:00'
});
```

## It works !
*Don't forget to give a* ⭐️ *if this markdown helped you !*
