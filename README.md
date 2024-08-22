# Center-Repository-Tales-Store

## Ideia

O objetivo deste projeto é criar um repositório central que integre diversos serviços relacionados à loja fictícia "Tales Store". O projeto inclui:

- **API RESTful em Go** para gerenciar produtos.
- **Microserviço de Processamento de Pagamentos em Rust** para processar transações.
- **Frontend em Next.js** para a interface do usuário.

## Estrutura do Projeto

Este repositório é dividido em três partes principais:

1. **API RESTful em Go**: Gerencia produtos na loja.
2. **Microserviço de Processamento de Pagamentos em Rust**: Gerencia e processa transações de pagamento.
3. **Frontend em Next.js**: Interface do usuário para interagir com a loja.

## Componentes

### 1. API RESTful em Go

- **Descrição**: API para gerenciar produtos na loja, incluindo operações de CRUD (criar, ler, atualizar e deletar).
- **Tecnologia**: Go com o framework Gin.

### 2. Microserviço de Processamento de Pagamentos em Rust

- **Descrição**: Serviço responsável por processar pagamentos.
- **Tecnologia**: Rust.

### 3. Frontend em Next.js

- **Descrição**: Interface do usuário para interagir com a loja, exibindo produtos e permitindo transações.
- **Tecnologia**: Next.js com React.

## Requisitos

Antes de começar, verifique se você tem os seguintes softwares instalados:

- [Go](https://golang.org/doc/install) (v1.18 ou superior)
- [Rust](https://www.rust-lang.org/learn/get-started) (v1.60 ou superior)
- [Node.js](https://nodejs.org/en/download/) (v16 ou superior)
- [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

## Instalação

### API RESTful em Go

1. Clone o repositório:

    ```bash
    git clone https://github.com/seu-usuario/center-repository-tales-store.git
    cd center-repository-tales-store/api
    ```

2. Instale as dependências:

    ```bash
    go mod tidy
    ```

3. Para rodar a API, use o comando:

    ```bash
    go run main.go
    ```

    Por padrão, a API será iniciada na porta `8080`.

### Microserviço de Processamento de Pagamentos em Rust

1. Navegue para o diretório do microserviço:

    ```bash
    cd center-repository-tales-store/payment-service
    ```

2. Compile e rode o microserviço:

    ```bash
    cargo build
    cargo run
    ```

    O microserviço será iniciado na porta `8081` por padrão. A porta pode ser configurada no arquivo de configuração do microserviço.

### Frontend em Next.js

1. Navegue para o diretório do frontend:

    ```bash
    cd center-repository-tales-store/frontend
    ```

2. Instale as dependências:

    ```bash
    npm install
    ```

3. Para rodar o frontend, use o comando:

    ```bash
    npm run dev
    ```

    O frontend será iniciado na porta `3000` por padrão.

## Endpoints da API

Aqui estão alguns dos endpoints disponíveis na API:

- `GET /products` - Lista todos os produtos.
- `GET /products/:id` - Obtém um produto específico pelo ID.
- `POST /products` - Adiciona um novo produto.
- `PUT /products/:id` - Atualiza um produto existente pelo ID.
- `DELETE /products/:id` - Remove um produto pelo ID.

## Testes

### API RESTful em Go

Para executar os testes da API, use o comando:

```bash
go test ./...
