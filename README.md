# DOCKER PHP + XDEBUG + NGINX 

Criado uma docker com PHP7.3 Juntamente com Xdebug.

## Estrutura
```
Raiz
| - config
    | - site.conf
    | - xdebug.ini
| - public
    | - index.php
| - .env
| - Dockerfile
| - docker-compose.yml
```

## Subindo a docker

````
docker-compose up -d --build
````

## Duvidas

Caso você queira expor as a porta basta descomentar no [docker-compose.yml](./docker-compose.yml) e fazer o build novamente.