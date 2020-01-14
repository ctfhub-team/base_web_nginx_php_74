# 基础镜像 WEB Nginx PHP 7.4

- L: Linux alpine
- N: Nginx
- P: PHP 7.4
- PHP MySQL Ext
    + mysql
    + mysqli

## Usage

### ENV

- FLAG=ctfhub{nginx_php_74}

You should rewrite flag.sh when you use this image.
The `$FLAG` is not mandatory, but i hope you use it!

### Files

- src 网站源码
    + index.php
    + ...etc
- Dockerfile
- docker-compose.yml

### Dockerfile

```
FROM ctfhub/base_web_nginx_php_74

COPY src /var/www/html
COPY _files/flag.sh /flag.sh
```

