# running images

run command:
```
docker run imagename
```

run a bash shell:

```
docker run -it imagename /bin/bash
```

Expose ports:
```
docker run -p localport:container-port imagename
```

If the app in the container run on port 80, but you want to access it on port 8080 in your browser:
```
docker run -p 8080:80 imagename
```

# managing images and containers

List all pulled or built images:
```
docker images
```

Delete an image
```
docker rm -f imagename
```

List all running containers:
```
docker ps
```

Kill a contaienr:
```
docker kill container id
```
