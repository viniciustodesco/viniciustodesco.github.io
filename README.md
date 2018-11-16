# Node.js Alpe API &nbsp;

Alpe API  **Portal Financeiro** desenvolvido em **[Node.js][node]** com banco de dados 
**[Postgres][postgres]**.

<p align="center"><a href="https://www.postgresql.org"><img src="https://www.postgresql.org/media/img/about/press/elephant.png" height="24" align="top" /></a> 
<sup><a href="https://nodejs.org/static/images/logo.svg">Node.js</a></sup></p>


---

## Tech Stack

* [Docker][docker], [Node.js][node], [JavaScript][js], [Babel][babel], [Winston][winston] — core platform and dev tools
* [Restify][restify],[session][session], etc. — common HTTP-server features
* [PostgreSQL][pg], [Oracledb] [oracledb] — SQL data acess and migrations
* [mocha][mocha] - testing

## Directory Layout

```bash
.
├── /postman/                   # Documentação das APIs (POSTMAN)
├── /scripts/                   # Scripts do banco de dados  seed/migrations
├── /src/                       # Node.js application source files
│   ├── /controllers/
│   ├── /environment/
│   ├── /model/
│   ├── /app-dev-seed.js
│   ├── /app-dev.js
│   ├── /app.js
├── /test
├── docker-compose.yml          # Defines Docker services, networks and volumes
├── docker-compose.override.yml # Overrides per developer environment (not under source control)
├── Dockerfile                  # Commands for building a Docker image for production
├── package.json                # List of project dependencies
```


## Prerequisites

* [Node.Js][node] Necessário utilizar a versão `v10.13.0`
* [Docker][docker] Community Edition v17 ou mair
* [VS Code][code] editor (preferido), [ESLint][vceslint] plug-ins.
* [Postgres][postgres] Banco de dados.


## Getting Started

* Verificar se a versão do node está em `v10.13.0`.
* Clonar o repositório e rodar `npm i`

- Setup banco de dados
* Necessário utilizar: 
    * Usuário **postgres** 
    * Senha **sa**
* Criar banco com o nome **alpe**

```bash
git clone https://github.com/ITLAB-BR/alpe-api.git alpe-api
cd alpe-api                  # Alterar para o diretório do projeto
npm i                        # Instalar as dependências
gulp start-dev               # Rodar o projeto
```

## Testing



## Projetos Relacionados

* [Front-End](https://github.com/ITLAB-BR/alpe-bko) —  Repositório código-fonte Front-End (www) 
* [Integração](https://github.com/ITLAB-BR/alpe-api-integracao) — Gateway de integração 
* [Documentação](https://github.com/ITLAB-BR/alpe) — Documentação/Backlog/Sprints
* [API](https://github.com/ITLAB-BR/alpe-api) — Repositório código-fonte Back-End (API)

---
Feito com ♥ por ITLAB (http://www.itlab.com.br)

[winston]: https://github.com/winstonjs/winston
[node]: https://nodejs.org
[js]: https://developer.mozilla.org/docs/Web/JavaScript
[babel]: http://babeljs.io/
[postgres]: https://www.postgresql.org/
[restify]: http://restify.com/
[pg]: https://www.postgresql.org/
[nodepg]: https://github.com/brianc/node-postgres
[psql]: https://www.postgresql.org/docs/current/static/app-psql.html
[code]: https://code.visualstudio.com/
[oracledb]:https://github.com/oracle/node-oracledb
[docker]: https://www.docker.com/community-edition
[compose]: https://docs.docker.com/compose/
[mocha]:https://mochajs.org
