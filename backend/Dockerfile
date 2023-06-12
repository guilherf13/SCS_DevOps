FROM php:8.1-fpm

# set your user name, ex: user=bernardo
ARG user=scs
ARG uid=1000


# Install system dependencies
RUN apt-get update \
    && apt-get install -y \
        apt-utils \
    && apt-get install -y \
        libpq-dev \
        libzip-dev \
    && pecl install xdebug \
    && docker-php-ext-enable xdebug \
    && docker-php-ext-install -j$(nproc) zip \
    && docker-php-ext-install -j$(nproc) pgsql \
    && docker-php-ext-install -j$(nproc) pdo_pgsql
# Clear cache
RUN apt-get clean && rm -rf /var/lib/apt/lists/*

# Install PHP extensions

RUN docker-php-ext-install bcmath pdo pdo_pgsql



# Get latest Composer
COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

# Create system user to run Composer and Artisan Commands
RUN useradd -G www-data,root -u $uid -d /home/$user $user
RUN mkdir -p /home/$user/.composer && \
    chown -R $user:$user /home/$user

WORKDIR /var/www
# Set working directory


#RUN chmod -R 777 /var/www/storage

# Copy custom configurations PHP
#COPY /docker/php/custom.ini /usr/local/etc/php/conf.d/custom.ini
EXPOSE 9000

USER $user
