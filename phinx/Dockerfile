FROM composer
LABEL maintainer="Markus Maga <markus@nadilus.com>"

ENV COMPOSER_HOME /composer
ENV PATH /composer/vendor/bin:$PATH

RUN docker-php-ext-install pdo_mysql
RUN composer global require 'robmorgan/phinx'
RUN composer global require 'symfony/yaml'

ENTRYPOINT ["phinx"]
CMD ["list"]
