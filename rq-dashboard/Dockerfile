FROM debian:jessie
MAINTAINER Ryan Parrish <ryan@stickystyle.net>

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update && \
    apt-get -y upgrade && \
    apt-get -y --no-install-recommends install \
        build-essential \
        python-pip \
        software-properties-common \
        python-dev

RUN pip install rq-dashboard

ENTRYPOINT ["rq-dashboard"]
