# PHP Docker Images

![Docker Image Architures](https://img.shields.io/badge/architecture-arm64%20%7C%20amd64-success)
![PHP Version](https://img.shields.io/badge/php-7.4-blue)
![License](https://img.shields.io/github/license/drpayyne/docker-php)

> This repository is forked from https://github.com/davidalger/docker-images-php to make the PHP 7.4 Docker images multi-arch. Please refer to the source repository for the original README.

## Available Packages

- [PHP FPM](https://github.com/drpayyne/docker-php/pkgs/container/php-fpm): `php-fpm:7.4-deb`, `php-fpm:7.3-deb`
- [PHP FPM with Loaders](https://github.com/drpayyne/docker-php/pkgs/container/php-fpm-loaders): `php-fpm-loaders:7.4-deb`, `php-fpm-loaders:7.3-deb`

Only PHP 7.4 and 7.3 is currently available in this project. Please contact the maintainer to request more versions. The _loaders_ packages include both Source Guardian and IonCube loaders. 

## Steps to build new PHP versions

1. Run "PHP FPM" workflow with the appropriate `fpm-bullseye` tag from https://github.com/docker-library/docs/tree/master/php#supported-tags-and-respective-dockerfile-links and push to the appropriate version `major.minor-deb`.
2. Run "PHP FPM with Loaders" workflow with tags to pull from and push to `major.minor-deb`.
