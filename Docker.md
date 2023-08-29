# Docker
- Docker works in 3 pieces: **Client**, **Daemon**, and **Socket**. These three make up the **Docker Engine**.
    - **Client (docker)**: This is the CLI application. It interacts with the daemon via a REST API with the ability to go through TCP (remote daemon).
    - **Daemon (dockerd)**: The daemon actually creates the containers, networks, volumes, etc themselves.
    - **Socket**: Facilitates communication between client and daemon.


## DinD (Docker in Docker)

- Start DinD setup locally.

```bash
# Very important that it is ran dettached at first
# should also pin a dind image version/tag
docker run docker run -d --privileged --name dind-test docker:dind

# exec into dind container
docker exec -it dind-test ash

# start python container
docker run python:3.10
```

