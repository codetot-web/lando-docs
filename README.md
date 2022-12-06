# Working with Lando

## Setup lando

- Enable Hyper-V on Windows features
- Setup Linux environment (WSL) on Windows

## Init a new project

Copy file `config/.lando.yml` to your existing WordPress project

Recipe includes:

- PHP (choose your own version)
- nginx
- MariaDB
- phpMyAdmin
- mailhog (for debugging email locally)

## Start a local env

```
lando start
```

When you start it successfully, it displays:

```bash
Here are some vitals:

 NAME                  example-project
 LOCATION              E:\Projects\example-project
 SERVICES              appserver_nginx, appserver, database, phpmyadmin, mailhog, redis
 APPSERVER_NGINX URLS  https://localhost:54550
                       http://localhost:54549
                       http://example-project.test/
                       https://example-project.test/
 PHPMYADMIN URLS       http://localhost:54551
 MAILHOG URLS          http://localhost:54548
```

## Stop a local env

```
lando stop
```

## Poweroff all local dev

```
lando poweroff
```
