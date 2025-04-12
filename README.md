# Docker Commands

### To see container logs & inspect container
```
docker logs < containerName>

docker inspect < containerName>
``` 
# Docker Images
```
# To list docker images
docker images / docker image ls

# To remove images
docker rmi < imgName>

# To Rename docker image
docker image tag < imgName>

# To get the id's of all images
docker images -aq

# To remove all docker images
docker rmi -f $(docker images -aq)
```

### To pull the docker image from DockerHub
 ```
 docker pull < imageName >
 ```

### To check the status of container
 ```
    docker ps    ... for running containers
   
    docker ps -a  ... for all containers
```

### To run stop and start the docker container
```
1. docker run < imageName>

2. docker start < imgName >

3. docker stop < imgName >

Flags
-d = To run container in detached mode
-p 8000:8000 = Port Binding
-e = To Pass ENV Variables
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

# Docker Network

### To list the all available networks
```
docker network ls
```

### To create docker network
```
docker network create mynet -d Bridge   

-d = driver
```

### To inspect the docker network
```
 docker network inspect < networkName>
```

# Docker Volumes and Storage

```
# To list docker volumes
docker volume ls

# To create docker volume
docker volume create < volName>

# To see more details
docker volume inspect < volName>
```

# Docker Compose

```
# To run docker containers
docker compose up

# To build docker containers
docker compose up --build

# To down docker containers
docker compose down

-d = for detached mode

# To Remove all unused volumes, images, networks, containers
docker system prune
```

# DockerHub

```
# To login 
docker login

# To push docker image
docker push < imgName>
```

# Docker Scout
```
# To check vulnerabilities
docker scout quickview < imgName>

# To scan common vulnerabilities
docker scout cves < imgName>
```

# Docker init
```
docker init
```