# 🎬 Movies Controll (Controle de Filmes e Séries)

## 📖 Sobre o Projeto

O **Movies Controll** é uma aplicação full-stack desenvolvida como parte de um desafio prático da **[Digital Innovation One (DIO)](https://dio.me)**.

O objetivo principal do projeto é aplicar a modelagem e estruturação de um banco de dados relacional a partir de um problema real — o controle pessoal de filmes e séries assistidos — integrando uma API back-end em **Node.js** com uma interface front-end em **React** para exibição e gerenciamento dos registros.

---

## ✨ Funcionalidades

- **Modelagem de Dados Relacional:** Estruturação de tabelas e relacionamentos para armazenar títulos (filmes ou séries), quantidade de episódios assistidos, total de episódios e data da última visualização.
- **Listagem de Filmes e Séries:** Exibição organizada em tabela dos conteúdos cadastrados no banco de dados.
- **Integração Full-Stack:** Comunicação entre o front-end React e a API REST no back-end para consulta e manipulação dos dados.

---

## 🛠️ Tecnologias Utilizadas

Com base na estrutura do repositório (`backend` e `frontend`), a stack do projeto envolve:

### Back-end (`/backend`)
- **[Node.js](https://nodejs.org):** Ambiente de execução JavaScript no lado do servidor.
- **[Express](https://expressjs.com):** Framework para criação das rotas e endpoints da API REST.
- **[MySQL](https://mysql.com) (`mysql` / `mysql2`):** Banco de dados relacional utilizado para persistir as informações dos filmes e séries.
- **CORS:** Middleware para permitir a comunicação segura entre o front-end e o back-end em portas diferentes.

### Front-end (`/frontend`)
- **[React](https://react.dev):** Biblioteca JavaScript para construção da interface de usuário.
- **[Bootstrap](https://getbootstrap.com) / CSS3:** Estilização e layout responsivo das tabelas e componentes.
- **Fetch API / Axios:** Consumo dos endpoints disponibilizados pelo back-end.

---

## 📂 Estrutura de Diretórios

```text
movies-controll/
├── backend/              # API Node.js, conexão com o banco de dados, rotas e scripts SQL
├── frontend/             # Aplicação React com os componentes de listagem e interface visual
└── README.md             # Documentação do projeto
```

---

## 🚀 Como Executar o Projeto na Sua Máquina

Como o projeto é dividido em **Back-end** e **Front-end**, você precisará configurar o banco de dados e rodar ambos os servidores simultaneamente (em dois terminais diferentes).

### Pré-requisitos

Certifique-se de ter instalado em sua máquina:
- **[Node.js](https://nodejs.org)** (versão LTS recomendada) e **npm** (ou **Yarn**)
- **[MySQL Server](https://mysql.com)** (ou pacotes como XAMPP, WAMP ou Docker com MySQL)
- **[Git](https://git-scm.com)**

---

### Passo 1: Clonar o Repositório

```bash
git clone https://github.com
cd movies-controll
```

---

### Passo 2: Configurar o Banco de Dados (MySQL)

1. Certifique-se de que o serviço do **MySQL** esteja em execução na sua máquina.
2. Abra o seu cliente MySQL (MySQL Workbench, DBeaver, phpMyAdmin ou terminal) e crie o banco de dados conforme o script SQL localizado na pasta `backend/` (ex.: `CREATE DATABASE movies_controll;`).
3. Execute as queries de criação de tabela (`CREATE TABLE`) e inserção inicial (`INSERT INTO`), caso disponíveis no arquivo `.sql` dentro de `backend/`.

---

### Passo 3: Configurar e Rodar o Back-end

1. Abra um terminal e acesse a pasta `backend`:
   ```bash
   cd backend
   ```

2. Instale as dependências:
   ```bash
   npm install
   ```

3. **Configure as credenciais do banco:**
   Verifique o arquivo de conexão com o banco de dados dentro de `backend/` (geralmente `database/connection.js`, `db.js` ou `.env`) e ajuste o **usuário** (`user`), **senha** (`password`), **host** (`localhost`) e **nome do banco** (`database`) de acordo com o seu ambiente MySQL local.

4. Inicie o servidor back-end:
   ```bash
   npm start
   ```
   *(O servidor da API geralmente inicia na porta `5000` ou `3001` — confira a mensagem exibida no terminal).*

---

### Passo 4: Configurar e Rodar o Front-end

1. Abra um **segundo terminal**, volte à raiz do projeto e entre na pasta `frontend`:
   ```bash
   cd frontend
   ```

2. Instale as dependências:
   ```bash
   npm install
   ```

3. **Verifique a URL da API (se necessário):**
   Confirme dentro de `frontend/src/` se o endereço das requisições HTTP aponta para a mesma porta em que o seu back-end está rodando (ex.: `http://localhost:5000/movies`).

4. Inicie a aplicação React:
   ```bash
   npm start
   ```

5. **Acesse no navegador:**
   Abra `http://localhost:3000/` para visualizar e interagir com o sistema.

---

## 🤝 Contribuição

Contribuições são sempre bem-vindas! Se você quiser melhorar este projeto:

1. Faça um **Fork** do repositório.
2. Crie uma **Branch** para sua melhoria (`git checkout -b feature/NovaFuncionalidade`).
3. Faça o **Commit** das suas alterações (`git commit -m 'Adiciona nova funcionalidade'`).
4. Faça o **Push** para a branch (`git push origin feature/NovaFuncionalidade`).
5. Abra um **Pull Request**.

---

## 👨‍💻 Autor

Desenvolvido por **[marceloxm](https://github.com/marceloxm)** durante os estudos na **Digital Innovation One (DIO)**.

