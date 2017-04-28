#This is a Dockerfile which includes normal users with normal privilledges.
FROM centos:latest

MAINTAINER yogeshgavhane596@gmail.com
RUN useradd -ms /bin/bash test

RUN echo "EXPORTS 10.0.0.0/24" >> /etc/exports.list
USER test

