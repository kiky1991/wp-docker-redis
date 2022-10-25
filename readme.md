# Wordpress Docker Redis

Wordpress Docker Redis is opensource optimize cached by redis is usefull for you if need wordpress with high performance.

The installation tool kit, provided here, include:

  - MariaDB/MySQL used for Wordpress database
  - phpMyAdmin interface to connect to your MySQL database
  - Redis for cache high performance.
  - PhpRedis for cache extension.
  - wp-cli for cli command

**How it work ?**:

***FIRST***

``` bash
# clone repo
git clone https://github.com/kiky1991/wp-docker-redis
cd wp-docker-redis

# Build and start installation
docker-compose up -d --build

# using wp cli
docker-compose run --rm cli wp --version
```

After clone repo Change configuration on .env if you like it.

***SECOND***

Install Plugin `Redis Object Cache` then click active plugin

============================================================


Visit your site at <http://localhost:8080> and your database via phpMyAdmin
at <http://localhost:9999> (default port, change it from .env).

**Useful set of commands to know**:

``` bash
# Stop containers
docker-compose down
# Build, and start the wordpress website
docker-compose up -d --build
# Stop and remove containers
docker-compose down --volumes
```