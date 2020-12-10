# Docker Commands

Check for running container
```
$ sudo docker ps
```
Check all container including stopped container
```
$ sudo docker ps -a
```
Build a docker image, -t allows you to specify Name and optionally a tag in the ‘name:tag’ format
```
$ sudo docker build -t yourName/ImageName:tag
```
Login to Docker Hub
```
$ sudo docker login
```
Push build image to Docker github
```
$ sudo docker push yourName/ImageName:tag
```
## Container
Go into the container
```
$ sudo docker exec -it containername bash
```
Go into the container as root user
```
$ docker exec -u root -it containername bash
```
Copy file from container to host
```
sudo docker cp containername:/file/path/in/container /file/path/in/host
```
Copy file from host to container
```
$ sudo docker cp /file/path/in/host containername:/file/path/in/container
```
Restart a container
```
$ sudo docker restart containername
```
Start a container
```
$ sudo docker start containername
```
Stop a container
```
$ sudo docker stop containername
```
Run a container, will grab the image specified and set it up. -d runs the container in the background.
```
$ sudo docker run -d --name name repository/ImageName:tag
```
Remove a container. -v remove volume associated with the container
```
$ sudo docker rm containername -v
```

## Volume
Remove a volume
```
$ sudo docker volume rm volume_name
```
List all volumes
```
$ sudo docker volume ls
```

## Network
Remove a network
```
$ sudo docker network rm network_name
```
List all networks
```
$ sudo docker network ls
```
Create a network
```
$ sudo docker network create network_name
```

## Image
List all images
```
$ sudo docker image ls
```
Remove image
```
$ sudo docker image rm imageName
```
Download an image
```
$ sudo docker image pull imageName
```
