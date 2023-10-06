## Coleção de Bancos de Dados para estudos

#### No momento, os bancos contidos na lista são:
- PostgreSQL
- MySQL (v.8)
- Redis
- MongoDB
- Apache Cassandra

## Como utilizar:

Para utilizar os BDs, você precisa ter o Docker instalado no seu computador.
Presumo que já tenha um mínimo de conhecimento em Docker, então, não ensinarei como usá-lo.

- Clone o projeto para o local de sua preferência.
- Entre na pasta "databases" (ou o nome que você escolheu, caso tenha alterado durante a clonagem).
- Digite o comando "docker-compose up -d" e aguarde que as imagens sejam baixadas e executadas.

Todos os bancos são independentes (não possuem network configurada), bastando usar o endereço padrão "localhost" e as portas específicas de cada um para se conectar. Atenção com usuário e senha!

### PostgreSQL:
- Porta: 5432
- Usuário: postgres
- Senha: postgres
- Obs: Nenhuma base padrão é criada, está totalmente limpo para você iniciar os estudos.

### MySQL:
- Porta: 3306
- Usuário: aluno
- Senha: 1234
- Obs: Uma base de dados com o nome "estudo_uninove" é criada por padrão, mas está vazia. Você pode criar tabelas ou sua própria base de dados.

### Redis:
- Porta: 6379
- Usuário e senha: A Autenticação foi desabilitada (pode executar tudo direto)
- Obs: Inicie com o comando "redis-cli" e depois digite "ping". Se tudo estiver correto, o Redis responderá "PONG", agora é só estudar!

### MongoDB:
- Porta: 27017
- Usuário e senha: A Autenticação foi desabilitada (pode executar tudo direto)
- Obs: Existem vários softwares diferentes para se conectar no MongoDB. Eu indico o [NoSQL Booster](https://nosqlbooster.com/downloads), tem versão grátis e você vai conseguir fazer o que quiser durante os estudos.

### Cassandra:
- Porta: 9042
- Usuário e senha: A Autenticação foi desabilitada (pode executar tudo direto)
- Obs: Você precisa acessar o CLI do container para usar. Ainda não encontrei um software tipo DBeaver para poder conectar no Cassandra e manipulá-lo, apesar de você poder usá-lo com Spark e NiFi (não inclusos!)


## Considerações:

Pretendo incrementar o projeto, incluindo mais ferramentas, como phpmyadmin, pgadmin, cassandra-web e outros, bem como outros bancos de dados relacionais e nosql.