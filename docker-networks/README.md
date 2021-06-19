# Docker Networks

docker network command

```
docker network ls
docker network rm <network-id>
docker network create --driver=<driver-name> <network -name>
```

commands for this example. It connect two mongodb with each other
```
docker run -d --network=app-net -p 27017:27017 --name=db --rm mongo:3 

 docker run -it --network=app-net --rm mongo:3 mongo --host db
```