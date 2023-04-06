# Build with Docker

This repository contains an example Go application, used in the
[Build with Docker guide](https://docs.docker.com/build/guide).

This goal of this guide is to illustrate Docker Build features and best
practices.

## In this repository

You'll find the Go source code for the application in the `cmd` directory. For
the purpose of the Build guide, there's no need to understand or interact with
the source code in any way. The guide only refers to Dockerfile changes.

The `Dockerfile` in the root directory of this project is the starting point for
this guide. It contains the unmodified version.

The `chapters` directory contains the finished Dockerfile examples for each
section of the guide. The sections are enumerated 1-8, and the Dockerfiles in
this directory are named after the section that they correspond to.

## Tasks

This repository implements [Task](https://taskfile.dev/) to make it easier to
switch between stages, or reset Dockerfile.

To reset your Dockerfile to a specific stage, install Task and run
`task goto:<stage>`. This overwrites the contents of the Dockerfile to the
**finished version** of the selected stage.

For example, running `task goto:1` resets the Dockerfile the starting point of
the guide. Running `task goto:4` resets the Dockerfile to reflect the **finished
version** of the 4th section of the guide.
