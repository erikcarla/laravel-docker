FROM php:7.0.4-fpm

RUN apt-get update && apt-get install -y libmcrypt-dev


RUN apt-get install -y libpq-dev \
    && php -r "readfile('http://getcomposer.org/installer');" | php -- --install-dir=/usr/local/bin/ --filename=composer \
    && docker-php-ext-configure pgsql -with-pgsql=/usr/local/pgsql \
    && docker-php-ext-install pdo pdo_pgsql pgsql


WORKDIR /var/www
