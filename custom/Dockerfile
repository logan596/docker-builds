#This Dockerfile contains OpenSSH Server and Apache Server.

FROM centos:6 
MAINTAINER yogeshgavhane596@gmail.com
RUN yum update -y
RUN yum install -y openssh-server
RUN yum install -y httpd
EXPOSE 22
EXPOSE 80
RUN echo "Hello this is image build file for the container Exporting it from Jenkins Server" > /var/www/html/index.html
ENTRYPOINT apachectl "-DFOREGROUND"

