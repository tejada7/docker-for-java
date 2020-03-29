# Chapter 1

### 1.1 Introduction to Docker

Slides only

### 1.2 Docker and Java

Slides only

### 1.3 Docker Workflow

Slides only

### 1.4 Getting Started with Docker

* Create Docker Machine: `docker-machine create -d virtualbox mymachine`
* Talk about `boot2docker.iso`
* Show `env | grep DOCKER`
* Setup machine: `eval $(docker-machine env mymachine)`
* Show `env | grep DOCKER`

Download command:
`docker container run jboss/wildfly` -> if not present the local, it will be pulled from docker hub
`docker container run -it jboss/wildfly` -> enables interactive mode 
`docker container run -d jboss/wildfly` -> detach mode (in background)
`docker container run --name my_custimized_container_name jboss/wildfly` -> assigns a custimized name
`docker container run -it jboss/wildfly bash` -> access to the container's shell

`docker container run -d --name web -P jboss/wildfly` -> runs the container in a random port
`docker container run -d --name web -p 8080:8080 jboss/wildfly` -> runs the container in an specific port