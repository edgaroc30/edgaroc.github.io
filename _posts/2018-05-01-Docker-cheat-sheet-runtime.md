This is my own Docker cheat sheet. 

#### List all the containers 
```bash
docker ps 
```

#### Delete a container
```bash
docker rm my-container
```

#### Stop a container
```bash
docker stop my-container
```

#### ssh into the container

```bash
sudo docker exec -it NameOfContainer /bin/bash
```

#### Tail logs

```bash
sudo docker logs -f gitlab
```

#### Copy stuff from the container to host

```bash
docker cp CONTAINER:/container/path/to /local/host/path
```

#### Docker statust - RAM, CPU, Network usage

```bash
docker stats [optionalContainer]

#### Inspect container
```bash
docker inspect my-container
```

#### List all the availalbe images
```bash
docker images
```

#### Restart container
```bash
docker restart my-container
```

#### Stop all running containers
```bash
docker stop $(docker ps -aq)
```

#### Remove all containers
```bash
docker rm $(docker ps -aq)
```

#### Remove all images
```bash
docker rmi $(docker images -q)
```

#### Prune system
```bash
docker system prune -a
```
