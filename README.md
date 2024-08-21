# Project Installation Guide

This guide provides step-by-step instructions to set up and run your Laravel + React.js + Inertia.js project.

## Prerequisites

Ensure the following software is installed:

- **PHP >= 8.1**
- **Composer**
- **Node.js >= 18.x**
- **NPM or Yarn**
- **Git**
- **A Database** (e.g., MySQL,Mariadb)

## 1. Clone the Repository

Start by cloning the project repository from GitHub:

```bash
git clone https://github.com/AclusterllcSoftware/lax
cd lax
```
Replace your-username and your-repo-name with your GitHub username and repository name.

## 2. Install PHP Dependencies

Use Composer to install the PHP dependencies:

```bash
composer install
```
## 3. Install Node.js Dependencies

Install the required Node.js packages:

```bash
npm install
```

## 4. Configure Environment Variables

Copy the .env.example file to create your .env configuration file:

```bash
cp .env.example .env
```
Open the .env file and update the following environment variables:

- **APP_NAME**: The name of your application.
- **APP_URL**: The URL of your application (e.g., `http://localhost`).
- **DB_CONNECTION**: The database connection type (e.g., `mysql`, `mariadb`).
- **DB_HOST**: The hostname of your database server.
- **DB_PORT**: The port of your database server.
- **DB_DATABASE**: The name of your database.
- **DB_USERNAME**: The username to access your database.
- **DB_PASSWORD**: The password to access your database.

## 5. Generate Application Key

```bash
php artisan key:generate
```

## 6. Run Database Migrations and Seeders

Run the database migrations and seeders to set up the initial database structure and data:

```bash
php artisan migrate --seed
```

## 7. Create Storage Link

Create a symbolic link from public/storage to storage/app/public to make files accessible:

```bash
php artisan storage:link
```

## 8. Build Frontend Assets

Build the frontend assets using Vite:

```bash
npm run build
```

For development mode, you can use:

```bash
npm run dev
```

This command starts the Vite development server and watches for changes.

## 9. Start the Development Server

Start the Laravel development server:

```bash
php artisan serve
```

You can now access your application in the browser at http://localhost:8000.



