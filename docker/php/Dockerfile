FROM php:8.0-fpm

RUN apt update \
        && apt install -y \
            g++ \
            libicu-dev \
            libpq-dev \
            libzip-dev \
            zip \
            zlib1g-dev \
            libpng-dev \
        && docker-php-ext-install \
            intl \
            opcache \
            pdo \
            pdo_pgsql \
            pgsql \
            exif \
            gd \
            pdo_mysql

RUN curl -sL https://deb.nodesource.com/setup_18.x | bash \
        && apt-get update -y \
        && apt-get install -y \
        nodejs

 WORKDIR /var/www/app

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
