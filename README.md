<div id="top"></div>

<br/>
<div align="center">
    <img src="./readme-img/docker-original.svg" alt="Logo" width="100" height="100" />
    <h1 align="center">Comandos Docker</h1>
    <p align="center">Comandos para trabalhar com Docker por CLI</p>
</div>

<br/>

<div align="center">
    <a href="https://github.com/YuriSiman/docker-CLI/blob/master/LICENSE" target="_blank">
      <img alt="LICENSE" src="https://img.shields.io/badge/license-mit-%23A6CE39?style=for-the-badge&logo=github" />
    </a>
    <a href="https://github.com/YuriSiman" target="_blank">
      <img alt="GitHub" src="https://img.shields.io/badge/github-perfil-%237159c1?style=for-the-badge&logo=github" />
    </a>
    <a href="https://www.linkedin.com/in/yurisiman/" target="_blank">
      <img alt="Linkedin" src="https://img.shields.io/badge/linkedin-social-0A66C2?style=for-the-badge&logo=LinkedIn" />
    </a>
</div>

<br/>

## :clipboard: Sobre o Projeto

Este repositório foi criado com o objetivo de ser uma fonte de consulta para desenvolvedores que trabalham com Docker em linha de comando.

Aproveite! :octocat:

---

## :pencil: Pré-requisitos

1. Se você não possui o Docker instalado, acesse [aqui](https://docs.docker.com/get-started/get-docker/)) e instale conforme o seu sistema operacional.
2. Clone este repositório em sua máquina local

   ```sh
   git clone https://github.com/YuriSiman/docker-CLI.git
   ```

---

## :dart: Tópicos

<details>
  <summary>Comandos</summary>
  <ul>
    <li><a href="#gerenciar-containers">Gerenciar Containers</a></li>
    <li><a href="#executar-um-novo-container">Executar um novo Container</a></li>
    <li><a href="#gerenciar-imagens">Gerenciar Imagens</a></li>
    <li><a href="#informacoes-estatisticas">Informações e Estatísticas</a></li>
  </ul>
</details>

---

## :rocket: Vamos Começar

### Comandos Docker

<div id="gerenciar-containers"></div>

### Gerenciar Containers

Iniciar um novo Container a partir de uma imagem

-d: iniciar o Container em segundo plano
-p: mapear uma porta
--hostname: atribuir um nome de host

```sh
docker run --hostname NOME-MEU-HOST --name NOME-MEU-CONTAINER -d -p 8088:80 NOME-MINHA-IMAGEM
```

<p align="right"><a href="#top">Início ↑</a></p>

---

<div id="executar-um-novo-container"></div>

### Executar um novo Container

Monstrar lista de Containers em execução

```sh
docker ps
```

Monstrar lista de todos Containers

```sh
docker ps -a
```

Deletar um Container em execução

```sh
docker rm NOME-MEU-CONTAINER
```

Deletar um Container forçadamente

```sh
docker rm -f NOME-MEU-CONTAINER
```

Deletar Containers parados

```sh
docker container prune
```

Para um Container em execução

```sh
docker stop NOME-MEU-CONTAINER
```

Iniciar um Container parado

```sh
docker start NOME-MEU-CONTAINER
```

Renomear um Container

```sh
docker rename ANTIGO-NOME-MEU-CONTAINER NOVO-NOME-MEU-CONTAINER
```

Criar umaimagem de um Container

```sh
docker commit NOME-MEU-CONTAINER
```

<p align="right"><a href="#top">Início ↑</a></p>

---

<div id="gerenciar-imagens"></div>

### Gerenciar Imagens

Baixar uma Imagem

```sh
docker pull NOME-MINHA-IMAGEM:TAG
```

Subir uma Imagem para um repositório

```sh
docker push NOME-MINHA-IMAGEM
```

Deletar uma Imagem

```sh
docker rmi NOME-MINHA-IMAGEM
```

Mostrar lista de todas as Imagens

```sh
docker images
```

Deletar Imagens pendentes

```sh
docker images prune
```

Deletar todas as Imagens não utilizadas

```sh
docker images prune -a
```

Construir uma Imagem a partir de um Dockerfile

```sh
docker build DIRETORIO
```

Taggear uma Imagem

```sh
docker tag NOME-MINHA-IMAGEM NOME-MINHA-IMAGEM:TAG
```

Construir e Taggear uma Imagem a partir de um Dockerfile

```sh
docker build -t NOME-MINHA-IMAGEM DIRETORIO
```

Salvar uma Imagem para um arquivo tar

```sh
docker save NOME-MINHA-IMAGEM > NOME-ARQUIVO.tar
```

Carregar uma Imagem de um arquivo tar

```sh
docker load -i NOME-ARQUIVO.tar
```

<p align="right"><a href="#top">Início ↑</a></p>

---

<div id="informacoes-estatisticas"></div>

### Informações e Estatísticas

Mostrar os logs de um Container

```sh
docker logs NOME-MEU-CONTAINER
```

Mostrar estatísticas dos Containers em execução

```sh
docker stats
```

Mostrar processos de um Container

```sh
docker top NOME-MEU-CONTAINER
```

Obter detalhes de um objeto

```sh
docker inspect NOME-OBJETO
```

Mostrar arquivos modificados em um Container

```sh
docker diff NOME-MEU-CONTAINER
```

Mostrar portas mapeadas de um Container

```sh
docker port NOME-MEU-CONTAINER
```

<p align="right"><a href="#top">Início ↑</a></p>

---

## :pencil: Licença

<a href="https://github.com/YuriSiman/git-command-line/blob/master/LICENSE" target="_blank">
  <img alt="LICENSE" src="https://img.shields.io/badge/license-mit-%23A6CE39?style=for-the-badge&logo=github" />
</a>

##

Code your life :octocat:

<p align="right"><a href="#top">Início ↑</a></p>
