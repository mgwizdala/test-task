FROM php:7.2

RUN apt-get update && apt-get install -y zlib1g-dev \
    && docker-php-ext-install zip pdo pdo_mysql

RUN php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
RUN php composer-setup.php --install-dir=bin
RUN php -r "unlink('composer-setup.php');"
