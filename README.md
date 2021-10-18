The Webservice has the ability to publish the following message "Wecome to Docker World - by Vamsi Copesetty"
This is published on the browser URL - http://localhost:8080/

Download image from https://hub.docker.com/repository/docker/vamsi2209/ift-510-project1

Hello World
===========

This is a simple Docker image that just gives "Wecome to Docker World - by Vamsi Copesetty" on port 8080. 

Pull my docker image using:
```bash
$ docker pull vamsi2209/ift-510-project1
Using default tag: latest
latest: Pulling from vamsi2209/ift-510-project1
Digest: sha256:9fbe5c4b8067394289b21dc05ab200064e12d2ceb65f7b510076612eefebcb55
Status: Image is up to date for vamsi2209/ift-510-project1:latest
docker.io/vamsi2209/ift-510-project1:latest
$ docker images | grep ift-510
REPOSITORY               TAG       IMAGE ID        CREATED          VIRTUAL SIZE
vamsi2209/ift-510-project1   latest    2c3e5bc3e447   35 minutes ago   126MB
```

OR

Build my Dockerfile using :
```bash
$ docker build -t vamsi-static-website .
$ docker images | grep vamsi
REPOSITORY               TAG       IMAGE ID        CREATED          VIRTUAL SIZE
vamsi-static-website   latest    2c3e5bc3e447   16 minutes ago   126MB
```



Sample usage
---------------------------

### Starting a web server on port 8080

```bash
$ docker run -it -d -p 8080:80 vamsi2209/ift-510-project1
```
