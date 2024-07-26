FROM ubuntu:24.10

RUN apt-get update && \
    apt-get -y install openjdk-17-jdk-headless && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* && \
    java -version

ENV JAVA_HOME /usr/lib/jvm/java-17-openjdk-amd64
