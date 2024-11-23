# 🛒 Shopyy - Loja Online

**Shopyy** é um e-commerce moderno com funcionalidades completas, incluindo cadastro de usuários, gerenciamento de produtos, carrinho de compras e uma interface administrativa para gerenciar o sistema.

---

## 📖 Descrição do Projeto

O **Shopyy** foi desenvolvido com foco na usabilidade e escalabilidade, permitindo que usuários naveguem por produtos, adicionem itens ao carrinho e realizem pagamentos de forma segura. Além disso, administradores têm controle total sobre o catálogo de produtos e gerenciamento de pedidos.

### **Funcionalidades Principais**
- Cadastro e login de usuários.
- Listagem de produtos com filtros e detalhamento.
- Carrinho de compras dinâmico.
- Sistema de checkout com integração à API do **Stripe** para pagamentos.
- Tela de administrador para gerenciar produtos, pedidos e usuários.

---

## 🛠️ Tecnologias Utilizadas

- **Frontend**:
  - React
  - Redux Toolkit (para gerenciamento de estado)
  - Axios (para consumo de APIs)

- **Backend**:
  - Node.js
  - Express (API REST)

- **Banco de Dados**:
  - MongoDB
  - Mongoose (para integração com o MongoDB)

- **Pagamento**:
  - Stripe API

---

## 🚀 Como Executar o Projeto

### Pré-requisitos
Certifique-se de ter as seguintes ferramentas instaladas:
- [Node.js](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/)
- Uma conta no [Stripe](https://stripe.com/)

### 1. Clone o Repositório
```bash
git clone https://github.com/Roberto-BR29/deploy-projeto-webII.git
cd deploy-projeto-webII
```

### 2. Configuração do Backend

   1.Acesse o diretório backend:
   
   ```bash
     cd backend
   ```

  2.Instale as dependências:
  
   ```bash
     npm install
   ```

  3.Crie um arquivo .env com as variáveis de ambiente:
  
   ```bash
     PORT=5000
     MONGO_URI=sua-url-do-mongodb
     JWT_SECRET=sua-chave-secreta
     STRIPE_SECRET_KEY=sua-chave-stripe
   ```

  4.Inicie o servidor:
  
   ```bash
     npm start
   ```


### 3.Configuração do Frontend

  1.Acesse o diretório frontend:
  
   ```bash
     cd ../frontend
   ```

  2.Instale as dependências:
  
   ```bash
     npm install
   ```

  3.Inicie o servidor:
  
   ```bash
     npm start
   ```

O frontend será acessível em http://localhost:3000 e o backend em http://localhost:5000.

deploy-projeto-webII/
├── backend/
│   ├── models/         # Modelos do MongoDB
│   ├── routes/         # Rotas da API
│   ├── controllers/    # Lógica de controle
│   ├── config/         # Configurações (banco de dados, Stripe)
│   ├── middleware/     # Middlewares de autenticação
│   └── server.js       # Configuração do servidor
├── frontend/
│   ├── src/
│   │   ├── components/ # Componentes reutilizáveis
│   │   ├── pages/      # Páginas do aplicativo
│   │   ├── redux/      # Configuração do Redux Toolkit
│   │   ├── App.js      # Configuração principal do React
│   └── public/         # Arquivos estáticos
└── README.md           # Documentação

