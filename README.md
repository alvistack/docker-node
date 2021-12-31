# Docker Image Packaging for Node.js

<img src="/alvistack.svg" width="75" alt="AlviStack">

[![GitLab pipeline status](https://img.shields.io/gitlab/pipeline/alvistack/docker-node/master)](https://gitlab.com/alvistack/docker-node/-/pipelines)
[![GitHub tag](https://img.shields.io/github/tag/alvistack/docker-node.svg)](https://github.com/alvistack/docker-node/tags)
[![GitHub license](https://img.shields.io/github/license/alvistack/docker-node.svg)](https://github.com/alvistack/docker-node/blob/master/LICENSE)
[![Docker Pulls](https://img.shields.io/docker/pulls/alvistack/node-17.svg)](https://hub.docker.com/r/alvistack/node-17)

Node.js is a software platform for scalable server-side and networking applications.

Learn more about Node.js: <https://nodejs.org/>

## Supported Tags and Respective Packer Template Links

  - [`alvistack/node-17`](https://hub.docker.com/r/alvistack/node-17)
      - [`packer/docker-17/packer.json`](https://github.com/alvistack/docker-node/blob/master/packer/docker-17/packer.json)
  - [`alvistack/node-16`](https://hub.docker.com/r/alvistack/node-16)
      - [`packer/docker-16/packer.json`](https://github.com/alvistack/docker-node/blob/master/packer/docker-16/packer.json)
  - [`alvistack/node-14`](https://hub.docker.com/r/alvistack/node-14)
      - [`packer/docker-14/packer.json`](https://github.com/alvistack/docker-node/blob/master/packer/docker-14/packer.json)

## Overview

This Docker container makes it easy to get an instance of Node.js up and running.

Based on [Official Ubuntu Docker Image](https://hub.docker.com/_/ubuntu/) with some minor hack:

  - Packaging by Packer Docker builder and Ansible provisioner in single layer
  - Handle `ENTRYPOINT` with [catatonit](https://github.com/openSUSE/catatonit)

### Quick Start

For the `VOLUME` directory that is used to store the repository data (amongst other things) we recommend mounting a host directory as a [data volume](https://docs.docker.com/engine/tutorials/dockervolumes/#/data-volumes), or via a named volume if using a docker version \>= 1.9.

Start Node.js:

    # Pull latest image
    docker pull alvistack/node-17
    
    # Run as detach
    docker run \
        -itd \
        --rm \
        --name node \
        alvistack/node-17 \
        node --version

## Versioning

### `YYYYMMDD.Y.Z`

Release tags could be find from [GitHub Release](https://github.com/alvistack/docker-node/tags) of this repository. Thus using these tags will ensure you are running the most up to date stable version of this image.

### `YYYYMMDD.0.0`

Version tags ended with `.0.0` are rolling release rebuild by [GitLab pipeline](https://gitlab.com/alvistack/docker-node/-/pipelines) in weekly basis. Thus using these tags will ensure you are running the latest packages provided by the base image project.

## License

  - Code released under [Apache License 2.0](LICENSE)
  - Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

## Author Information

  - Wong Hoi Sing Edison
      - <https://twitter.com/hswong3i>
      - <https://github.com/hswong3i>
