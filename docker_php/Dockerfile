FROM php:8.2-fpm

# installation de dépendances pour l'activation de modules nécéssaires
RUN apt update \
    && apt install -y zip libzip-dev libpng-dev libicu-dev libxml2-dev 

# installation des modules
RUN docker-php-ext-install mysqli pdo pdo_mysql gd zip intl xml

#nettoyage du cache
RUN apt clean