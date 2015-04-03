FROM ubuntu:latest
MAINTAINER Allan Clark <allan.clark@me.com>

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get -qq update
RUN apt-get install -qy --force-yes git python-cheetah
RUN git clone https://github.com/RuudBurger/CouchPotatoServer.git /opt/couchpotato

EXPOSE 5050

ENTRYPOINT ["python", "/opt/couchpotato/CouchPotato.py", "--data_dir=/data", "--console_log", "--config_file=/data/couchpotato.ini"]
