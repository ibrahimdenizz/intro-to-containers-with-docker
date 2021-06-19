# More complicated nodejs app

node-alpine(80M) is smaller than node-stretch(900M)

Run command when docker file is built and add any changes to image

```docker
RUN <command>
```

Publish continer's port

```docker
EXPOSE 3000
```

Publish continer' port according to EXPOSE

```
docker run --init --rm --detacth -P <imagename>
```

dev.Dockerfile for devolopment 

build dev.Dockerfile

```
docker build -t my-node-app -f dev.Dockerfile .
```

