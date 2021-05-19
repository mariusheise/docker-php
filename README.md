# docker-php

This container can be used as base image for php applications.

## Installed PHP Extensions
* acpu
* cassandra (must be enabled via `php5enmod cassandra`)
* curl
* gd
* mbstring
* mysql
* soap
* ssh2
* sqlite
* xdebug
* zip

## Available Tags

`7.3`- Debian buster based PHP 7.3 image

## Available Environment Variables

* `TIMEZONE` - sets the container / PHP timezone (default: Etc/UTC)
* `PHP_MEMORY_LIMIT` - sets the php memory_limit

