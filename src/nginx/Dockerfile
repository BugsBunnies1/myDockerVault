# Creating a basic Dockefile for Nginx

FROM ubuntu

MAINTAINER BugsBunnies1

RUN apt-get update && apt-get install -y nginx

ADD index.html /usr/share/nginx/html/index.html

ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]

EXPOSE 82
