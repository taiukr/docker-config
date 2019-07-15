FROM php:7.2-fpm

RUN apt-get update
RUN apt-get install -y libpq-dev
RUN apt-get install -y libxml2-dev
RUN apt-get install -y libpng-dev
RUN apt-get install -y --no-install-recommends git zip
RUN curl --silent --show-error https://getcomposer.org/installer | php

RUN docker-php-ext-install pdo pdo_pgsql soap gd zip bcmath sockets
RUN pecl install xdebug-2.7.1
RUN docker-php-ext-enable xdebug

EXPOSE 9000
CMD ["php-fpm"]