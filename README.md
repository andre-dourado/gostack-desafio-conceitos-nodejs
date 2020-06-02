<img alt="GoStack" src="https://storage.googleapis.com/golden-wind/bootcamp-gostack/header-desafios.png" />

<h3 align="center">
  Desafio 02: Conceitos do Node.js
</h3>

## 🚀 Sobre o desafio
Nesse desafio, foi criado uma aplicação em NodeJS que permite a criação, listagem, atualização e remoção dos repositórios, e além disso permite que os repositórios possam receber "likes".

### Rotas da aplicação

- **`POST /repositories`**: A rota recebe `title`, `url` e `techs` dentro do corpo da requisição, sendo a URL o link para o github desse repositório. Além disso é gerado um ID do tipo UUID e o campo likes iniciando com o valor 0.

- **`GET /repositories`**: Rota que lista todos os repositórios;

- **`PUT /repositories/:id`**: A rota altera apenas o `título`, a `url` e as `techs` do repositório que possua o `id` igual ao `id` presente nos parâmetros da rota;

- **`DELETE /repositories/:id`**: A rota deleta o repositório com o `id` presente nos parâmetros da rota;

- **`POST /repositories/:id/like`**: A rota aumenta o número de likes do repositório específico escolhido através do `id` presente nos parâmetros da rota, a cada chamada dessa rota, o número de likes aumenta em 1;
