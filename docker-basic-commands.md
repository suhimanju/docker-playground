To pull a Docker image from the docker hub:

$ docker pull <image-name:tag>

To run that image, we can use the command:
$ docker run<image-name:tag> or $ docker run<image-id>

To list down all the images in our system, we can give command:
$ docker images ls

To list down all the running containers, we can use the command:
$ docker ps

To list down all the containers(even the ones not running) use the command below:
$ docker ps -a



Creating a Dockerfile:
Dockerfile contains instructions for building a Docker Image. Instructions contain various keywords.

FROM -> This keyword indicates the base image from which the container is built
RUN -> This key indicates the command that needs to be executed on the image

Command to Build an image:
$ docker build -t [image_name]:tag .
$ docker build -t demodocker:1.0 .

Command to Run the newly built image:
$ docker run --name "container-name" -p <host port>:<container port> <image_name:tag>
$ docker run --name "ubuntutomcat7" -p 8080:8080 edureka:1.0


## Start/Stop containers
List containers:
$ docker ps -a

To start the container, use the command:
$ docker start <container id>

To stop the container, use the command:
$ docker stop <container id>
