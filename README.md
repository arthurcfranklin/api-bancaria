# 🏦 API Bancária Assíncrona com FastAPI

API RESTful desenvolvida com **FastAPI** para simular operações bancárias básicas, como **depósitos**, **saques** e **consulta de extrato**, utilizando **boas práticas de design de APIs**, validações de regras de negócio e **autenticação com JWT**.

Projeto desenvolvido com foco em **aprendizado prático de backend**, organização de código e estrutura profissional para portfólio.

---

## 🚀 Tecnologias Utilizadas

- **Python 3.10+**
- **FastAPI**
- **SQLAlchemy**
- **SQLite** (ambiente de desenvolvimento)
- **JWT (JSON Web Token)**
- **Pydantic**
- **Uvicorn**

---

## 📌 Funcionalidades

- ✔ Cadastro de transações bancárias (depósito e saque)
- 🔒 Validação de regras de negócio
  - 🚫 Não permite valores negativos
  - 🚫 Não permite saque sem saldo suficiente
- ✔ Atualização automática de saldo da conta
- ✔ Consulta de extrato bancário
- ✔ Autenticação segura utilizando JWT
- ✔ Documentação automática via OpenAPI (Swagger)



---

## 📂 Estrutura do Projeto

```
app/
├── main.py
├── core/
│   └── security.py
├── database/
│   ├── base.py
│   └── session.py
├── models/
│   ├── user.py
│   ├── account.py
│   └── transaction.py
├── schemas/
│   └── transaction.py
├── services/
│   └── transaction_service.py
└── routes/
    └── transactions.py
```

## ▶️ Como Executar o Projeto

### 1️⃣ Clone o repositório

```
git clone https://github.com/SEU_USUARIO/banking-api.git
cd banking-api
```

### 2️⃣ Crie e ative o ambiente virtual

```
python -m venv venv
```

* 🪟 Windows: `source venv/bin/activate`

* 🐧 Linux: `source venv/bin/activate`

* 🍎 MacOS: `source venv/bin/activate`


### 3️⃣ Instale as dependências
```
pip install -r requirements.txt
```


### 4️⃣ Execute a aplicação
```
uvicorn app.main:app --reload
```
---
## 📖 Documentação da API

Após iniciar o servidor, acesse:

👉 Swagger UI:
`http://localhost:8000/docs`

👉Redoc:
`http://localhost:8000/redoc`

---
## 🔐 Autenticação

A API utiliza JWT (JSON Web Token) para proteger os endpoints sensíveis.
O token deve ser enviado no header:

---
## 🧪 Status do Projeto

#### 📌 Em desenvolvimento
- Novas funcionalidades serão adicionadas, como:
- Autenticação completa de usuários
- Associação real de contas por usuário
- Testes automatizados
- Persistência em banco relacional (PostgreSQL)
- Dockerização

---
## 📄 Licença

Este projeto está sob a licença MIT.
Sinta-se à vontade para estudar, utilizar e adaptar.

---
