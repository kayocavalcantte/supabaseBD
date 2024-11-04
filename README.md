
# API de Produtos com Express e Supabase

Esta é uma API simples para gerenciamento de produtos, construída com Node.js, Express e Supabase. A API permite operações CRUD (Criar, Ler, Atualizar e Deletar) em uma tabela de produtos.

## Tecnologias Utilizadas

- **Node.js**: Ambiente de execução para JavaScript no lado do servidor.
- **Express**: Framework web para Node.js.
- **Supabase**: Backend como serviço (BaaS) que fornece um banco de dados e autenticação.
- **Morgan**: Middleware para registro de requisições HTTP.
- **Body-parser**: Middleware para analisar o corpo das requisições.
- **CORS**: Middleware para habilitar CORS (Cross-Origin Resource Sharing).

## Instalação

1. **Clone o repositório**:
   ```bash
   git clone https://github.com/seuusuario/seurepositorio.git
   cd seurepositorio


2. **Instale as dependências**:
   ```bash
   npm install
   ```

3. **Configuração do Supabase**:
   - Crie uma conta em [Supabase](https://supabase.io/).
   - Crie um novo projeto e uma tabela chamada `products` com os seguintes campos:
     - `id`: Integer (Auto Increment)
     - `name`: Text
     - `description`: Text
     - `price`: Numeric
   - Obtenha a URL do projeto e a chave da API.

4. **Configure as Variáveis de Ambiente**:
   Crie um arquivo `.env` na raiz do projeto e adicione as seguintes variáveis (substitua pelos seus valores):
   ```env
   SUPABASE_URL=https://vldzgqflpthizcomqtvb.supabase.co
   SUPABASE_KEY=seu_token_de_api
   ```

## Uso

1. **Inicie o servidor**:
   ```bash
   node server.js
   ```

2. O servidor estará disponível em `http://localhost:3000`.

## Endpoints

### GET /products
Retorna todos os produtos.

### GET /products/:id
Retorna um produto específico pelo ID.

### POST /products
Cria um novo produto. Exemplo de corpo da requisição:
```json
{
  "name": "Produto Exemplo",
  "description": "Descrição do produto",
  "price": 100
}
```

### PUT /products/:id
Atualiza um produto existente. Exemplo de corpo da requisição:
```json
{
  "name": "Produto Atualizado",
  "description": "Descrição atualizada",
  "price": 150
}
```

### DELETE /products/:id
Deleta um produto pelo ID.

## Contribuição

Sinta-se à vontade para abrir issues ou enviar pull requests para melhorias!

## Licença

Este projeto está licenciado sob a MIT License. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
```

### Personalizações

- Certifique-se de substituir as partes relevantes, como o nome do repositório e o URL do Git.
- Você pode adicionar seções extras, como "Exemplos de Uso", "Testes", "Autenticação", etc., conforme a complexidade do seu projeto.
