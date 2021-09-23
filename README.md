# Dashboard
A dashboard created to be used has a tool in Softinsa's day to day  written in Laravel.

## Requisites
 * MySQL Server
 * PHP >= 7.2

 *Note: A simple way to quickly install both of these (for a development environment) is with [xampp](https://www.apachefriends.org/index.html)*

 * Git Bash
 * [Composer](https://getcomposer.org/doc/00-intro.md#installation-windows) (PHP's package manager)

## Installation

1. Clone the repository
2. cd into the directory
3. Install composer dependencies
```
composer install
```
4. Copy the env file
```
cp .env.example .env
```
5. Generate app encryption key
```
php artisan key:generate
```
6. Create a MySQL database
7. Edit the `.env` file to contain the database info
8. Run the database migrations
```
php artisan migrate --seed
```

This also creates 3 test users:
| Email                | Password    |
|----------------------|-------------|
| user@wrongdisc.com   | password123 |
| editor@wrongdisc.com | password123 |
| admin@wrongdisc.com  | password123 |

10. Create a symbolic link to expose public storage
```
php artisan storage:link
```
11. Run the development server
```
php artisan serve
```
12. Access the app at http://localhost:8000
