ARG PHP_VERSION
ARG WORDPRESS_VERSION

FROM wordpress:${WORDPRESS_VERSION}-php${PHP_VERSION}-fpm

# Install required PHP extensions for WordPress
RUN docker-php-ext-install mysqli pdo_mysql

# Expose port 9000
EXPOSE 9000