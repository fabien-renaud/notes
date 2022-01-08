[Go back to Docker](https://github.com/fabien-renaud/notes/blob/master/docker)

# How to run a Linux instance 🖥

**Install and run your favorite Linux distrib 🖥 (optional)**

If you don't pull image first, it will be automatically pulled when you first try running it.

| Name   | Tags            |
| ------ | --------------- |
| Ubuntu | ubuntu:22.04    |
| Debian | debian:bullseye |

```sh
# Pull image from Docker registry
cmd	docker pull <image:tag>
```

**Run a persisting Linux instance**

```sh
# -d option run containers in background
# -it option run containers in interactive mode
cmd	docker run -dit --name linux <image:tag>
cmd	docker exec -it linux
```

**Run a Linux instance that auto-remove itself when it exits**

```sh
cmd	docker run -it --rm <image:tag>
```

## It works !

*Don't forget to give a* ⭐️ *if this markdown helped you !*
