### Run container
```
docker run nginx
```

### Run container by specific tag
```
docker run nginx:1.18.0-alpine
```

### Run container by default name
```
docker run -d --name web01 nginx
```

### Run container by map port with external
```
docker run -d --name web01 -p 80:80 nginx
```
### Remote and edit source in container
```
docker exec -it web01 bash
```
### Run container by map volumn
```
docker run -d --name web01 -p 80:80 -v C:\\labs\\html:/usr/share/nginx/html:ro nginx
```


### Extra Command
- update package and install vim for edit file in container
```
apt-get update && apt-get install -y vim
```
### Reference 
- https://hub.docker.com/_/nginx