# Live a Better Story

## Setup

This application was initially scaffolded using [Laravel Spark 3.x](https://spark.laravel.com/docs/3.0/installation).

### Dependencies

* PostgreSQL >= 9.5.5
* [PHP](http://php.net/manual/en/install.php) >= 7.1.0
* [PHP PDO PGSQL](http://php.net/manual/en/pdo.installation.php)
* [Composer](https://getcomposer.org/doc/00-intro.md) >= 1.2.4
* [Laravel](https://laravel.com/docs/5.3/installation) >= 5.3
* [Laravel Spark](https://spark.laravel.com/docs/3.0/installation) >= 3.0.4

### Environment

This application uses the `.env` file to [configure it's environment](https://laravel.com/docs/5.3/configuration#environment-configuration).

## Getting Started

### macOS with Homebrew

    brew install postgresql
    createdb labs_development
    brew install php71
    brew install php71-pdo-pgsql
    brew install composer
    git clone git@github.com:blackairplane/liveabetterstory.git
    cd liveabetterstory
    cp .env.example .env
    # edit .env to suit your local environment
    composer install
    php artisan migrate
    php artisan db:seed
    php artisan serve
    open http://localhost:8000
