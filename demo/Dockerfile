FROM centos:latest

RUN mkdir /app
ADD ./target /app
WORKDIR /app

RUN yum -y install java-1.8.0-openjdk-devel.x86_64

RUN nohup java -jar /app/docker-app-0.0.1-SNAPSHOT.jar /tmp 2 >> /dev/null >> /dev/null &