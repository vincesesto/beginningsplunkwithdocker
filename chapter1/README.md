# Chapter 1 Summary of Commands

### Display the Version of Docker running on your system.
`docker --version`
 
### Run the basic hello-world Docker service.
`docker run hello-world`
 
    Search for a Docker image or type that you need from Docker Hub.
    docker search <image_name>
 
    Pull the latest stable version of your required image.
    docker pull <image_name>:latest
 
    Display all running Docker containers.
docker ps
 
    Display all running and stopped Docker containers.
docker ps -a
 
    Running Splunk as a Docker container with environment variables set.
docker run -d -e "SPLUNK_START_ARGS=--accept-license" -e "SPLUNK_USER=root" -p 8000:8000 splunk/splunk
 
    Show all relevant information for a Docker container.
docker inspect <container_id>
 
    View the logs of a Docker container.
docker logs <container_id>
 
    Show the history of a Docker image.
docker history <image_name>
 
    Access the shell of a running container.
docker attach <container_id>
 
    Perform the touch command on a running container using exec.
docker exec -d <container_id> touch /tmp/test.txt
 
Access the bash shell of a running container.
docker exec -it <container_id> /bin/bash

