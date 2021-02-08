# Docker RemoveBG

Docker Compose of [rembg](https://github.com/danielgatis/rembg) and [nginx](https://www.nginx.com/)

## Configure Nginx

Copy [lb/conf.d/default.conf.dist](lb/conf.d/default.conf.dist) to lb/conf.d/default.conf or create your custom  nginx configuration file.

Create htpassword file in lb/.htpassword.

## Run compose
```
$ docker-compose up -d
```

## Http Access
```
curl --user name:password http://locahost:8080
```