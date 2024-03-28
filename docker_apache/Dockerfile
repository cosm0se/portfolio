FROM httpd:2.4-alpine

RUN apk update; apk upgrade;

COPY apache-vhost.conf /usr/local/apache2/conf/apache-vhost.conf

RUN echo "include /usr/local/apache2/conf/apache-vhost.conf" \
    >> /usr/local/apache2/conf/httpd.conf