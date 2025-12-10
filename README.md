# 📄 BACKEND (Node.js + Express + Prisma + MongoDB) — Cadastro de Usuários
<br>
Este é o backend do projeto Full Stack Cadastro de Usuários, responsável por gerenciar o CRUD de usuários utilizando **Node.js, Express, Prisma ORM e MongoDB (Atlas)**.

---

## 📌 Tecnologias Utilizadas

- Node.js

- Express

- Prisma ORM

- MongoDB (Atlas)

- CORS

---

## 📁 Funcionalidades

✔ Criar novos usuários

✔ Listar todos os usuários

✔ Excluir usuário

✔ Integração com Prisma ORM

✔ API REST completa

---

## 📡 Endpoints da API
#### 📍 GET /usuarios

Retorna a lista de todos os usuários cadastrados.

#### 📍 POST /usuarios

Cria um novo usuário.

#### 📍 PUT /usuarios/:id

Atualiza os dados de um usuário pelo ID.

#### 📍 DELETE /usuarios/:id

Remove um usuário do banco de dados.

---

## 🗄 Modelo de Dados (Prisma)
```prisma
model User {
  id    String @id @default(auto()) @map("_id") @db.ObjectId
  email String @unique
  name  String
  age   String
}
```

---

## 🚀 Como rodar o projeto
#### 1️⃣ Clonar o repositório:
```bash
git clone https://github.com/Gabriel-1812/Cadastro-de-Usuarios-backend.git
```

#### 2️⃣ Entrar na pasta do projeto:
```bash
cd Cadastro-de-Usuarios-backend
```

#### 3️⃣ Instalar as dependências:
```bash
npm install
```

#### 4️⃣ Configurar o arquivo .env
Crie um arquivo .env na raiz do projeto e coloque sua string do MongoDB Atlas:
```bash
DATABASE_URL="sua_string_do_mongodb_aqui"
```

#### 5️⃣ Rodar o servidor:
```bash
node server.js
```

O servidor irá iniciar na porta 3000:

http://localhost:3000


## 🔗 Conexão com o Frontend

Este backend foi criado para ser consumido pelo frontend em React:
👉 https://github.com/Gabriel-1812/Cadastro-de-Usuarios-frontend
