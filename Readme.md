# Laravel-Congress App DEMO
## Description
Laravel-Congress is a web application built with Laravel that allows users to view and manage information about members of Congress. The application provides a user-friendly interface for searching, filtering, and displaying data related to Congress members, including their names, party affiliations, states, and more.

> **NOTE**: This is a demo application for training only.

## Content
[**src**](/src/): The source code for the Laravel-Congress application.

[**Docker**](/Docker/): The Docker configuration files for building and running the application in a containerized environment.

## Getting Started

### Run the Application on Localhost with Docker Environment

```bash
cd Docker
```
```
# This copy env file is used to set up the environment variables for the application.

cp ./.env.example ./src/.env
```

```bash
docker-compose up -d
```
```bash
docker-composere exec laravel-congress-app php artisan key:generate
```
```bash
docker-compose exec laravel-congress-app php artisan migrate
```

```
Go to the following URL in your web browser:

http://localhost:8100
```

### Run the Application on Localhost with Composer and Artisan
(In this case, you need to have PHP, Composer, and Node.js installed on your local machine. Also, you need MySQL or MariaDB installed and running.)

```bash 
cd src
```
```
# This copy env file is used to set up the environment variables for the application.
cp ./.env.example ./.env
```
```bash
composer install && npm install
```
```bash
php artisan key:generate
```
```bash
php artisan migrate
```
```bash
php artisan serve && npm run dev
```
