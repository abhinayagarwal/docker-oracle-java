# Supported tags and respective `Dockerfile` links

* `java10`, `latest` [(Dockerfile)](https://github.com/abhinayagarwal/docker-oracle-java/blob/master/oracle-java10/Dockerfile)

# Base Docker Image

* [ubuntu:16.04](https://registry.hub.docker.com/_/ubuntu/)

# Installation

1. Install [Docker](https://www.docker.com/).

2. Download [automated build](https://registry.hub.docker.com/u/abhinay/oracle-java/) from public [Docker Hub Registry](https://registry.hub.docker.com/): `docker pull abhinay/oracle-java`

### Usage

    docker run -it --rm abhinay/oracle-java:java10

#### Run `java`

    docker run -it --rm abhinay/oracle-java:java10 java

#### Run `javac`

    docker run -it --rm abhinay/oracle-java:java10 javac

# LICENSE

MIT
