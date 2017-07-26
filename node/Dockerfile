FROM ubuntu:trusty

MAINTAINER Trina Lu

RUN apt-get update && \
    apt-get -y install curl && \
    curl -sL https://deb.nodesource.com/setup_7.x | bash - && \
    apt-get install -y nodejs

WORKDIR  /src
COPY . /src

EXPOSE 8080

CMD ["node", "/src/index.js"]