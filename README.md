<div align="center" id="top"> 
  <img src="./.github/app.gif" alt="Ambiente_de_desenvolvimentos_scs" />

  &#xa0;

  <!-- <a href="https://ambiente_de_desenvolvimentos_scs.netlify.app">Demo</a> -->
</div>

<h1 align="center">Ambiente de desenvolvimentos SCS Facimp</h1>

<p align="center">
  <img alt="Github top language" src="https://img.shields.io/github/languages/top/{{YOUR_GITHUB_USERNAME}}/ambiente_de_desenvolvimentos_scs?color=56BEB8">

  <img alt="Github language count" src="https://img.shields.io/github/languages/count/{{YOUR_GITHUB_USERNAME}}/ambiente_de_desenvolvimentos_scs?color=56BEB8">

  <img alt="Repository size" src="https://img.shields.io/github/repo-size/{{YOUR_GITHUB_USERNAME}}/ambiente_de_desenvolvimentos_scs?color=56BEB8">

  <img alt="License" src="https://img.shields.io/github/license/{{YOUR_GITHUB_USERNAME}}/ambiente_de_desenvolvimentos_scs?color=56BEB8">

  <!-- <img alt="Github issues" src="https://img.shields.io/github/issues/{{YOUR_GITHUB_USERNAME}}/ambiente_de_desenvolvimentos_scs?color=56BEB8" /> -->

  <!-- <img alt="Github forks" src="https://img.shields.io/github/forks/{{YOUR_GITHUB_USERNAME}}/ambiente_de_desenvolvimentos_scs?color=56BEB8" /> -->

  <!-- <img alt="Github stars" src="https://img.shields.io/github/stars/{{YOUR_GITHUB_USERNAME}}/ambiente_de_desenvolvimentos_scs?color=56BEB8" /> -->
</p>

<!-- Status -->

<!-- <h4 align="center"> 
	🚧  Ambiente_de_desenvolvimentos_scs 🚀 Under construction...  🚧
</h4> 

<hr> -->

<p align="center">
  <a href="#dart-about">About</a> &#xa0; | &#xa0; 
  <a href="#sparkles-features">Features</a> &#xa0; | &#xa0;
  <a href="#rocket-technologies">Technologies</a> &#xa0; | &#xa0;
  <a href="#white_check_mark-requirements">Requirements</a> &#xa0; | &#xa0;
  <a href="#checkered_flag-starting">Starting</a> &#xa0; | &#xa0;
  <a href="#memo-license">License</a> &#xa0; | &#xa0;
  <a href="https://github.com/{{YOUR_GITHUB_USERNAME}}" target="_blank">Author</a>
</p>

<br>

## :dart: Sobre o Projeto ##

Ambiente de desenvolvimento da SCS na Facimp Wyden

## :rocket: Tecnologias ultilizadas ##

Ferramentas ultilizadas no projeto:

- [Vite](https://pt-br.reactjs.org/)
- [Reactjs](https://pt-br.reactjs.org/)
- [TypeScript](https://www.typescriptlang.org/)
- [Laravel](https://www.typescriptlang.org/)
- [Postgres](https://www.typescriptlang.org/)
- [Docker](https://www.typescriptlang.org/)

## :white_check_mark: Requirements ##

Para rodar o projeto, você vai precisar do docker [Docker](https://www.docker.com/).

## :checkered_flag: Subindo o ambiente de desenvolvimento ##

```bash
# Clone o projeto
$ git clone https://github.com/guilherf13/SCS_DevOps

# Executando o ambiente

$ cd SCS_DevOps
$ cd backend
$ cp .env.example .env
$ cd ..
$ cd ..
$ sudo chmod -R 777 SCS_DevOps
$ cd SCS_DevgOps
$ docker compose up -d --build
$ docker exec -it backend composer install
$ docker exec -it backend php artisan key:generate

# A aplicação esta rodando nas seguintes portas:

# laravel <http://localhost:80>
# vite <http://localhost:5173>
# postgres port 5432
```

## :memo: License ##

This project is under license from MIT. For more details, see the [LICENSE](LICENSE.md) file.


Made with :heart: by <a href="https://github.com/guilherf13" target="_blank">{{guilherme}}</a>

&#xa0;

<a href="#top">Back to top</a>
