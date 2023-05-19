# Docker Image (Udemy | Stephane Mareek)

## Introduction

- A Docker image is a read-only template that contains a set of instructions for creating a container that can run on the Docker platform. It provides a convenient way to package up applications and preconfigured server environments, which you can use for your own private use or share publicly with other Docker users

## Cloud Research

### Where Docker images are stored?

- Docker images are stored in Docker Repositories
  > - Public: Docker Hub https://hub.docker.com/
  >   <br>• Find base images for many technologies or OS:
  >   <br>• Ubuntu
  >   <br>• MySQL
  >   <br>• NodeJS, Java…
- Private: Amazon ECR (Elastic Container Registry)

### Docker versus Virtual Machines

- Docker is ”sort of” a virtualization technology, but not exactly
- Resources are shared with the host => many containers on one server

## Next Steps

- Amazon • ECS
