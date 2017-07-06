# beam-dev

[![Docker Build Statu](https://img.shields.io/docker/build/zishanbilal/beam-dev.svg)](https://hub.docker.com/r/zishanbilal/beam-dev/)
[![Docker Automated buil](https://img.shields.io/docker/automated/zishanbilal/beam-dev.svg)](https://hub.docker.com/r/zishanbilal/beam-dev/)

Beam development environments.

## How to use this image

### Building a Gradle project

Run this from the directory of the Gradle project you want to build.

`docker run --rm -v "$PWD":/project -w /project --name beam-dev zishanbilal/beam-dev gradle <gradle-task>`

### Instructions for a new Gradle release

- Change ENV GRADLE_VERSION in all Dockerfiles to new version number.
