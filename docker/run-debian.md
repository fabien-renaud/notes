[Go back to Docker](https://github.com/fabien-renaud/notes/blob/master/docker)

# How to run a debian instance 🖥

**Install and run debian 🖥**
```sh
cmd		docker pull debian
cmd		docker run -dit --name linux-debian debian
```

**Run bash in debian container**
```sh
cmd		docker exec -it linux-debian bash
```

## It works !
*Don't forget to give a* ⭐️ *if this markdown helped you !*
