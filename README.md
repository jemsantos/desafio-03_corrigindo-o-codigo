# Desafio-03_Corrigindo-o-Codigo
Desafio 'Corrigindo o código' aplicado no Bootcamp Ignite

## 💻 Sobre o desafio

Nesse desafio, temos uma aplicação Node.js que está em processo de desenvolvimento mas que já possui os testes necessários para fazer toda a validação dos requisitos.

Após algumas alterações no código da aplicação, parte dos testes deixaram de passar e agora só você pode resolver esse problema. Bora lá? 🚀

Essa aplicação realiza o CRUD (**C**reate, **R**ead, **U**pdate, **D**elete) de repositórios de projetos. Além disso, é possível dar likes em repositórios cadastrados, aumentando a quantidade de likes em 1 a cada vez que a rota é chamada.


## Rotas da aplicação

### GET `/repositories`

A rota deve retornar uma lista contendo todos os repositórios cadastrados.

### POST `/repositories`

A rota deve receber `title`, `url` e `techs` pelo corpo da requisição e retornar um objeto com as informações do repositório criado e um status `201`.

### PUT `/repositories/:id`

A rota deve receber `title`, `url` e `techs` pelo corpo da requisição e o `id` do repositório que deve ser atualizado pelo parâmetro da rota. Deve alterar apenas as informações recebidas pelo corpo da requisição e retornar esse repositório atualizado.

### DELETE `/repositories/:id`

A rota deve receber, pelo parâmetro da rota, o `id` do repositório que deve ser excluído e retornar um status `204` após a exclusão.

### POST `/repositories/:id/like`

A rota deve receber, pelo parâmetro da rota, o `id` do repositório que deve receber o like e retornar o repositório com a quantidade de likes atualizada.

## Específicação dos testes

### Testes de repositórios

- **Should be able to create a new repository**
- **Should be able to list the projects**
- **Should be able to update repository**
- **Should not be able to update a non existing repository**
- **Should not be able to update repository likes manually**
- **Should be able to delete the repository**
- **Should not be able to delete a non existing repository**

### Testes de likes

- **Should be able to give a like to the repository**
- **Should not be able to give a like to a non existing repository**
