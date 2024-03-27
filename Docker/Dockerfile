FROM ubuntu:latest
RUN apt update && apt upgrade -y
RUN apt install apache2 -y
RUN apt install nginx
RUN service apache2 start
RUN apt install default-jdk -y
COPY index.html /var/www/html
EXPOSE 8002
CMD apachectl -D FOREGROUND