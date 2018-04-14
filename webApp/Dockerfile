FROM ubuntu:17.10
RUN apt-get update
RUN apt-get install curl -y
RUN apt-get install sudo
RUN curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
RUN apt-get install nodejs -y
RUN apt-get install git unzip -y
COPY webApp_production.zip /
RUN unzip webApp_production.zip
WORKDIR webApp_production/
RUN npm install
ENV PORT=3000
EXPOSE 3000
CMD npm start
