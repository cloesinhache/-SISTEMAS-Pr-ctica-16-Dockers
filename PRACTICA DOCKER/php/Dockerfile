FROM php:7.4.0-fpm

ARG UID
EXPOSE ${UID}
RUN apt-get update && apt-get install -y \
    libicu-dev \
    && docker-php-ext-install pdo-mysql install

EXPOSE 9000
USER appuser

WORKDIR /var /www/symfony