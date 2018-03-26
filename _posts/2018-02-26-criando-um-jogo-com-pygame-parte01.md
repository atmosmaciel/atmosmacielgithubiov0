---
layout: post
title: Criando um jogo com Pygame - parte 01
subtitle: Conhecendo o projeto e fazendo configurações iniciais
tags: [python, pygame, games]
---

Neste artigo nós iremos criar um jogo utilizando o Pygame. Este primeiro exemplo será bem simples para que a gente possa absorver os conceitos iniciais do Pygame e também utilizar algumas de suas funções na prática.

## O Pygame

O Pygame é uma biblioteca do Python que estende o SDL(Simple DirectMedia Layer). O SDL é uma biblioteca multimídia multiplataforma, escrita em C. O Pygame funciona como um módulo do Python que fornece uma API para o SDL, além de várias implementações para criações gráficas com foco em jogos. Você pode saber mais aqui e em português aqui.

## Configurações iniciais

### Configurando o Virtualenv

Antes de mais nada, devo lembrar que se você está começando a se aventurar agora no Pygame, não necessariamente você deverá utilizar virtualenvs. Mas nós utilizaremos aqui por se tratar de uma boa prática.

Utilizar virtualenvs, nos permite, principalmente, separar as dependências do nosso projeto das bibliotecas globais do sistema operacional, assim nós mantemos versões compatíveis entre essas dependências sem nos preocupar que elas possam impactar nas bibliotecas globais do OS. Se você está usando Windows, isso não deve ser um problema pra você. Mas se estiver utilizando sistemas baseados no Unix, essa prática pode evitar problemas futuros.

Eu utilizo a seguinte abordagem: <a target="_blank" href="https://medium.com/welcome-to-the-django/guia-definitivo-para-organizar-meu-ambiente-python-a16e2479b753">Guia definitivo para organizar meu ambiente Python</a>

A partir do artigo acima, você pode iniciar seus estudos e definir a melhor forma de trabalhar com virtualenvs nos seus projetos.

Eu criei um virtualenv chamado env-pygame através do seguinte comando:

```mkvirtualenv env-pygame```

<center>
    <img src="../img/articles-images/2018-02-26-criando-um-jogo-com-pygame-parte01/2018-02-26-criando-um-jogo-com-pygame-parte01-mark0.png" alt="">
</center>

### Utilizando a Virtualenv

Para utilizar nosso virtualenv você deve ativá-lo, para isso, utilize o seguinte comando:

```workon o-nome-do-seu-virtual-env```

<center>
    <img src="../img/articles-images/2018-02-26-criando-um-jogo-com-pygame-parte01/1__fNBLcUKSRw4iOc_Z_WCzw.png" alt="">
</center>

### Instalando Pygame

Agora que temos nosso virtualenv ativo iremos instalar o Pygame com o seguinte comando:

```pip install pygame```

<center>
    <img src="../img/articles-images/2018-02-26-criando-um-jogo-com-pygame-parte01/1_Z3bJplD4HeqQoGRb__adjQ.png" alt="">
</center>

Em projetos maiores nossa estrutura de diretórios seria melhor dividida, teríamos mais módulos e consequentemente mais arquivos. No nosso caso teremos apenas um arquivo principal que eu vou chamar de main.py e um diretório para guardar as imagens que iremos utlizar, nos próximos artigos iremos conhecer essa estrutura inicial.

Agora já temos o que precisamos para começar a trabalhar com o Pygame da forma correta. Investir esse tempo inicial para fazer a devida ambientação no sistema vai nos livrar de muitas preocupações.

### Conhecendo o Projeto

O jogo que iremos criar é bem simples. Teremos apenas 3 elementos: uma barra, uma bola, e a tela de fundo. Ao final dessa série de artigos nosso jogo deverá funcionar de forma semelhante a isso(poderão haver modificações):

<center>
    <img src="../img/articles-images/2018-02-26-criando-um-jogo-com-pygame-parte01/1_bvUZYV4iliY8546NS2i5wg.gif" alt="">
</center>

Nada muito impressionante não é mesmo? Mas com isso nós iremos entender, controles, colisões, movimentações de objetos e outros conceitos bem legais que o Pygame nos permite utilizar. Todos sabemos como funciona este jogo.

A bola se move de forma independente dentro do espaço e se ela passar pela barra o jogo será finalizado.

### Conclusões

No próximo artigo vamos começar a implementar as primeiras funções do nosso game.

Por hoje é só galera. Até a próxima.

*OBS: Este artigo foi originalmente postado no site da <a target="_blank" href="https://blog.codeexpertslearning.com.br/como-criar-seu-primeiro-jogo-com-pygame-parte-01-8eb7e704a488">Code Experts Learning</a>*.
