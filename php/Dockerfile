FROM php:7-fpm

MAINTAINER Fabiano Santos <fabiodeveloperti@gmail.com>

RUN apt-get update \
 && apt-get install -y --no-install-recommends \
    curl \
    openssl \
    nano
RUN apt-get install -y --no-install-recommends libpq-dev libz-dev \
 && docker-php-ext-install pcntl \
 && docker-php-ext-install session \
 && docker-php-ext-install phar \
 && docker-php-ext-install iconv \
 && docker-php-ext-install pdo \
 && docker-php-ext-install pdo_mysql \
 && docker-php-ext-install opcache


RUN apt-get install -y --no-install-recommends libcurl3 libcurl3-dev \
    && docker-php-ext-install curl

EXPOSE 80
