# 🚀 API de Cadastro de Usuários

API REST desenvolvida com Node.js, Express e Prisma para gerenciamento de usuários, preparada para deploy serverless na Vercel.

---

## 📌 Tecnologias utilizadas

* Node.js
* Express
* Prisma ORM
* Mongodb
* Vercel (Serverless Functions)

---

## 📁 Estrutura do projeto

```
/api
  index.js          # Entry point para Vercel
/prisma
  schema.prisma     # Configuração do banco de dados
/server.js          # Configuração principal da API
/vercel.json        # Configuração de rotas da Vercel
/package.json
```

---

## ⚙️ Configuração do ambiente

### 1. Clone o repositório

```
git clone https://github.com/seu-usuario/seu-repo.git
cd seu-repo
```

---

### 2. Instale as dependências

```
npm install
```

---

### 3. Configure as variáveis de ambiente

Crie um arquivo `.env` na raiz:

```
DATABASE_URL="mongodb+srv://user:password@users.1obrpuc.mongodb.net/Nome-da-base?appName=Nome-da-base"
```

---

### 4. Gere o Prisma Client

```
npx prisma generate
```

---

### 5. Execute localmente

```
npm run dev
```

---

## 🌐 Rotas da API

### 📍 Listar usuários

```
GET /users
```

### 📍 Criar usuário

```
POST /users
```

### 📍 Atualizar usuário

```
PUT /users/:id
```

### 📍 Deletar usuário

```
DELETE /users/:id
```

---

## ☁️ Deploy na Vercel

### 1. Suba o projeto para o GitHub

### 2. Acesse a Vercel e importe o repositório

### 3. Configure a variável de ambiente:

```
DATABASE_URL=...
```

### 4. Deploy automático 🚀

---

## ⚠️ Observações importantes

* A aplicação foi adaptada para ambiente serverless (sem `app.listen`)
* O Prisma utiliza a variável `DATABASE_URL` definida no ambiente
* Recomendado uso de banco com suporte a conexão serverless (ex: Neon, Supabase)

---

## 🧠 Boas práticas aplicadas

* Separação de responsabilidades
* Uso de ORM (Prisma)
* Configuração para ambiente serverless
* Variáveis de ambiente para segurança

---

## 📄 Licença

Este projeto está sob a licença MIT.

---

## 👨‍💻 Autor

Thiago Mendes
