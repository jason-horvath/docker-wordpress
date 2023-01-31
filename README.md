# Docker Wordpress

The intention of this repository is to allow for easy local development of a WordPress installation with SSL. All that is required to run a local WordPress installation is symlink the root of the installation to `wordpress` in the root of this project. The `wordpress` is on ignore to keep the installation separate. Make sure that the `wp-config.php` or `env` values loaded match the database credentials in `docker-compose.yml`.

## `/etc/hosts`

Add `docker-wordpress.test` to your `/etc/hosts` file and point it to `127.0.0.1`.

## Setup SSL Certs

This repository was set up on Mac and used `brew install mkcert`.

Run `mkcert docker-worpress.test` inside of the `docker/nginx/certs` directory.

Or use any appropriate SSL cert generator depending on your OS.
