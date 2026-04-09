# 🔌 QA — Testes de API com Postman

Coleção de testes de API REST desenvolvidos com Postman, cobrindo os principais verbos HTTP (GET, POST, PUT, PATCH, DELETE) com validações automatizadas de status code, contrato e dados de resposta.

API testada: **Restful Booker** — ambiente público de prática para QA.

---

## 📋 Cobertura de Testes

| Método | Endpoint | Descrição | Validações |
|--------|----------|-----------|-----------|
| GET | `/booking` | Listar todas as reservas | Status 200, array não vazio |
| GET | `/booking/:id` | Buscar reserva por ID | Status 200, campos obrigatórios |
| POST | `/booking` | Criar nova reserva | Status 200, ID gerado |
| PUT | `/booking/:id` | Atualizar reserva completa | Status 200, dados atualizados |
| PATCH | `/booking/:id` | Atualizar reserva parcial | Status 200, campo atualizado |
| DELETE | `/booking/:id` | Deletar reserva | Status 201 |
| POST | `/auth` | Gerar token de autenticação | Status 200, token gerado |

---

## 📁 Estrutura do Repositório

```
qa-testes-api/
├── collections/
│   └── Restful-Booker.postman_collection.json
├── environments/
│   └── restful-booker-env.postman_environment.json
├── evidencias/
│   └── README.md
└── README.md
```

---

## 🚀 Como executar

### Importar no Postman
1. Abra o Postman
2. Clique em **Import**
3. Selecione o arquivo `collections/Restful-Booker.postman_collection.json`
4. Importe também o ambiente `environments/restful-booker-env.postman_environment.json`
5. Selecione o ambiente **Restful Booker** no canto superior direito
6. Execute a coleção completa com **Run collection**

---

## 🌐 API testada

**Restful Booker** — [restful-booker.herokuapp.com](https://restful-booker.herokuapp.com/apidoc)

API pública para prática de testes, sem necessidade de cadastro.

---

## 🛠️ Ferramentas

- **Postman** — criação e execução dos testes
- **JavaScript** — scripts de validação (Tests)

---

## 👤 Autor

**Mateus Alves da Cruz**
Analista de QA | Pinhais, PR

[![LinkedIn](https://img.shields.io/badge/LinkedIn-mateus--cruz10-blue?logo=linkedin)](https://www.linkedin.com/in/mateus-cruz10)
