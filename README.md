# Base Docker Image

* [debian:jessie-slim](https://hub.docker.com/r/_/debian/)


# Installation

* Install [Docker](https://www.docker.com/)

* Get automated build from public registry:

Latest version:

`docker pull bperel/pac:latest`

* [Alternatively] Build an image from Dockerfile: `docker build -t="dresantos/pac" github.com/bperel/pac-docker`

# Usage


Running PAC in X11

```
xhost +
docker run -it -e DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix --rm bperel/pac pac
```
