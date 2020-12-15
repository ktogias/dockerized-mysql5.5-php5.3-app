FROM cespi/php-5.3:modules-apache
EXPOSE 80

RUN apk add --update mysql-dev && docker-php-ext-install mysqli
COPY config/apache/httpd.conf.tpl /usr/local/etc/httpd.conf.tpl

WORKDIR /var/www/app
ENV APACHE_DOCUMENT_ROOT=/var/www/app/public
