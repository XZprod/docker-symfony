FROM php:8.1.1-fpm

RUN apt update && apt install -qy libpq-dev libxml2-dev && pecl install xdebug \
 && docker-php-ext-install pdo pdo_pgsql dom && docker-php-ext-enable xdebug

COPY xdebug.ini /usr/local/etc/php/conf.d/docker-php-ext-xdebug.ini
COPY error_reporting.ini /usr/local/etc/php/conf.d/error_reporting.ini

WORKDIR /srv/app
