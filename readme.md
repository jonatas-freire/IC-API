# Iniciação Ciêntífica

Projeto volutário desenvolvido com o objetivo de automatizar o processo do [**Programa de Iniciação Científica (PIC)**](https://fatecrl.edu.br/projetos/iniciacao-cientifica) da Fatec Rubens Lara, utilizando as tecnólogias **NodeJS**, **MySql** e **Docker**.

Para executar o projeto em modo de desenvolvimento é necessário a instalação do **docker**

## Executando em modo de desenvolvimento

Após instalado o docker basta utilizando o comando
```
    docker-compose up
```

*O comando docker-compose up ira criar todo o ambiente necessário para trabalhar com aplicação, desde a configuração do banco de dados até as configurações da aplicação*

## Arquitetura da Aplicação

O projeto é uma **API REST** estando dividido da seguinte forma:

```bash
src
    ├───app
    │   ├───config
    │   ├───controller
    │   ├───model
    │   ├───repository
    │   └───view
    └───database
        ├───migrations
        └───seeders
```

**config**: pasta destinada para arquivos de configuração como banco de dados, api key do google, etc.

**controller**: camada dos controladores responsaveis pelas regras de negocios.

**model**: camada responsavel por criar os modelos que serão utilizado como a nossa abstração do banco de dados.

**repository**: camada responsavel pela manipulação das models.

**view**: camada utilizada para validação dos dados recebido e definição de rotas.

**migrations**: pasta destinada para os arquivos referentes as nossas tabelas do banco de dados.

**seeders**: pasta destinado para os dados pre cadastrados do nosso banco.

## Modelo do Banco de Dados

