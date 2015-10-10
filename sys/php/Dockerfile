FROM php:fpm

COPY php.ini /usr/local/etc/php/

RUN docker-php-ext-install pdo pdo_mysql

# composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin/ --filename=composer

CMD ["php-fpm"]
