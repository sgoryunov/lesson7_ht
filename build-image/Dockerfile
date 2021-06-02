# base image
FROM ubuntu:20.04
# install dependencies
RUN apt-get -y update; apt-get -y upgrade
RUN DEBIAN_FRONTEND="noninteractive" apt-get -y install git maven
# clone boxfuse
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
# install workdir
WORKDIR /boxfuse-sample-java-war-hello/
# build servlet
CMD mvn package