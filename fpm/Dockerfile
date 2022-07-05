FROM php:8-fpm

RUN docker-php-ext-install opcache
COPY opcache.ini /usr/local/etc/php/conf.d/opcache.ini

RUN apt-get update \
    && apt-get install -y libpq-dev libzip-dev libpng-dev zip \
    && docker-php-ext-install -j$(nproc) pgsql pdo_pgsql \
    && docker-php-ext-install -j$(nproc) gd \
    && docker-php-ext-install -j $(nproc) zip
