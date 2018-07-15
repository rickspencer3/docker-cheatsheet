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

Then navigate in the browser to that port (localhost:8080). Or, if you are running docker toolbox, that means that docker is running in a VM, so it will have is own ip address. You can find the local address with this command:
```
docker-machine ip default
```

If that doesn't work, you can [find the name of the docker-machine](https://github.com/prakhar1989/docker-curriculum/issues/27).


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
