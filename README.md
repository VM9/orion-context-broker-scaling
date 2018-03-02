# Orion Context Broker Scaling
Repository for [Orion Context Broker](https://github.com/telefonicaid/fiware-orion) scaling laboratory and tests

Requiriments
- [Docker](https://www.docker.com/get-docker)
- [Docker compose](https://docs.docker.com/compose/install/)

Usage:
- Place  `docker-compose.yml` into folder
- Run command to start as daemon:

```
docker-compose up -d
```

- Scale orion:
```
docker-compose scale orion=2
```

- Debug and Log

```
 docker-compose logs -f
```


Explanation:

The service `ld`  will start a haproxy server that will include all new orion instances to the balancing, it will bind at port 1026, internally `ld` will bind it at port 80.
More details inside `docker-compose.yml` file.
