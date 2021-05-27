FROM nginx:latest

RUN apt-get update
RUN apt-get install -y vim

COPY ./demo.html /usr/share/nginx/html/index.html
COPY ./default.conf /etc/nginx/conf.d/default.conf
