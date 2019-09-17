## Creation

#### Port mapping

```bash
--publish, -p host:container
```

#### Volume mapping

```bash
--volume, -v /path/in/host:/path/in/docker
```

#### Limit memory

```bash
--memory= '4096MB'
-m= '4GB'
```

## Runtime

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
```
