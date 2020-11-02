# Docker Image Packaging for Node.js

## 15.0.1-XalvistackY - TBC

### Major Changes

  - Revamp with Packer

## 14.13.1-4alvistack1 - 2020-10-14

### Major Changes

  - Refine Molecule matrix

## 14.8.0-4alvistack2 - 2020-08-26

### Major Changes

  - Upgrade minimal Ansible Lint support to 4.3.2
  - Upgrade Travis CI test as Ubuntu Focal based
  - Upgrade minimal Ansible support to 2.10.0

## 14.4.0-4alvistack2 - 2020-06-10

### Major Changes

  - Add Node.js 14 support
  - Remove Node.js 13 support
  - Revamp `create`, `side_effect`, `verify` and `destroy` logic
  - Replace `tini` with `catatonit`
  - Rename `post_tasks.yml` as `side_effect.yml`

## 13.8.0-4alvistack4 - 2020-03-05

### Major Changes

  - Revamp with Molecule and `docker commit`
  - Consolidate molecule tests into `default` (noop)
  - Hotfix for systemd

## 13.6.0-3alvistack1 - 2020-01-15

### Major Changes

  - Replace `dumb-init` with `tini`, as like as `docker --init`
  - Include release specific vars and tasks

## 13.6.0-2alvistack1 - 2020-01-14

  - Ubuntu 18.04 based
  - Handle ENTRYPOINT with dumb-init
  - Self initialize with Ansible, by dogfooding with Ansible Playbook
