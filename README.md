<h1 align="center">
  🌐 Projeto Backend — Digital API
</h1>

<p align="center">
  Uma API RESTful desenvolvida para representar a base sólida de um sistema de e-commerce moderno, modular e escalável. Criada com amor por alguém que acredita no poder transformador da tecnologia.
</p>

<p align="center">
  <a href="#-sobre-o-projeto">Sobre</a> •
  <a href="#-funcionalidades">Funcionalidades</a> •
  <a href="#-tecnologias-utilizadas">Tecnologias</a> •
  <a href="#-estrutura-do-projeto">Estrutura</a> •
  <a href="#-como-executar">Como Executar</a> •
  <a href="#-autor">Agradecimentos</a>
</p>

---

## 💡 Sobre o Projeto

Este backend foi projetado como parte de um sistema completo de e-commerce, com foco em organização, segurança e escalabilidade. Desenvolvido com Node.js, Express e PostgreSQL, ele gerencia autenticação, produtos, usuários e categorias, servindo como base confiável para qualquer aplicação moderna.


## 🔥 Funcionalidades

- 🔐 Autenticação com JWT e criptografia de senhas com Bcrypt
- 👤 Cadastro, login e gerenciamento de usuários
- 🛍 Cadastro e filtragem de produtos por categorias, nome, preço, etc.
- 🗂 CRUD completo de categorias
- 🖼 Associação de imagens e variações aos produtos
- 🧱 Organização por camadas: controllers, services, middlewares, models e rotas
- 🐳 Docker-ready com banco PostgreSQL integrado
- 🧪 Estrutura para testes automatizados com Jest e Supertest


## 🛠 Tecnologias Utilizadas

- [Node.js](https://nodejs.org/)  
- [Express](https://expressjs.com/)  
- [Sequelize](https://sequelize.org/)  
- [PostgreSQL](https://www.postgresql.org/)  
- [JWT](https://jwt.io/)  
- [Bcrypt.js](https://github.com/dcodeIO/bcrypt.js)  
- [Docker](https://www.docker.com/)  
- [Jest](https://jestjs.io/) + [Supertest](https://github.com/visionmedia/supertest)  
- [Dotenv](https://www.npmjs.com/package/dotenv)  
- [CORS](https://developer.mozilla.org/pt-BR/docs/Web/HTTP/CORS)  


## 📁 Estrutura do Projeto

```bash
digital-api/
├── src/
│   ├── config/         # Configurações de ambiente e banco de dados
│   ├── controllers/    # Camada responsável por receber e responder requisições
│   ├── middleware/     # Interceptadores de requisições (ex: autenticação)
│   ├── models/         # Definições dos modelos (Sequelize)
│   ├── routes/         # Mapeamento das rotas da API
│   ├── services/       # Regras de negócio reutilizáveis
│   ├── database/       # Migrations, seeds e conexão
│   ├── app.js          # Instância e configuração do Express
│   └── server.js       # Ponto de entrada da aplicação
├── .env                # Variáveis de ambiente
├── .gitignore          # Arquivos e pastas ignorados pelo Git
├── package.json        # Dependências e scripts do projeto
└── README.md           # Documentação do projeto
```

## 🚀 Como Executar

### Pré-requisitos

- Node.js 16+
- Docker (opcional, para PostgreSQL)
- NPM ou Yarn

### Passos

```bash
# Clone o repositório
git clone https://github.com/jsolo84work/digital-store-backend.git

# Acesse a pasta
cd digital-api

# Instale as dependências
npm install

# Configure o arquivo .env baseado no .env.example
cp .env.example .env

# Inicie o container PostgreSQL (opcional)
docker run --name db-digital -e POSTGRES_PASSWORD=docker -e POSTGRES_USER=docker -e POSTGRES_DB=digital_db -p 5432:5432 -d postgres

# Rode as migrations e inicie o servidor
npm run dev
```

---

## 🙏 Agradecimentos

A realização deste projeto só foi possível graças ao apoio e incentivo da Geração Tech e às ferramentas que facilitaram todo o processo de desenvolvimento. A cada linha de código, houve também aprendizado, dedicação e paixão.

A todos que acreditam no poder da criação digital, à comunidade de Desenvolvedores que compartilham conhecimento diariamente — e à você, que chegou até aqui: Obrigado! 💡

Deixo também, um agradecimento mais que especial para:

👏  *Prof. Luan Oliveira*
    https://github.com/in100tiva

👏  *Nazaré Almeida*
    https://github.com/nazare4lmeida

---

Desenvolvido por *JulianSolo*.
Atualização em: 30/06/2025.