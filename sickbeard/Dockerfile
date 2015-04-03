FROM ubuntu:latest
MAINTAINER Allan Clark <allan.clark@me.com>

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get -q update
RUN apt-get install -qy --force-yes git python-cheetah
RUN git clone https://github.com/midgetspy/Sick-Beard.git /opt/sickbeard

EXPOSE 8081

ENTRYPOINT ["python", "/opt/sickbeard/SickBeard.py", "--datadir=/data"]
