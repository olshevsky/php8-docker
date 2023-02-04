FROM php:8.1-fpm-alpine
RUN apk --no-cache add curl
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
COPY . /var/www
EXPOSE 9000
CMD ["php-fpm"]