# Docker Swarm Traefik v2

![logo](logo.png)

Deploy Traefik v2 in Docker Swarm

## Prerequisites

Create a network for the swarm cluster

```bash
docker network create --driver=overlay --attachable --scope=swarm traefik
```

Set your domain for Traefik dashboard and metrics in `stack.yml`. The default value is http://traefik.localhost

## Install

```bash
docker stack deploy -c stack.yml Traefik
```

## Access

- Traefik dashboard : [http://traefik.localhost](http://traefik.localhost)
- Traefik prometheus metrics : [http://traefik.localhost/metrics](http://traefik.localhost/metrics)
