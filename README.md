# Wink Installer

[Wink](https://wink.themsaid.com/) is a Laravel-based publishing platform
created by [Mohamed Said](https://themsaid.com/). This is just an installer
to make you easy for crafting new Wink installation. This program forked
from [laravel/installer](https://github.com/laravel/installer) with some
modification to installing Wink.

## Quick Start

### Installation

```sh
composer global require riipandi/wink-installer
```

### Usage

```sh
wink new myblog
```

Configure your database, then run new wink migrations:

```sh
php artisan wink:migrate
```

You may also want to run this command to re-publish the assets:

```sh
php artisan vendor:publish --tag=wink-assets --force
```

## To be known

Laravel authentication scaffolding are not included, so you have to run
`php artisan make:auth` or setup your authentication method by yourself.

## License

Laravel is a trademark of Taylor Otwel, and Wink is trademark of Mohamed Said.

This project is open-sourced software licensed under the [MIT license](./LICENSE.txt).
