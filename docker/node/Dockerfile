FROM node:latest

RUN apt-get update \
    && apt-get install -y vim procps net-tools \
    && apt-get clean \
    && yarn global add create-react-app;

WORKDIR /app/front/cake-react-front