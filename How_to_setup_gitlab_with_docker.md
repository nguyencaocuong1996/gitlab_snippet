[Reference link](https://docs.gitlab.com/omnibus/docker/)
# Run gitlab docker container
```docker
    docker run --detach \
    --hostname 0.0.0.0 \
    --publish 9080:80 --publish 9022:22 \
    --name gitlab11 \
    --restart=always \
    --volume /gitlab11/config:/etc/gitlab \
    --volume /gitlab11/logs:/var/log/gitlab \
    --volume /gitlab11/data:/var/opt/gitlab \
    gitlab/gitlab-ce:latest
```


# Run gitlab docker container
```docker
    docker run --detach \
    --hostname 0.0.0.0 \
    --publish 180:80 --publish 122:22 \
    --name gitlab11 \
    --restart=always \
    --volume /docker/volume/gitlab/config:/etc/gitlab \
    --volume /docker/volume/gitlab/logs:/var/log/gitlab \
    --volume /docker/volume/gitlab/data:/var/opt/gitlab \
    gitlab/gitlab-ce:latest
```
