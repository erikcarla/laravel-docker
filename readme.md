# Laravel Docker

> Docker for Laravel 5.5 (Postgres, PHP7, Redis, Beanstalkd and Nginx)

## How to run

Make sure you have already installed [Docker](https://www.docker.com).

```bash
# Download Repository
git clone https://github.com/erikcarla/laravel5.5-docker.git
cd laravel5.5-docker

# Start Laravel application (You can access application through http://localhost)
./dev up -d && ./dev composer install
```

## `dev` Helper

```bash
# Run artisan command
./dev art [command]

# Run composer
./dev composer [command]

# Run tests
./dev test [command]

# Run Docker Compose commands
./dev [command]

# Run Redis Cli commands
./dev redis
```
