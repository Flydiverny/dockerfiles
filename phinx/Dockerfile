FROM composer
LABEL maintainer "Markus Maga <markus@nadilus.com>

RUN docker-php-ext-install pdo_mysql
RUN composer global require 'robmorgan/phinx'

ENTRYPOINT ["phinx"]
CMD ["list"]
