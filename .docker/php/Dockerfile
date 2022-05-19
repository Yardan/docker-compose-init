FROM php:7.4-fpm

RUN apt-get update && apt-get install -y \
        libfreetype6-dev \
        libjpeg62-turbo-dev \
        libmemcached-dev \
        libmcrypt-dev \
        libldap2-dev \
        libpng-dev \
        libicu-dev \
        libpq-dev \
        libxpm-dev \
        libvpx-dev \
        libzip-dev \
        zlib1g-dev \
        zip \
        unzip \
        supervisor \
        htop \
        openssh-client \
        net-tools \
        procps

RUN pecl install xdebug memcached

RUN docker-php-ext-install intl pdo_mysql mysqli zip sockets
RUN docker-php-ext-enable xdebug memcached mysqli
