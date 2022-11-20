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
- copy jar/java file to container
```
$ docker cp filepath/xxx container_id:/filepath/xxx
```
- start container 
```
$ docker start container_id
```
- enter container
```
$ docker exec -it jre11-hotspot bash 
```
- runtime check
```
$ time java -jar xxx.jar
$ time java xxx.java
```
- GC check
```
//for hotspot
java -verbose:gc -Xms10M -Xmx10m -XX:-PrintGCDetails Main.java
//if convert Main.java to Main, then it will not print GC while compile .java to .class
```
