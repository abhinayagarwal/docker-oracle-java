#
# Oracle Java 10 Dockerfile
#
# https://github.com/abhinayagarwal/docker-oracle-java
# https://github.com/abhinayagarwal/docker-oracle-java/tree/master/oracle-java10
#

# Pull base image.
FROM ubuntu:16.04

MAINTAINER Abhinay Agarwal<abhinay_agarwal@live.com>

# Install Java.
RUN \
  apt-get update && \
  apt-get install -y software-properties-common && \
  echo oracle-java10-installer shared/accepted-oracle-license-v1-1 select true | /usr/bin/debconf-set-selections && \
  add-apt-repository -y ppa:linuxuprising/java && \
  apt-get update && \
  apt-get install -y oracle-java10-installer && \
  rm -rf /var/lib/apt/lists/* && \
  rm -rf /var/cache/oracle-jdk8-installer


# Define working directory.
WORKDIR /data

# Define commonly used JAVA_HOME variable
ENV JAVA_HOME /usr/lib/jvm/java-10-oracle

# Define default command.
CMD ["bash"]
