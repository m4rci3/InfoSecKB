# Docker Hub

```bash
#Login into Docker
docker login -u {username}

#Publish an image to Docker Hub
docker push {username}/{image name}

#Search Hub for an image 
docker search {image name}

#Pull an image from Docker Hub
docker pull {e.g.ngnix} {version e.g. 1.23}
```

# Image Commands

```bash
#Build an image from a Dockerfile(image)
docker built -t {image name}

#List all docker images (Repo, TAG, Image ID, Creation date, Size)
docker images

#Delete an image
docker rmi {image name}

```

# Interact with containers

```bash
#Run the docker container in the foreground
docker run {name}:{tag} 

#Run the docker container interactivley (command line)
docker run -it {name}:{tag}

#Run docker container in the background/ detatched
docker run -d {name}:{tag}

#Stop a docker container
docker stop {docker name or container name}

#Show running Docker containers 
docker ps 

#Show stopped Docker containers
docker ps -a 

#Open a shell inside an already running container
docker exec -it {container name} sh

#Run a container with and publish a container's ports to the host
docker run -p {host port}:{container port} {image name}
```
