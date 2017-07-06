# beam-dev

[![Docker Build Statu](https://img.shields.io/docker/build/zishanbilal/beam-dev.svg)](https://hub.docker.com/r/zishanbilal/beam-dev/)
[![Docker Automated buil](https://img.shields.io/docker/automated/zishanbilal/beam-dev.svg)](https://hub.docker.com/r/zishanbilal/beam-dev/)

Development environment for the BEAM modeling framework.

## How to use this image

### Building a Gradle project

Run this from the directory of the Beam project you want to build.

`docker run --rm -v "$PWD":/home/dev --name beam-dev zishanbilal/beam-dev gradle <gradle-task>`
