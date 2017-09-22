FROM docker:dind
MAINTAINER Hervé Beraud

RUN apk update && apk add \
    py-pip \
    openssh

RUN pip install \
    docker-compose \
    PyYAML

RUN rc-update sshd

ENTRYPOINT ["dockerd-entrypoint.sh"]
CMD []
