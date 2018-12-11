# Docker available containers and images usage
![logo](https://cdn-images-1.medium.com/max/1600/0*m-xEibEV8ttbhv7W.png)

# Docker file
```
FROM ubuntu
RUN apt-get update -y
EXPOSE 6443
```
## docker container commit with id:+1:

```
CONTAINER ID        IMAGE                       COMMAND             CREATED             STATUS                     PORTS               NAMES
3b99d0ccd98d        b6fe2dd5a86d                "/bin/bash"         26 minutes ago      Up 26 minutes              6443/tcp            ks

docker commit 3b99d0ccd98d rajarani/ubntu_kubernetes:latest---------->3b99d0ccd98d(containerid):bat:
```

## docker images tag&push
```
REPOSITORY                  TAG                 IMAGE ID            CREATED             SIZE
rajarani/ubntu_kubernetes   latest              9bb582e4fdf6        12 minutes ago      714MB

docker tag 9bb582e4fdf6 rajarani/ubntu_kubernetes--------->9bb582e4fdf6(imageid):boy:
docker login
username
password
docker push rajarani/ubntu_kubernetes

```
