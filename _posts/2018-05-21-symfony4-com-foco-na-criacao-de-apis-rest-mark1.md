---
layout: post
title: Symfony 4
subtitle: Com foco na criação de APIS REST - mark1
tags: [php, symfony, api, rest]
---

Olá. Dando continuidade na série de artigos de APIs com Symfony 4, iremos neste artigos, criar nossa actions/métodos que irão realizar as ações ordenadas pelos verbos HTTP.

Se você não viu o ultimo artigo. Eu recomendo que você leia ele antes [por aqui]();

A estrutura do projeto, deve estar semelhante a esta:

<!-- imagem aqui -->

Mas o que vai nos interessar principalmente, é o que conteúdo da pasta ```src```. Alia recomendo que você leia um pouco sobre a estrura do Symfony 4. Talvez dependendo de quando você estiver lendo isso. Essa estrutura ja esteja um pouco alterada.

A nossa API irá obedecer os verbos do HTTP, iremos utilizar os principais. Basicamente funcionam da seguinte maneira:

| Verbo| Ações                   |
|------|-------------------------|
|GET   | busca/acessa um recurso |
|POST  | adiciona um recurso     |
|PUT   | atualiza um recurso     |
|DELETE| deleta um recurso       |


Existem outros vários verbos HTTP que são responsáveis pode diferentes ações e funções. Recomendo **fortemente** que você leia a especificação do protocolo HTTP, você pode ler aqui:

Podemos chamar de recursos em REST de propriedades globais que poderão ser manipuladas. Cada recurso deve ser idependente e ter sua próprias ações bem especificadas.

Por exemplo, nosso principal recurso neste exemplo será o recurso de *Books*. Nele nós iremos realizar e implementar todas as actions necessárias para a manipulação dos dados.

Vamos tentar nos aproximar da seguinte estrutra em endpoints:

| Verbo  | End Points         |
|--------|--------------------|
| GET    | /books/{id}        |
| POST   | /books/create      |
| PUT    | /books/update/{id} |
| DELETE | /books/delete/{id} |

Endpoint nada mais são do que nossas rotas que serão acessadas pelo usuário em cada ação que ele mandar executar.

## Continua ...
