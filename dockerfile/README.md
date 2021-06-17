# Dockerfile

Select image for container

```docker
FROM <image-name>
```
Run command when docker container start

```docker
CMD ["command", "parameter"]
```

build Dockerfile located in current directory

```
docker build .
```

build Dockerfile with a tag

```
docker build --tag <name>:<version|default=lastest> .
```

run docker image

```
docker run <name>:<version|default=latest>
```
