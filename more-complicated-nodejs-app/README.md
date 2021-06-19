# More complicated nodejs app

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