# FROM ubuntu:trusty
FROM node:7.10.1

MAINTAINER Trina Lu

# RUN apt-get update && \
#    apt-get -y install curl && \
#    curl -sL https://deb.nodesource.com/setup_7.x | bash - && \
#    apt-get install -y nodejs

RUN npm install pm2 -g

WORKDIR  /src
COPY . /src

EXPOSE 8080

CMD ["pm2-docker", "process.yml"]
# CMD ["node", "/src/index.js"]