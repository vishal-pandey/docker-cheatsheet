## Docker Cheatsheet

![Docker Lifecycle](https://raw.githubusercontent.com/vishal-pandey/docker-cheatsheet/main/img/docker-lifecycle.jpg "Docker Lifecycle")

- `docker images` - list of Docker images on the system

- `docker run image ` - download image if not present and run image as container.

- `docker run –it ubuntu bash` -  `-it` optoin tells docker to run command in interactive mode.

- `docker run -p 80:8080/tcp ubuntu bash` - 80 hostport, 8080 container port

- `docker rmi ImageID` - remove docker image with ImageId

- `docker ps` - list currently running containers on the machine

- `docker ps -a` - list all the containers on the machine

- `docker history ImageId` - see all the commands that were run with an image via a container

- `docker top ContainerID` - see the top processes within a container

- `docker stop ContainerID` - stop a running container

- `docker rm ContainerID` - delete a container

- `docker stats ContainerID` - statstics of a running container

- `docker inspect Container/Image` - return low-level information on the container or image

- `docker logs containerID` - to see the logs of the container

- `docker attach ContainerID` - attach a running container

- `docker pause ContainerID` - pause the processes in a running container

- `docker unpause ContainerID` - unpause the processes in a running container

- `docker kill ContainerID` - kill the processes in a running container

![Container Lifecycle](https://raw.githubusercontent.com/vishal-pandey/docker-cheatsheet/main/img/container_lifecycle.jpg "Container Lifecycle")


### Dockerfile

Dockerfile is used to create images which in turn can be used to create containers.

- `#` - for comments

- `FROM` - tells docker, from which base image you want to base your image from

- `RUN` - run instructions against the image

- `CMD command param1` - execute a command at runtime when the container is executed 

- `ENV key value` - set environment variables in the container

- `WORKDIR dirname` - set the working directory of the container

- `docker build  -t ImageName:TagName dir` - Build image from dockerfile, -t for tagging, dir for location of Dockerfile

### DockerCompose

Docker Compose is used to run multiple containers as a single service without the need to start each one separately.

- `docker-compose.yml` - filename for docker compose

- `docker-compose version` - details of the version of docker compose














