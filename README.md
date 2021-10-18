The Webservice has the ability to publish the following message "Wecome to Docker World - by Vamsi Copesetty"
This is published on the browser URL - http://localhost:8080/

Hello World
===========

This is a simple Docker image that just gives "Wecome to Docker World - by Vamsi Copesetty" on port 8080. 

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
$ docker run -it -d -p 8080:80 vamsi-static-website
```
