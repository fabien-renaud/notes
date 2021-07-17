[Go back to Docker](https://github.com/fabien-renaud/notes/blob/master/docker)

# How to install RabbitMQ on docker 🔨🐳

**Install and run docker image 🐳**
```sh
cmd		docker pull rabbitmq:management
cmd   docker run -d --name rabbit -p 5672:5672 -p 15672:15672 rabbitmq:management
```

**.env file 🌳️**
```dotenv
# Database
MQ_HOST=localhost
MQ_PORT=5672
```

## It works !
*Don't forget to give a* ⭐️ *if this markdown helped you !*
