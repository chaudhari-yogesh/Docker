# Docker Commands

#### To list the docker images
```
docker images
     OR
docker image ls
```

### To pull the docker image from DockerHub
 ```
 docker pull < imageName >
 ```

### To check the status of container
 ```
    docker ps     for running containers
   
    docker ps -a  for all containers
```

### To run stop and start the docker container
```
1. docker run < imageName>

2. docker start < imgName >

3. docker stop < imgName >

Flags
-d = To run container in detached mode
-p 8000:8000 = Port Binding
--name = Assigned name to docker container
```

### To build the docker images from docker file
```
docker build -t < imgName > .
```

### To run docker container in interactive mode
```
docker exec -it < containerName> bash 
```