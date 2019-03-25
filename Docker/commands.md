# Docker Commands

## Pull and Run

Pulls an image 

`docker pull ubuntu`

Runs a basic container and downloads it if it isn't available

`docker run ubuntu`

Run in detached mode 

`docker run -d ubuntu`

Map ports, in this case map host port 80 to client port 5000

`docker run -p 80:5000 <containerName>`

Map column outside of container

`docker run -v /Documents/things:/var/things <containerName>`

## Build Image

##### Build Image from Dockerfile

`docker build Dockerfile -t <imageName>`

##### Push Image to Registry

`docker push <imageName>`

## List Containers

##### List All Running Containers

`docker ps`

##### List All Containers 

`docker ps -a`

## Stop and Remove Containers

##### Stop One Container

`docker stop <containerName>`

or 

`docker stop <containerId>`

##### Stop All Containers

`docker stop $(docker ps -q)`

##### Stop Some Containers

You only need to type the first few characters of a container id

`docker stop 345 efc 6da`

##### Remove Containers

`docker rm <containerName>`

## Images

##### List Images

`docker images`

##### Remove images

`docker rmi images`

## Container Commands and Access

##### Run Command

Displays contents of host file

`docker exec <containerName> cat etc/hosts`

Run bash in container. Super useful!

`docker exec -it <containerName> /bin/bash`


