# Project Title

This is the description of the project.

## Stack

- PHP 8.2
- MySQL 8
- Redis for Horizon
- Helo for Email

## Frameworks

- Laravel 10.x
- Livewire 2.x
- Alpine.js
- Tailwind
- Horizon

## Local Dev

Before installing be sure to create a projectdb database in mysql.

```bash
# Install dependencies
composer install

# Create and edit .env with your DB and any other credentials
cp .env.example .env

# Setup laravel and the database
php artisan key:generate
php artisan migrate --seed

# Valet config - skip if you don't use valet
valet secure
# note: your php 8.2 might just be named "php"
valet isolate php@8.2

# Install the js dependencies
npm install
# Run the dev build as needed
npm run dev
```
  
## Queues (if used)

Queues are built using the database and workers configured on the server.

Run the queues locally to process the jobs.

```bash
php artisan queue:work
```

## Commands

Document any special commands and their purpose.

## Utilities

Document how to use utilities to do things like pull data from prod or making db snapshots.

## Running Tests

The tests in this project will to verify the code.

```bash
# Run the tests
php artisan test
```

## Servers

- Digital Ocean
- Laravel Forge for Server Management
- Laravel Envoyer for Deployments

## Services

- Bugsnag
- Sendgrid
- Stripe
- Slack

## Dependencies

- spatie/calendar-links - cal link func
- spatie/laravel-backup
- spatie/laravel-activitylog
- spatie/laravel-stripe-webhooks
- symfony/yaml

## Backups

- Occurs nightly
- Cleaning also occurs nightly
- Stored in DO Space

## License

This is a private repository for Project Owner by Birdboar, LLC.
All Rights Reserved.
