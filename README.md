# MySQL and Mongodb Docker Container Setup

Este repositório contém instruções para configurar e executar um banco de dados MySQL dentro de um container Docker, assim como um banco de dados Mongodb, conforme solicitado no desafio do módulo de Docker do curso devopspro.  Siga estes passos para colocar os containers em funcionamento.

## Pré-requisitos

- [Docker](https://www.docker.com/get-started) instalado na sua máquina
- Conhecimento básico de operações de linha de comando

## Para criar o banco de dados MySQL:

Abra seu terminal e execute o seguinte comando:

```bash
docker container run -d -p 3306:3306 -e MYSQL_ROOT_PASSWORD="root" -e MYSQL_DATABASE="docker_db" -e MYSQL_USER="docker_usr" -e MYSQL_PASSWORD="docker_pwd" mysql
```

## Para criar o banco de dados Mongodb:

Abra seu terminal e execute o seguinte comando:

```bash
docker container run -d -p 27017:27017 -e MONGO_INITDB_ROOT_USERNAME=mongo_usr -e MONGO_INITDB_ROOT_PASSWORD=mongo_pwd mongo
```
