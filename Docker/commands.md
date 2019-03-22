# Docker Commands

## Basic Run
Runs a basic container 


`docker run ubuntu`

## List Containers

##### List all running containers

`docker ps`

##### List all containers 

`docker ps -a`

## Stop Containers

##### Stop one container

`docker stop containerName`

or 

`docker stop contianerId`

##### Stop all containers

'docker stop $(docker ps -q)'


