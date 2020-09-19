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

---

## Support

[![ko-fi](https://www.ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/D1D1WGU9)

<div><a href="https://payping.ir/@hatamiarash7"><img src="https://cdn.payping.ir/statics/Payping-logo/Trust/blue.svg" height="128" width="128"></a></div>

## Contributing

1. Fork it !
2. Create your feature branch : `git checkout -b my-new-feature`
3. Commit your changes : `git commit -am 'Add some feature'`
4. Push to the branch : `git push origin my-new-feature`
5. Submit a pull request :D

## Issues

Each project may have many problems. Contributing to the better development of this project by reporting them.
