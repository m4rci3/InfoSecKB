# Manage Images / Docker Hub

```bash
#Login to Docker account
docker login -u {username}

#Publish an image to a repository (public/private)
docker push {image:tag}

#Delete an image
docker rmi {image:tag}

#Show a list of all images
docker images

#Search docker hub for images
docker search {image}

#Build an image from a Dockerfile
docker build -t {dockerfile path}
```

# Container Management

```bash
#See current running docker containers 
docker ps 

#See all (including shutdown) docker containers 
docker ps -a

#Delete a running container
docker rm {container-name or ID}

#Delete stopped containers 
docker container prune 

#Stop a running container 
docker stop {contiainer-name or ID}

#Start a stopped container 
docker start {container-name or ID}

#Copy a file from a container to the host
docker cp {target container:/path}

#Start a shell inside a running container
docker exec -it {container-name or ID}

#Rename a container
docker rename {old-name} {new-name}

#Pause a container
docker pause {container-name or ID}

#
```

# Run a new container

```bash
#Start a new container from an image
docker run {image}

#assign it a name 
docker run --name {name} {image}

#port mapping
docker run -p {hostport}:{containerport} {image}

#Start container in the background
docker run -d {image}

#Assign a hostname 
docker run --hostname {hostname} {image}

#Assign a specific docker network
docker run --network={network-name} {image}
```

# Docker Networking

```bash
#Creation of a user-defined network  with specified subnet, gateway and name
sudo docker network create -d {network-type e.g. bridge} {name} --subnet={subnet} --gateway={gateway}  

#Show all details of docker networks (and their connected containers)
docker inspect network {network name or type e.g driver}
```