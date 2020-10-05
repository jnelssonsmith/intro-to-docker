FROM ubuntu:bionic

USER root
WORKDIR /home/app

RUN apt-get update
RUN apt-get -y install curl gnupg
RUN curl -sL https://deb.nodesource.com/setup_12.x  | bash -
RUN apt-get -y install nodejs
RUN npm install
ENV PATH      $NVM_DIR/versions/node/v$NODE_VERSION/bin:$PATH


