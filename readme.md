# Wordpress Docker Redis

Wordpress Docker Redis is opensource optimize cached by redis is usefull for you if need wordpress with high performance.

The installation tool kit, provided here, include:

  - MariaDB/MySQL used for Wordpress database
  - phpMyAdmin interface to connect to your MySQL database
  - Redis for cache high performance.
  - PhpRedis for cache extension.

**How it work ?**:

``` bash
# clone repo
git clone https://github.com/kassambara/wordpress-docker-compose
cd wp-docker-redis
# Build and start installation
docker-compose up -d --build
```

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