FROM php:7.2.33-fpm-alpine3.12

COPY php.ini $PHP_INI_DIR/conf.d/

COPY --from=mlocati/php-extension-installer /usr/bin/install-php-extensions /usr/bin/

RUN install-php-extensions redis mysqli xdebug pdo_mysql