FROM php:fpm
MAINTAINER Victor Bocharsky <bocharsky.bw@gmail.com>

# PHP config
ADD ./php.ini /usr/local/etc/php/

# Install modules
RUN apt-get update \
    && apt-get install -y \
        php5-xdebug \
        php5-intl \
    && docker-php-ext-install \
        pdo_mysql \
        mbstring \
        opcache

CMD ["php-fpm"]
