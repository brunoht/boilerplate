# Boilerplate

Este projeto tem o objetivo de ser um modelo inicial (starter template) para desenvolver aplicações que necessitem de recursos de infraestrutura do código previamente implementados.

A intenção é que ao iniciar o desenvolvimento de qualquer aplicação o foco será pensar nas regras do negócio ao invés da aplicação em si.

Ideal para desenvolvimento de aplicações CRUD, sites com painel de controle, etc.

## Recursos implementados

- Camada de Frontend e Backend separadas, sendo o frontend com Vue.js e o backend com Laravel
- CSS previamente configurado e disponível através do TailwindCSS
- Componentes de interface já implementados e documentados (layout, painéis, formulários, input)
- Integração com backend já implementada
- Sistema de autenticação já implementado e integrado ao Backend
- Documentação e padronização de código
- Testes automatizados

## Instalação
---

copie o arquivo .env

```shell
cp bp-backend/.env.example bp-backend/.env
```

inicie o docker

```shell
docker-compose up --build
```

> Após feita a instalação, acesse http://localhost:8000, clique em "Generate app key" para concluir a instalação do backend.

## Comandos básicos
---

Iniciar todas as aplicações do projeto

```shell
docker-compose up -d
```

Parar todas as aplicações do projeto

```shell
docker-compose down
```

Monitore os logs das aplicações

```shell
docker logs -f [nome do conteiner]
```

Acesse o contêiner da aplicação

```shell
docker exec -it [nome do conteiner] bash
```

### Nomes dos contêineres

- bp-frontend-playground
- bp-backend-playground
- bp-database
- bp-adminer

## Naming convention
Because we are autoloading the modules using psr-4, we strongly recommend using StudlyCase convention.
