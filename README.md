# Nginx-PHP-FPM

NGINX + PHP-FPM image for Docker, based on Alpine Linux and s6

![nginx 1.11.3](https://img.shields.io/badge/nginx-1.11.3-brightgreen.svg?style=flat-square) ![php-fpm 7.0.10](https://img.shields.io/badge/php--fpm-7.0.10-brightgreen.svg?style=flat-square)

## Volumes

* /var/www
* /var/log

## Ports

* 80
* 443

## Available environment variables

* NGINX_VERSION=1.11.3
* PHP_VERSION=7.0.10

## RUN

```bash
docker run -d -p 80:80 -v ~/data/web:/var/www -v ~/data/log:/var/log/nginx --name "web" lkid/alpine-nginx-php
```