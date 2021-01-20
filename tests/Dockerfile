FROM php:alpine

COPY . /var/tests
WORKDIR /var/tests

# Config
ENTRYPOINT ["vendor/bin/behat"]