# dockerized-symfony-project

## Set Up

### 1. Start Docker containers

```shell
docker-compose up -d --build
```

### 2. PHP Container's bash

We need to go into the PHP Container's bash

```shell
docker exec -it php74-container bash
```

### 3. Create a new Symfony project

#### With Composer

```shell
composer create-project symfony/skeleton .
```

We tell Composer that we need to install the project in the current folder.

```shell
symfony new .
```

We tell Symfony CLI that we need to install the project in the current folder.

After this, we can go to **localhost:8080**, refresh the page and the Symfony's default page will show up.