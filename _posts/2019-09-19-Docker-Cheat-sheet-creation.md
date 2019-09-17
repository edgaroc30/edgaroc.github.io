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

### Example of Gitlab with Volume and Port mapping

```bash
--gitlab
sudo docker run --detach \
  --hostname odin.com \
  --publish 443:443 --publish 80:80 --publish 22:22 \
  --name gitlab \
  --restart always \
  --volume /srv/gitlab/config:/etc/gitlab \
  --volume /srv/gitlab/logs:/var/log/gitlab \
  --volume /srv/gitlab/data:/var/opt/gitlab \
  gitlab/gitlab-ce:latest
```
