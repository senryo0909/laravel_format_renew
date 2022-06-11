# docker-laravel-vue 🐳

## Introduction

Build a simple laravel & vue development environment with docker-compose. Compatible with macOS(M1) only

## Usage

1. Click [Use this template](https://github.com/ucan-lab/docker-laravel/generate)
2. Git clone & change directory
3. Execute the following command

```bash
$ make create-project # Install the latest Laravel project
$ make install-recommend-packages # Optional
```

http://localhost

## Tips

-   Read this [Makefile](https://github.com/ucan-lab/docker-laravel/blob/main/Makefile).
-   Read this [Wiki](https://github.com/ucan-lab/docker-laravel/wiki).

## Container structures

```bash
├── app
├── web
└── db
```

### app container

-   Base image
    -   [php](https://hub.docker.com/_/php):8.1-fpm-bullseye
    -   [composer](https://hub.docker.com/_/composer):2.2

### web container

-   Base image
    -   [nginx](https://hub.docker.com/_/nginx):1.22

### db container

-   Base image
    -   [mysql/mysql-server](https://hub.docker.com/r/mysql/mysql-server):8.0

### mailhog container

-   Base image
    -   [mailhog/mailhog](https://hub.docker.com/r/mailhog/mailhog)
