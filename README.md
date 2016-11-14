# Introduction
This image is especially built to be linked to this [Jenkins images](https://hub.docker.com/r/fjudith/jenkins)

# Quick start
First, run the Jenkins image as a deamon.

`docker run -it --rm --name='jenkins' -it --rm -p 8080:8080 -p 50000:50000 fjudith/jenkins`

Then run the Nginx image linked to the Jenkins with the link alias `jenkins-master`.

`docker run -d --name='jenkins-nginx' -it --rm -p 80:80 fjudith/jenkins-nginx`

# Reference

* https://engineering.riotgames.com/news/jenkins-docker-proxies-and-compose