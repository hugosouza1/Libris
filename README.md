
# Libris

Plataforma web desenvolvida para conectar leitores, permitindo o acompanhamento de leituras, interação social por meio de resenhas e comentários, e a descoberta de novas obras literárias.

---

Aplicação web desenvolvida com Next.js 16, React 19, Tailwind CSS v4 e Prisma ORM, contando com autenticação via NextAuth.js (v5).


## Tecnologias Utilizadas

* **Framework Web:** Next.js 16 (App Router)
* **Interface e Estilização:** React 19, Tailwind CSS v4, Lucide React, Radix UI, Recharts
* **Banco de Dados e ORM:** PostgreSQL (`@prisma/adapter-pg`), Prisma ORM
* **Autenticação e Segurança:** NextAuth.js (v5), `@auth/prisma-adapter`, bcryptjs
* **Linguagem:** TypeScript

---

## Como Executar o Projeto

### Pré-requisitos

* **Node.js** (versão 20 ou superior recomendada)
* **npm**, **pnpm** ou **yarn**
* Instância do **PostgreSQL** em execução

### 1. Clonar o Repositório

```bash
git clone https://github.com/hugosouza1/Libris.git
cd Libris

```

### 2. Instalar as Dependências

```bash
npm install

```

### 3. Configurar Variáveis de Ambiente

Crie um arquivo `.env` na raiz do projeto com as credenciais do banco de dados e segredos da aplicação:

```env
DATABASE_URL="postgresql://usuario:senha@localhost:5432/nome_do_banco?schema=public"
AUTH_SECRET="seu_secret_aqui"

```

### 4. Executar as Migrações do Prisma

```bash
npx prisma migrate dev

```

### 5. Iniciar o Servidor de Desenvolvimento

```bash
npm run dev

```

Acesse [http://localhost:3000](http://localhost:3000) no seu navegador para ver a aplicação em execução.

---

## Scripts Disponíveis

* `npm run dev` - Inicia o ambiente de desenvolvimento.
* `npm run build` - Cria a compilação otimizada para produção.
* `npm run start` - Inicia o servidor em modo de produção.

---

## Banco de Dados e Diagramas

O projeto inclui o `prisma-erd-generator` e o `@mermaid-js/mermaid-cli` configurados. Para gerar visualizações do diagrama de entidade-relacionamento do banco de dados, execute:

```bash
npx prisma generate

```
