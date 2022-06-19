# docker-scratch-curl [![Release Github Packages](https://github.com/antyung88/docker-scratch-curl/actions/workflows/release.yml/badge.svg)](https://github.com/antyung88/docker-scratch-curl/actions/workflows/release.yml)
Scratch Base with CURL

```
REPOSITORY                       TAG       IMAGE ID       CREATED          SIZE
ghcr.io/antyung88/scratch-curl   latest    4182919fd0c5   10 minutes ago   3.04MB
```

# Usage
```
docker run ghcr.io/antyung88/scratch-curl:latest curl 127.0.0.1
```


# To enable curl in Scratch Image
```
FROM scratch
ENV PATH="/bin:${PATH}"
COPY --from=ghcr.io/antyung88/scratch-curl:stable /bin /bin
```
