# Docker Tutorial

### docker build image
        docker build -t getting-started .

the -t flag tags our image. Think of this simply as a human-readable name for the final image. Since we named the image getting-started, we can refer to that image when we run a container.

The . at the end of the docker build command tells that Docker should look for the Dockerfile in the current directory.

### run docker in port
    docker run -dp 3000:3000 getting-started

-dp : is detacched mode (in background) and p is port mapping

## update source code
after update the source code
### build container
        docker build -t getting-started .
### try to run the container with command : 
        docker run -dp 3000:3000 getting-started

then replacing old container  with 
### command to get ID Container
        docker ps
Use the docker stop command to stop the container.
### Swap out <the-container-id> with the ID from docker ps
    docker stop <the-container-id>
### Once the container has stopped, you can remove it by using the docker rm command.
      docker rm <the-container-id>
### Now, start your updated app
        docker run -dp 3000:3000 getting-started
