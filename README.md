# Personal Robotics Docker Images
This repository contains build information for generating various Docker images and Docker-Compose containers that package useful components of the software at the Personal Robotics lab.

----
#### Building images with Docker

Folders that contain a Dockerfile can be build into a Docker image:

```bash
$ docker build -t <image_name> .
```

----
#### Building containers with Docker-Compose

Folders that contain a docker-compose.yml can start a Docker-Compose container:

```bash
$ docker-compose up
```

[1]: http://docs.docker.com/
[2]: https://docs.docker.com/compose/
