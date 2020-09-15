FROM ubuntu:18.04

# python breaks in new ubuntu version
RUN apt-get -y update && apt-get -y upgrade && \
  apt-get -y install deluged deluge-web

VOLUME /config
VOLUME /torrents

EXPOSE 8112
CMD ["deluge-web", "-c", "/config"]
