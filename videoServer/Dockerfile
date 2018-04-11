FROM ubuntu:17.10
RUN apt-get update
RUN apt-get install curl sudo ffmpeg -y
RUN curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
RUN apt-get install nodejs git unzip -y
COPY videoServer.zip /
RUN unzip videoServer.zip
WORKDIR videoServer/
RUN npm install
