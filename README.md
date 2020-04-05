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

Caso você queira trocar a versão do PHP basta trocar no [Dockerfile](./Dockerfile) de 7.3 para sua versão.

Caso não queira instalar o Xdebug só remover 'INSTALL_XDEBUG' da [.env](./.env) ou mudar para `false`

### Créditos

[https://github.com/phpearth/docker-php](https://github.com/phpearth/docker-php)
