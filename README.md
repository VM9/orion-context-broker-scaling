# Orion Context Broker Scaling
Repository for Orion Context Broker scaling laboratory and tests

Requiriments
- Docker
- Docker compose

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
