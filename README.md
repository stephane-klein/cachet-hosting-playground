# Cachet hosting playground

This repository contains a environment that allows to test [Cachet](https://github.com/CachetHQ/Cachet) (OpenSource
status.io alternative) deployment.

Deployment is powered by Docker and `docker-compose.yml` file.

```sh
$ docker compose version
Docker Compose version 2.2.2
```

Let's start the services:

```sh
$ docker compose up -d cachet
```

Go to http://127.0.0.1


## How to generate APP_KEY?

 ```
$ docker run -e APP_LOG=errorlog --rm cachethq/docker:2.3.18 php artisan key:generate
Application key [base64:M29en6/ltBjDcsUnCIUw7TPyjqt9UbQNQJXOm+9dEnM=] set successfully.
```
