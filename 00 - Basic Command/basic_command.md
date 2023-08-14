# Docker Basic Command
### check docker information running on your computer
```
docker info
```

### check docker version on your computer
```
docker --version
```

### list docker images on your computer
```
docker images
docker images -a
```

### remove docker images on your computer
```
docker rmi <images id/name>
```


### list docker container on your computer
```
docker ps
docker ps -a
```

### remove docker container on your computer
```
docker rm <container id/name>
```

### run docker container on your computer
- attach mode
```
docker run <images id/name>
```

- detach mode
```
docker run -d <images id/name>
```
- attach back
```
docker attach <container id/name>
```

### start docker container on your computer
```
docker start <images id/name>
```

### stop docker container on your computer
```
docker stop <images id/name>
```

### pull docker image from docker registry to your computer
```
docker pull <images name on docker registry>
```

### execute command on docker container
- execute command in container
```
docker exec <container id/name> <command> <option>
```
ex. docker exec cranky_lewin cat /etc/hosts
- remote container
```
docker exec -it <container id/name> <command>
```
ex. docker exec -it cranky_lewin sh