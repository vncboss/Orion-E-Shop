# 🚀 Orion E-Shop: Plataforma de E-commerce Full-Stack

![Banner do Orion E-Shop](https://i.imgur.com/L1ryb2x.png)

## 📄 Sobre o Projeto

Orion E-Shop é uma simulação de uma plataforma de e-commerce moderna e completa, construída para demonstrar habilidades em desenvolvimento full-stack. A aplicação inclui funcionalidades essenciais como galeria de produtos, página de detalhes, carrinho de compras e uma API REST para gerenciar os dados.

Este projeto foi desenvolvido como parte do meu portfólio pessoal para aplicar e demonstrar conhecimentos em arquiteturas baseadas em Node.js e React.

---

## 🛠️ Tecnologias Utilizadas

O projeto foi construído utilizando as seguintes tecnologias:

-   **Frontend:**
    -   React.js
    -   Redux & Redux Thunk (para gerenciamento de estado)
    -   React Router (para navegação)
    -   Axios (para chamadas à API)
-   **Backend:**
    -   Node.js
    -   Express.js (para criação da API REST)
    -   MongoDB (banco de dados NoSQL)
    -   Mongoose (para modelagem dos dados)
-   **Ferramentas:**
    -   JSON Web Tokens (JWT) para autenticação (funcionalidade futura)
    -   Dotenv para gerenciamento de variáveis de ambiente
    -   CORS

---

## 🏛️ Arquitetura

A aplicação segue uma arquitetura de microsserviços desacoplada, com um backend que expõe uma API REST e um frontend que a consome.

![Fluxo da Arquitetura MERN]

1.  **Frontend (React):** O usuário interage com a interface. Uma ação (ex: carregar a página de produtos) é despachada pelo Redux.
2.  **Redux Thunk:** Permite que a ação faça uma chamada assíncrona para a API usando o Axios.
3.  **Backend (Node/Express):** Recebe a requisição na rota correspondente (ex: `/api/products`).
4.  **Controller:** Executa a lógica de negócio, utilizando o Mongoose para consultar o banco de dados.
5.  **MongoDB:** Retorna os dados solicitados para o backend.
6.  **Resposta da API:** O backend envia os dados em formato JSON de volta para o frontend.
7.  **Redux Store:** A ação de sucesso é despachada, e o Reducer atualiza o estado global com os novos dados.
8.  **React UI:** O componente React, conectado à store, re-renderiza automaticamente para exibir os dados atualizados ao usuário.

---

## ⚙️ Como Executar o Projeto

```bash
# Clone este repositório
$ git clone [https://github.com/SEU-USUARIO/Orion-E-Shop.git](https://github.com/SEU-USUARIO/Orion-E-Shop.git)

# Instale as dependências do Backend
$ cd Orion-E-Shop/Orion-E-Shop-Backend
$ npm install

# Inicie o servidor do Backend
$ npm start

# Instale as dependências do Frontend
$ cd ../Orion-E-Shop-Frontend
$ npm install

# Inicie o cliente Frontend
$ npm start
