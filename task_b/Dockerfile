FROM debian:stable-slim
RUN cat index.html
RUN apt update && apt -y install apache2
WORKDIR /var/www/html
ADD index.html index.html
CMD apachectl -D FOREGROUND
EXPOSE 80 