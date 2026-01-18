# 🚀 API REST com Node.js

> Repositório de estudos do Módulo 2 do curso de Node.js da Rocketseat

## 📋 Sobre

Este repositório foi criado exclusivamente para fins educacionais, contendo os códigos e exercícios desenvolvidos durante as aulas do **Módulo 2** do curso de Node.js da **Rocketseat**. O objetivo é aplicar os conceitos de desenvolvimento de APIs RESTful utilizando Node.js e suas principais ferramentas do ecossistema.

## 🛠️ Tecnologias

Este projeto foi desenvolvido com as seguintes tecnologias:

- **[Node.js](https://nodejs.org/)** - Ambiente de execução JavaScript
- **[TypeScript](https://www.typescriptlang.org/)** - Superset JavaScript com tipagem estática
- **[Fastify](https://www.fastify.io/)** - Framework web rápido e eficiente
- **[Knex.js](http://knexjs.org/)** - Query builder SQL
- **[SQLite](https://www.sqlite.org/)** - Banco de dados relacional
- **[TSX](https://github.com/esbuild-kit/tsx)** - Executor TypeScript para Node.js
- **[ESLint](https://eslint.org/)** - Linter para padronização de código

## 🚀 Como executar

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/02-api-rest-nodejs.git

# Entre na pasta do projeto
cd 02-api-rest-nodejs

# Instale as dependências
npm install

# Execute o projeto em modo de desenvolvimento
npm run dev
```

## �️ Migrations

**Migrations** são arquivos que controlam as mudanças no esquema do banco de dados de forma versionada. Elas funcionam como um histórico de alterações, permitindo que você crie, modifique ou delete tabelas e colunas de maneira organizada e rastreável.

### Por que usar Migrations?

- **Versionamento**: Mantém um histórico de todas as alterações no banco de dados
- **Reversibilidade**: Permite desfazer mudanças caso necessário
- **Colaboração**: Facilita o trabalho em equipe, pois todos têm a mesma estrutura de banco
- **Ambiente**: Garante que desenvolvimento, homologação e produção tenham a mesma estrutura

### Executando as Migrations

Para executar todas as migrations: 

```bash
# Executar todas as migrations
npm run knex -- migrate:latest
```

Para criar uma nova migration:

```bash
# Criar uma nova migration
npm run knex -- migrate:make nome-da-migration
```

Para desfazer a última migration executada:

```bash
# Desfazer a última migration
npm run knex -- migrate:rollback
```

### Localização das Migrations

As migrations deste projeto estão armazenadas na pasta:

```
📁 db/
  └── 📁 migrations/
      └── 20260118194457_create-documents.ts
```

Todos os arquivos de migration devem ser criados na pasta `db/migrations/` e seguirão o padrão de nomenclatura com timestamp automático.

## �📚 Aprendizados

Durante este módulo, foram abordados os seguintes tópicos:

- Criação de APIs RESTful
- Utilização do Fastify
- Configuração de banco de dados com Knex.js
- Migrations e queries SQL
- Boas práticas com TypeScript
- Padronização de código com ESLint

## 📝 Licença

Este projeto é apenas para fins de estudo e aprendizado.

---

Desenvolvido durante o curso de Node.js da [Rocketseat](https://www.rocketseat.com.br) 💜
