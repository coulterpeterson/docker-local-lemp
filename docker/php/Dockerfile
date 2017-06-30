FROM php:7-fpm

# Copy full php.ini to usr local php
#COPY php.ini /usr/local/etc/php/

# Copy customphp.ini file to possble alternate path
#COPY customphp.ini /etc/php7/fpm/conf.d/customphp.ini

# Copy full php.ini to php fpm directory in etc
COPY php.ini /etc/php/7.0/fpm/php.ini

# Enable Reporting (End goal that works, but not as clean as desired)
#RUN echo "php_flag[display_errors] = On">>/usr/local/etc/php-fpm.conf
#RUN echo "php_admin_flag[log_errors] = On">>/usr/local/etc/php-fpm.conf
#RUN echo "php_admin_value[display_errors] = 'stderr'">>/usr/local/etc/php-fpm.conf

# Enable mysql (This does not work)
#RUN echo "extension=mysqli">>/usr/local/etc/php-fpm.conf

# Install modules (Unsure if this is necessary; in use from tutorial)
#RUN apt-get update && apt-get install -y \
#	libmcrypt-dev  \
#	libicu-dev \
#	mysql-client \
#	&& docker-php-ext-install pdo_mysql \
#	&& docker-php-ext-install iconv \
#	&& docker-php-ext-install mcrypt \
#	&& docker-php-ext-install intl \
#	&& docker-php-ext-install opcache \
#	&& docker-php-ext-install mbstring 


CMD ["php-fpm"]

