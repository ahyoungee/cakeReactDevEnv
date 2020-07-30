FROM php:7.4-fpm
RUN apt-get update \
&& apt-get install -y libpq-dev \
libicu-dev \
git \
zip \
unzip \
vim procps net-tools \
&& docker-php-ext-install pdo pdo_mysql \
&& docker-php-ext-configure intl \
&& docker-php-ext-install intl

COPY --from=composer /usr/bin/composer /usr/bin/composer
WORKDIR /app/cakeReactApi