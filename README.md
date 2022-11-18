# CS263-Project

Team Members:
Zeyu Wang, Jing Peng

## Week 1
- prepare JVM related files
- learn to write benchmarks

## Week 2
- find test games in java

## Week 3
- build docker of GraalVM, azul, HotSpot, OpenJ9

## Week 4
- deploy application in docker
- learn to use time in java to record execution time


## creating JAR from .java -- InteliJ


## docker start guide
- docker create container with specific image
```
docker container create -i -t --name MY_CONTAINER_NAME IMAGE_NAME
```

- copy jar to container
```
$ docker cp filepath/xxx.jar container_id:/xxx.jar
```
- enter container
```
$ docker exec -it jre11-hotspot bash 
```
- runtime check
```
$ time java -jar xxx.jar
```

