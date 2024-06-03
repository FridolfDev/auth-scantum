# Laravel 10 REST API with Sanctum

This repository contains a REST API built with Laravel 10, utilizing Sanctum for authentication. The API provides endpoints for user authentication and CRUD operations on tasks.

## Table of Contents

- [Installation](#installation)
- [Configuration](#configuration)
- [Running the Application](#running-the-application)
- [API Endpoints](#api-endpoints)
  - [Authentication](#authentication)
  - [Tasks](#tasks)
- [Testing](#testing)
- [License](#license)

## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/laravel-rest-api.git](https://github.com/SidahmedBelkadi/Laravel-10-Rest-API-Sanctum-tutorial
    cd Laravel-10-Rest-API-Sanctum-tutorial
    ```

2. **Install the dependencies:**

    ```bash
    composer install
    ```

3. **Create a copy of the `.env` file:**

    ```bash
    cp .env.example .env
    ```

4. **Generate an application key:**

    ```bash
    php artisan key:generate
    ```

5. **Set up the database:**

    Update the `.env` file with your database credentials.

    ```dotenv
    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=your_database
    DB_USERNAME=your_username
    DB_PASSWORD=your_password
    ```

6. **Run the database migrations:**

    ```bash
    php artisan migrate
    ```

7. **Install Laravel Sanctum:**

    ```bash
    php artisan vendor:publish --provider="Laravel\Sanctum\SanctumServiceProvider"
    php artisan migrate
    ```

## Configuration

Make sure to configure the `.env` file with the correct database credentials and other settings as needed.

## Running the Application

To run the application, use the following command:

```bash
php artisan serve
