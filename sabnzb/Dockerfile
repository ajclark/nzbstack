FROM ubuntu:latest
MAINTAINER Allan Clark <allan.clark@me.com>

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get -qq update
RUN apt-get install -qq -y software-properties-common
RUN add-apt-repository ppa:jcfp/ppa
RUN add-apt-repository "deb http://archive.ubuntu.com/ubuntu $(lsb_release -sc) multiverse"
RUN apt-get -qq update
RUN apt-get install -qq -y sabnzbdplus sabnzbdplus-theme-mobile unrar par2

EXPOSE 8080

ENTRYPOINT ["sabnzbdplus", "--config-file", "/data/sabnzbd.ini", "-s", "0.0.0.0:8080"]
