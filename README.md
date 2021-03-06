## Dockerfiles for various things

#### 1. Go Development

The following are steps to start up a docker container that serves as a Go 1.12 development environment. Please note that step 1 intends for users to update the compose yaml file so that they can configure the volumes and environment variables needed for the container

```
1. vim go-dev/go-dev.yml
2. docker-compose -f go-de/go-dev.ymp up -d --build
```

To add a new volume, update the `volumes` section like so:
```
    volumes:
      - <PATH-ON-HOST>:<PATH-IN-CONTAINER>
```

To add a new environment variable, update the `environment` section like so:
```
    environment:
      - <ENV-VAR-NAME>=<ENV-VAR-VALUE>
```