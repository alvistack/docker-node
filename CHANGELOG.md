# Docker Image Packaging for Node.js

## 13.8.0-XalvistackY - TBC

### Major Changes

  - Consolidate molecule tests into `default` (noop)

## 13.8.0-4alvistack3 - 2020-03-04

### Major Changes

  - Revamp with Molecule and `docker commit`
  - Hotfix for systemd

## 13.6.0-3alvistack1 - 2020-01-15

### Major Changes

  - Replace `dumb-init` with `tini`, as like as `docker --init`
  - Include release specific vars and tasks

## 13.6.0-2alvistack1 - 2020-01-14

  - Ubuntu 18.04 based
  - Handle ENTRYPOINT with dumb-init
  - Self initialize with Ansible, by dogfooding with Ansible Playbook
