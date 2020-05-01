# Cloud9

## Build

```bash
$ docker build \
  --no-cache \
  --pull \
  -t denhamparry/cloud9:latest .
```

### ARM

```bash
$ docker run --rm --privileged multiarch/qemu-user-static:register --reset
$ docker build \
  --no-cache \
  --pull \
  -f Dockerfile.armhf
  -t denhamparry/cloud9:latest .
```

## Basics

### Run

```bash
$ docker run -it -d \
  --name=cloud9 \
  -e PUID=1000 \
  -e PGID=1000 \
  -e TZ=Europe/London \
  -p 8000:8000 \
  --restart unless-stopped \
  denhamparry/cloud9
```

### Delete

```bash
$ docker stop cloud9 &&\
    docker rm cloud9
```

## References

- [Linux Server Cloud 9](https://github.com/linuxserver/docker-cloud9)
