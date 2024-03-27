# java devcontainer [![Docker](https://img.shields.io/docker/v/jeffersonlab/java-devcontainer?sort=semver&label=DockerHub)](https://hub.docker.com/r/jeffersonlab/java-devcontainer)
A Java [devcontainer](https://containers.dev/).

## Overview
The 1.x version series is intended to use the following:
- Java 17
- Gradle 7.4
- Ubuntu "jammy"

## Build / Release
Make changes to the Dockerfile, test them, then bump the version in the VERSION file and commit it.  The CD GitHub Action should take care of the rest.