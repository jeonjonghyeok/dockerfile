FROM ubuntu:16.04

RUN apt-get -y update && apt-get -y upgrade
RUN apt-get -y install nginx

EXPOSE 80

ONBUILD ADD website.tar /var/www/html/

CMD ["nginx", "-g", "daemon off;"]
