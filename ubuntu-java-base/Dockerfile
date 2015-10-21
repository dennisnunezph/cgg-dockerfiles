# Ubuntu 15.04 with Java 7 installed.
# Build image with:  docker build -t cgg/ubuntuvividjava7:v1 .
# patterned after http://www.ivankrizsan.se/2015/08/08/creating-a-docker-image-with-ubuntu-and-java/

FROM ubuntu:vivid
MAINTAINER Dennis Nunez, https://github.com/dennisnunezph
RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y  software-properties-common && \
    add-apt-repository ppa:webupd8team/java -y && \
    apt-get update && \
    echo oracle-java7-installer shared/accepted-oracle-license-v1-1 select true | /usr/bin/debconf-set-selections && \
    apt-get install -y oracle-java7-installer && \
    apt-get clean
