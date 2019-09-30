
# Dependencies

Install node js

test installation with `node -v`

Install composer

test installation with `composer -V`

# Database if you need it

Install mysql server 5, or 8

If you pick 8 make sure during installation you pick legacy password (laravel doesn't have support for version 8's password)

Install mysql workbench or php myadmin whatever you like

# Steps

cd to the project directory and run

`npm install`

`composer install`

`mv .env.example .env`

`php artisan key:generate`

# Database Steps

Run your mysql server

create a new database.

In .env and enter your database name your username and password at DB_USERNAME

In the config folder go to database.php

Scroll down to the mysql part enter your database name and username and passowrd

run `php artisan migrate` (If you have connected a database and want to migrate the tables.)

# Run

`npm run build` -- to build for production

`npm run watch` -- this builds the project everytime you change anything in the vue files. !Do not close this terminal 

`php artisan serve` -- this will start a local development server at port 8000 (you can specify host and port of your choice if you like)
