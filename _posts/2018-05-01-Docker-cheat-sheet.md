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


#### Run a container detach and redirect localport to container port
```bash
docker run -p 80:80 --detach --name=my-container --env="SOME_ENV_VAR=value" container-name
```

#### Run a container and redirect localport to container port
```bash
docker run -p 80:80 --name=my-container --env="SOME_ENV_VAR=value" container-name
```

#### View container logs
```bash
docker logs my-container
```

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
