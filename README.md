# CRUD Farmácia - Backend

Este projeto tem como objetivo criar uma API backend para gerenciar produtos e categorias em uma farmácia, utilizando Spring Boot, JPA e MySQL. A aplicação realiza operações de CRUD (criar, ler, atualizar e excluir) para os recursos "Produto" e "Categoria".

## Tecnologias Utilizadas

- **Java**: Linguagem de programação principal.
- **Spring Boot**: Framework para construção da aplicação backend.
- **Spring Data JPA**: Para integração com banco de dados e manipulação de entidades.
- **MySQL**: Banco de dados utilizado para armazenar as informações.
- **Jakarta Validation**: Para validação dos campos das entidades.

## Endpoints da API

### Categoria

| Método | Endpoint             | Descrição                                |
|--------|----------------------|------------------------------------------|
| GET    | /categorias           | Lista todas as categorias.              |
| GET    | /categorias/{id}      | Obtém os detalhes de uma categoria.     |
| POST   | /categorias           | Cria uma nova categoria.                |
| PUT    | /categorias/{id}      | Atualiza os dados de uma categoria.     |
| DELETE | /categorias/{id}      | Exclui uma categoria.                   |

### Produto

| Método | Endpoint             | Descrição                                |
|--------|----------------------|------------------------------------------|
| GET    | /produtos             | Lista todos os produtos.                |
| GET    | /produtos/{id}        | Obtém os detalhes de um produto específico. |
| POST   | /produtos             | Cria um novo produto.                   |
| PUT    | /produtos/{id}        | Atualiza os dados de um produto.        |
| DELETE | /produtos/{id}        | Exclui um produto.                      |

### Exemplo de requisição para Produto

```json
{
  "nome": "Paracetamol",
  "descricao": "Medicamento para dor e febre",
  "preco": 10.50,
  "categoria": [
    {
      "id": 1
    }
  ]
}
