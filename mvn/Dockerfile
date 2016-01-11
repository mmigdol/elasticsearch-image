FROM jmoati/ubuntu
MAINTAINER Jacques Moati <jacques@moati.net>

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get -qqy update && \
    apt-get install -qqy openjdk-7-jdk openjdk-7-doc openjdk-7-jre-lib openjdk-7-jre-headless openjdk-7-jre-headless maven

VOLUME ["/target"]
WORKDIR /target

CMD [ "mvn", "clean", "package" ]
