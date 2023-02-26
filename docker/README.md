# Docker

## Getting started

Docker is an OS virtualized software platform that allows to quickly create, deploy, and run applications in Docker containers, which have all the dependencies within them. The Docker container can be moved from environment to environment very easily.

## Topics
- [Container]()
- [Dockerfile]()
- [Compose]()
- [Swarm]()
- [Commands]()
- [Networking]()

## Docker Interview Questions and Answers

### What is Docker?
Docker is an open-source containerization platform. It is used to automate the deployment of any application, using lightweight, portable containers.

### What are Docker’s most notable features?
Docker is an open-source containerization platform. It is used to automate the deployment of any application, using lightweight, portable containers.

### Explain virtualization?
Virtualization is the means of employing software (such as Hypervisor) to create a virtual version of a resource such as a server, data storage, or application. Virtualization lets you divide a system into a series of separate sections, each one acting as a distinct individual system. The virtual environment is called a virtual machine.

## Docker Commands
Build an image from the Dockerfile in the current directory and tag the image
```bash
docker build -t your_image_name
```
List all Docker images
```bash
docker images
```
Delete an image from the docker image
```bash
docker image rm alpine:3.4
```
Create a container
```bash
docker create [IMAGE] 
```
Run a command in a new container
```bash
docker run [IMAGE] [COMMAND] 
```
Rename an existing container
```bash
docker rename [CONTAINER_NAME] [NEW_CONTAINER_NAME]
```
Removes all the stopped containers
```bash
docker container prune [OPTIONS] 
```
Create a new image from a container’s file changes
```bash
docker container commit [OPTIONS] CONTAINER [REPOSITORY[:TAG]]
```
Remove an existing container
```bash
docker rm [CONTAINER] 
```
List the running containers
```bash
docker container ls
```
Stop a running container
```bash
docker stop [CONTAINER_NAME]
```
Restart a running container
```bash
docker restart [CONTAINER]
```
Kill the running containers
```bash
docker Kill [CONTAINER]
```
Attach local standard input, output, and error streams to a running container
```bash
docker attach  [CONTAINER]
```
Block a container 
```bash
docker wait  [CONTAINER]
```
Pull an image from a registry
```bash
docker pull [OPTIONS] NAME[:TAG] 
```
Push an image to a registry 
```bash
docker push [OPTIONS] NAME[:TAG] 
```
Run a command in a running container
```bash
docker exec [OPTIONS] CONTAINER COMMAND [ARG...] 
```
Login into docker hub
```bash
docker login
```
Get information on the Docker tool
```bash
docker info
```
Display the history of an image with the image name mentioned in the command
```bash
docker history httpd 
```
Create a volume for containers
```bash
docker volume create
```
Create a Docker Swarm
```bash
docker swarm init --advertise-addr [IP ADDRESS] 
```
Joins nodes in the swarm
```bash
docker swarm join --advertise-addr HOST:PORT 
```
Execute this command to leave docker swarm
```bash
docker swarm leave [OPTIONS]
```
Display docker-compose version
```bash
docker-compose -version 
```
Creating your first Docker-Compose File
```bash
vi docker-compose.yml
```
Run our Docker Compose file
```bash
docker-compose up 
```