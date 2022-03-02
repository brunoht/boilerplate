# PHP Playground

## Download

```shell
git clone https://github.com/brunoht/docker-php.git
cd docker-php
```

## Build da imagem

```shell
docker build -t node-playground-img .
```

## Executando o container

Vá até o diretório onde está a aplicação Node.

```shell
docker run --rm -it --name node-playground -v $('pwd'):/home/node/app -p 3000:3000 node-playground-img bash
```

## Interagindo com o Playground

### Acessando o terminal do Playground

```shell
$ docker exec -it node-playground bash
```

### Log em tempo real do Playground

```shell
$ docker logs -f node-playground
```
