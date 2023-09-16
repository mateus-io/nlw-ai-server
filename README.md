## 🚀 Setup Development Envirtonment

- #### Pré-requisitos:

###### Docker Instalado
###### Docker Compose Instalado

- #### Serviços:

| App | Porta |
| ----------- | ----------- |
| PGAdmin | 5050 |
| PostgreSQL | 5432 |
| App | 3333 |

- #### 1º Passo:

#### Criar uma rede:

> ⚠️ Importante: Por segurança antes de criar a rede verifique se ela já não existe usando:
> <code> docker network ls </code>
> Caso ocorra algum problema com a rede, tente deletar ela e criar novamente usando:
> <code> docker network rm mynetwork </code>
> e
> <code> docker network create --driver=bridge --subnet=172.14.0.0/16 mynetwork </code>

- #### 2º Passo:

#### Navegar até a pasta docker

Na raiz do projeto, use:

<code> cd docker </code>

- #### 3º Passo:

#### Iniciar os serviços

<code> docker-compose up </code>

> ⚠️ OBS: Use a flag `--force-recreate`, caso dê `network not found` com a rede já criada
> <code> docker-compose up --force-recreate </code>


