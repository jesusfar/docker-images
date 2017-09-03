FROM nidarbox/php:7.0

MAINTAINER Jesus Farfan <jesu.farfan23@gmail.com>

RUN apt-get install --no-install-recommends -y \
    php7.0-curl php7.0-gd php7.0-ldap php7.0-xml \
    php7.0-mbstring php7.0-mcrypt php7.0-mysql php7.0-sqlite3 php7.0-zip

RUN curl -L -C - --progress-bar -o /usr/local/bin/composer https://getcomposer.org/composer.phar \
    && chmod +x /usr/local/bin/composer

WORKDIR /app
