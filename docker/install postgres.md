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

## It works !
*Don't forget to give a* ⭐️ *if this markdown helped you !*