#This is a Dockerfile which includes normal users with normal privilledges.
FROM centos:latest

MAINTAINER yogeshgavhane596@gmail.com
RUN useradd -ms /bin/bash test

RUN echo "EXPORTS 10.0.0.0/24" >> /etc/exports.list
RUN yum update -y
RUN yum install wget -y
RUN cd ~

RUN wget http://dl.fedoraproject.org/pub/epel/7/x86_64/e/epel-release-7-9.noarch.rpm
RUN rpm -ivh epel-release-7-9.noarch.rpm
RUN yum update -y 
RUN yum install java-1.7.0-openjdk -y 
USER test
RUN cd ~ && echo "export JAVA_HOME=/usr/java/jdk1.7.0/jre" >> /home/test/.bashrc
ENV JAVA_BIN /usr/java/jdk1.7.0/jre

