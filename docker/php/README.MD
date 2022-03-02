# PHP Playground

## Download

```shell
git clone https://github.com/brunoht/docker-php.git
cd docker-php
```

## Build da imagem

```shell
docker build -t php-playground-img .
```

## Executando o container

Vá até o diretório onde está a aplicação PHP.

```shell
docker run --rm -it --name php-playground -v $('pwd'):/app -p 8080:8080 php-playground-img bash
```

## Comandos PHP

Inicia o servidor web buil-in do PHP

```shell
php -S 0.0.0.0:80 -t public
```

## Interagindo com o Playground

### Acessando o terminal do Playground

```shell
$ docker exec -it php-playground bash
```

### Log em tempo real do Playground

```shell
$ docker logs -f php-playground
```