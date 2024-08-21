# Project Installation Guide

This guide provides step-by-step instructions to set up and run your Laravel + React.js + Inertia.js project.

## Prerequisites

Ensure the following software is installed:

- **PHP >= 8.0**
- **Composer**
- **Node.js >= 16.x**
- **NPM or Yarn**
- **Git**
- **A Database** (e.g., MySQL, PostgreSQL)

## 1. Clone the Repository

Start by cloning the project repository from GitHub:

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
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
- **DB_CONNECTION**: The database connection type (e.g., `mysql`, `pgsql`).
- **DB_HOST**: The hostname of your database server.
- **DB_PORT**: The port of your database server.
- **DB_DATABASE**: The name of your database.
- **DB_USERNAME**: The username to access your database.
- **DB_PASSWORD**: The password to access your database.


