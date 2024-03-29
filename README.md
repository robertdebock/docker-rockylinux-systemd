Docker Rocky Linux Systemd
==========================

This Dockerfile can build containers capable to use systemd.

[![rockylinux build status](https://img.shields.io/docker/cloud/build/robertdebock/rockylinux.svg)](https://hub.docker.com/repository/docker/robertdebock/rockylinux)

Branches
--------

This repository has multiple branches that relate to RockyLinux versions.

|Branch |Rocky Linux Version|Docker image tag|
|-------|-------------------|----------------|
|7      |7                  |7               |
|8      |8                  |8               |
|master |9                  |latest          |

Pull strategy
-------------

The different branches are **not** merged, they live as individual branches.

Manually starting
-----------------

```
docker run \
  --tty \
  --privileged \
  --volume /sys/fs/cgroup:/sys/fs/cgroup:ro \
  robertdebock/rockylinux
```
