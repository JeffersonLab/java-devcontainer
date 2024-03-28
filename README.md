# java devcontainer [![Docker](https://img.shields.io/docker/v/jeffersonlab/java-devcontainer?sort=semver&label=DockerHub)](https://hub.docker.com/r/jeffersonlab/java-devcontainer)
A Java [devcontainer](https://containers.dev/).

## Overview
The 1.x version series is intended to use the following:
- Java 17
- Gradle 7.4
- Ubuntu "jammy"
- [Docker outside of Docker](https://github.com/devcontainers/features/tree/main/src/docker-outside-of-docker) (sibling container).   Use a bind mount of the form `/var/run/docker.sock:/var/run/docker.sock`. We don't use [Docker in  Docker]([https://jpetazzo.github.io/2015/09/03/do-not-use-docker-in-docker-for-ci/](https://github.com/devcontainers/features/tree/main/src/docker-in-docker)), because it appears to be the [less good option](https://jpetazzo.github.io/2015/09/03/do-not-use-docker-in-docker-for-ci/).

## Build / Release
Make changes to the Dockerfile, test them, then bump the version in the VERSION file and commit it.  The CD GitHub Action should take care of the rest.
