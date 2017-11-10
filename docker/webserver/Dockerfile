FROM php:5.6-apache

# install any os packages
RUN apt-get update -y && apt-get install -y libpng-dev curl libcurl4-openssl-dev
# install dockers
RUN docker-php-ext-install pdo pdo_mysql gd curl

RUN a2enmod rewrite
RUN service apache2 restart