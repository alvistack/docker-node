# Docker Image Packaging for Node.js

[![Travis](https://img.shields.io/travis/alvistack/docker-node.svg)](https://travis-ci.org/alvistack/docker-node)
[![GitHub release](https://img.shields.io/github/release/alvistack/docker-node.svg)](https://github.com/alvistack/docker-node/releases)
[![GitHub license](https://img.shields.io/github/license/alvistack/docker-node.svg)](https://github.com/alvistack/docker-node/blob/master/LICENSE)
[![Docker Pulls](https://img.shields.io/docker/pulls/alvistack/node.svg)](https://hub.docker.com/r/alvistack/node/)

Node.js is a software platform for scalable server-side and networking applications.

Learn more about Node.js: <https://nodejs.org/>

## Supported Tags and Respective `Dockerfile` Links

  - [`latest` (master/Dockerfile)](https://github.com/alvistack/docker-node/blob/master/Dockerfile)
  - [`13` (13/Dockerfile)](https://github.com/alvistack/docker-node/blob/13/Dockerfile)
  - [`12` (12/Dockerfile)](https://github.com/alvistack/docker-node/blob/12/Dockerfile)
  - [`10` (10/Dockerfile)](https://github.com/alvistack/docker-node/blob/10/Dockerfile)

## Overview

This Docker container makes it easy to get an instance of Node.js up and running.

### Quick Start

For the `VOLUME` directory that is used to store the repository data (amongst other things) we recommend mounting a host directory as a [data volume](https://docs.docker.com/engine/tutorials/dockervolumes/#/data-volumes), or via a named volume if using a docker version \>= 1.9.

Start Node.js:

    # Pull latest image
    docker pull alvistack/node
    
    # Run as detach
    docker run \
        -itd \
        --rm \
        --name node \
        alvistack/node \
        node --version

## Versioning

The `latest` tag matches the most recent version of this repository. Thus using `alvistack/node:latest` or `alvistack/node` will ensure you are running the most up to date version of this image.

## License

  - Code released under [Apache License 2.0](LICENSE)
  - Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

## Author Information

  - Wong Hoi Sing Edison
      - <https://twitter.com/hswong3i>
      - <https://github.com/hswong3i>
