# Build a nodejs app

Select user that docker is run as

```docker
USER <user>
```

Copy the file into the container and give permission to the user

```docker
COPY --chown=<user>:<group> <source> <destination>
```

Copy the file or download files from the network and if it is zip, it unzips it automatically

```docker
ADD --chown=<user>:<group> <source> <destination>
```

Change base directory

```docker
WORKDIR /the/workdir/path
```

run container in 3000 port

```
docker run --init --rm --publish 3000:3000 my-node-app
```
