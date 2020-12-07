# Docker Image Packaging for Node.js

[![Travis](https://img.shields.io/travis/com/alvistack/docker-node.svg)](https://travis-ci.com/alvistack/docker-node)
[![GitHub release](https://img.shields.io/github/release/alvistack/docker-node.svg)](https://github.com/alvistack/docker-node/releases)
[![GitHub license](https://img.shields.io/github/license/alvistack/docker-node.svg)](https://github.com/alvistack/docker-node/blob/master/LICENSE)
[![Docker Pulls](https://img.shields.io/docker/pulls/alvistack/node.svg)](https://hub.docker.com/r/alvistack/node/)

Node.js is a software platform for scalable server-side and networking applications.

Learn more about Node.js: <https://nodejs.org/>

## Supported Tags and Respective Packer Template Links

  - [`15`, `latest`](https://github.com/alvistack/docker-node/blob/master/packer/docker-15/packer.json)
  - [`14`](https://github.com/alvistack/docker-node/blob/master/packer/docker-14/packer.json)
  - [`12`](https://github.com/alvistack/docker-node/blob/master/packer/docker-12/packer.json)

## Overview

This Docker container makes it easy to get an instance of Node.js up and running.

Based on [Official Ubuntu Docker Image](https://hub.docker.com/_/ubuntu/) with some minor hack:

  - Packaging by Packer Docker builder and Ansible provisioner in single layer
  - Handle `ENTRYPOINT` with [catatonit](https://github.com/openSUSE/catatonit)

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

### `alvistack/node:latest`

The `latest` tag matches the most recent [GitHub Release](https://github.com/alvistack/docker-node/releases) of this repository. Thus using `alvistack/node:latest` or `alvistack/node` will ensure you are running the most up to date stable version of this image.

### `alvistack/node:<version>`

The version tags are rolling release rebuild by [Travis](https://travis-ci.com/alvistack/docker-node) in weekly basis. Thus using these tags will ensure you are running the latest packages provided by the base image project.

## License

  - Code released under [Apache License 2.0](LICENSE)
  - Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

## Author Information

  - Wong Hoi Sing Edison
      - <https://twitter.com/hswong3i>
      - <https://github.com/hswong3i>
