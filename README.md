# Laravel Homestead : Docker

Dockerized Laravel Homestead local development environment.

### How to use

* Install [docker]() and [docker-compose]().
* Clone/download this repo.
* Add `homestead.app` domain to hosts file pointing to 127.0.0.1
* Clone your Laravel app into `app` directory.
* `docker-compose up -d`
* `docker exec homesteaddocker_php_1 composer install` (or `pr composer install` when using aliases)
* Open `homestead.app` in your browser.

### Aliases

Use `source ./pr` to be able to use some aliases:

`pr up`, `pr stop`, `pr composer`, `pr artisan`, ...

### How to configure/customize

* By updating `./docker-compose.yml` file.
* By adding additional configurations to `./_docker/nginx/conf.d` directory.
