#This is a Dockerfile which create httpd server.

FROM centos:latest
MAINTAINER yogeshgavhane596@gmail.com
RUN yum update -y
RUN yum install -y httpd net-tools
RUN echo "Hi this is a custom index file httpd" > /var/www/html/index.html
ENTRYPOINT apachectl "-DFOREGROUND"
#EXPOSE 80
