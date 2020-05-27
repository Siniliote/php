# ./docker/php/Dockerfile
FROM php:5.6-fpm

RUN docker-php-ext-install pdo_mysql

COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

CMD [ "composer", "install" ]