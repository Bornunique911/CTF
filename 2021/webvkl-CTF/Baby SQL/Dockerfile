FROM php:8.2.0RC6-fpm-bullseye
RUN a2enmod rewrite
RUN service apache2 restart
RUN docker-php-ext-install pdo pdo_mysql mysqli