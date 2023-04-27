# Product-List
Este projeto foi desenvolvido como parte do curso de Desenvolvimento Full-Stack da PUC-Rio. O objetivo é criar uma lista de compras para auxiliar na organização de itens a serem comprados no mercado. O sistema permite que o usuário adicione produtos à lista, juntamente com suas quantidades e preços correspondentes.

O projeto é uma API RESTful desenvolvida em Flask que permite a adição, visualização e remoção de produtos e comentários associados a eles. Foram utilizados HTML, CSS e Javascript para desenvolver a interface do usuário.

## Utilização

A API possui três endpoints: `/produto`, `/produtos` e `/produto`.

### `/produto`

O endpoint `/produto` permite a adição de um novo produto à base de dados. Para adicionar um produto, é necessário fazer uma requisição `POST`, passando as informações do produto em um JSON no corpo da requisição.

As informações necessárias para adicionar um produto são:

- `nome`: nome do produto 
- `quantidade`: quantidade em estoque do produto 
- `valor`: valor do produto 

Em caso de sucesso, a API retorna uma representação dos produtos e comentários associados em formato JSON. Em caso de erro, a API retorna uma mensagem de erro com um status code indicando o erro.

### `/produtos`

O endpoint `/produtos` permite a visualização de todos os produtos cadastrados na base de dados. Para visualizar os produtos, é necessário fazer uma requisição `GET`.

Em caso de sucesso, a API retorna uma representação da listagem de produtos em formato JSON. Em caso de erro, a API retorna uma mensagem de erro com um status code indicando o erro.

### `/produto`

O endpoint `/produto` permite a busca de um produto específico a partir do ID do produto. Para buscar um produto, é necessário fazer uma requisição `GET`, passando o ID do produto na query string.

As informações necessárias para buscar um produto são:

- `id`: ID do produto 

Em caso de sucesso, a API retorna uma representação dos produtos e comentários associados em formato JSON. Em caso de erro, a API retorna uma mensagem de erro com um status code indicando o erro.

O endpoint `/produto` também permite a remoção de um produto específico a partir do nome do produto. Para remover um produto, é necessário fazer uma requisição `DELETE`, passando o nome do produto na query string.

As informações necessárias para remover um produto são:

- `nome`: nome do produto 

Em caso de sucesso, a API retorna uma mensagem de confirmação da remoção em formato JSON. Em caso de erro, a API retorna uma mensagem de erro com um status code indicando o erro.

## Documentação

A documentação da API pode ser acessada nos seguintes endpoints:

- `/openapi`: documentação Swagger
- `/redoc`: documentação Redoc
- `/rapidoc`: documentação RapiDoc


