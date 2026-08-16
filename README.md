# :rocket: Minha Lista - Ponte de Login

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E" alt="JavaScript" />
  <img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black" alt="Firebase" />
  <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Vercel" />
</p>

> Uma aplicação web que funciona como ponte para realizar o login via Google de forma segura para o aplicativo desktop Minha Lista.

## :clipboard: Tabela de Conteúdos

- [Sobre](#-sobre)
- [Features](#-features)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Como Rodar](#-como-rodar)
- [Licença](#-licença)
- [Contato](#-contato)

---

## :book: Sobre

Este projeto foi desenvolvido para permitir a autenticação via OAuth (Google) no aplicativo desktop **Minha Lista**. Em muitas aplicações construídas para Desktop (como Electron, Tauri, ou scripts nativos), o uso de janelas de pop-up do Firebase de forma direta pode gerar erros de segurança ou limitações.

Por isso, essa página serve como um intermediário. O aplicativo desktop abre essa aplicação web no navegador principal do usuário, o login é efetuado através do Firebase (que verifica o token do Google), e em seguida a aplicação redireciona de volta para o aplicativo desktop passando os dados pela Deep Link (`minha-lista://callback`).

---

## :sparkles: Features

O que o projeto já faz?

- [x] Autenticação com o Google utilizando o Firebase Auth.
- [x] Interface limpa e minimalista.
- [x] Redirecionamento automático do navegador para o aplicativo Desktop (Deep Linking).
- [x] Tratamento de erros caso a autenticação falhe ou o usuário feche a janela sem confirmar.

---

## :computer: Tecnologias Utilizadas

As principais ferramentas, linguagens e bibliotecas usadas na construção do projeto:

- [HTML5 e CSS3 Vanilla](https://developer.mozilla.org/pt-BR/)
- [JavaScript](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript)
- [Firebase Auth](https://firebase.google.com/) (Google Authentication via pop-up)
- [Vercel](https://vercel.com/) (Hospedagem e configuração de rotas estáticas via `vercel.json`)

---

## :rocket: Como Rodar

### Pré-requisitos

Para abrir a aplicação, basta um navegador de internet moderno. Porém, para rodar localmente com propósito de desenvolvimento, será necessário:

- [Git](https://git-scm.com/)

### Instalação e Execução

Como este projeto é composto apenas por arquivos estáticos e HTML padrão, você não precisará rodar nenhum comando de build demorado:

1. Clone o repositório em sua máquina local:

```bash
git clone https://github.com/Lintzz/my-list-ponte-login.git
```

2. Você pode simplesmente abrir o arquivo `index.html` em qualquer navegador:

```bash
# Exemplo no Windows (via terminal)
start index.html
```

> **Nota de Desenvolvimento:** Se você for editar o projeto para usar suas próprias credenciais, lembre-se de atualizar o objeto `firebaseConfig` no código e adicionar seu domínio à aba de domínios autorizados no Console do Firebase Authentication.

---

## :page_facing_up: Licença

Este projeto está sob a licença [MIT](./LICENSE).

---

## :telephone_receiver: Contato

Alexandre Lintz - [alexandrelintz.1999@gmail.com](mailto:alexandrelintz.1999@gmail.com)

GitHub: [Lintzz](https://github.com/Lintzz)
