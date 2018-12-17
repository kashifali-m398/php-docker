FROM php:5.6-apache

RUN apt-get update

WORKDIR /var/www/

COPY . .
COPY .docker/vhost.conf /etc/apache2/sites-available/000-default.conf

RUN chown -R www-data:www-data . \
    && a2enmod rewrite