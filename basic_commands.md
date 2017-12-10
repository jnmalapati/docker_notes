# docker_notes

#Docker

Images ~ Stopped containers
Containers ~ Running images


Docker pull <<image>>:version
For e.g., 
 Docker pull ubuntu:14.04

To pull images to locally

Docker rmi <<image>>:version/tag
To remove images


# Container lifecycle :
Docker contains can be started, stoped and removed

Docker start <container>
Docker stop <container>
Docker rm <container>

Docker run -d —name web -p 80:8080 <imageToUse>

-d : detach mode (running in background)
-name: name
-p : network port, web server listening on port 8080, map port 80 on docker host, to 8080 in a container

Docker run -it —name temp ubuntu:latest /bin/bash

# Removing

Docker stop $(docker ps -aq)
   ~ stops all the containers ( a - all containers, q - quite)
Returns all id’s of the containers stopped…

Docker rm $(docker ps -aq)
Removes all containers

# Images

Docker rmi $(docker images -q)
~ removes all the images


# attach a interactive

Docker run -d/ -it <image>
  -d: detached
  -it: interactive

Docker ps - list of running containers








