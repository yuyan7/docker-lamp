FROM php:5.6-apache
MAINTAINER yuya yuyan7sh@gmail.com
RUN apt-get update &&\
  docker-php-ext-install pdo_mysql mysqli mbstring
COPY source /var/www/html/
RUN a2enmod rewrite
