---
layout: page
title: "Como colaborar"
date: 2015-03-27 11:59
comments: true
share: true
footer: true
image:
  feature: http://jsenv.com/post_images/64696F92C4.jpg
---

## Antes de começar 

* [Instalar o Git](http://git-scm.com/book/pt-br/v1/Primeiros-passos-Instalando-Git). 
* [Instalar o Ruby 1.9.3](https://www.ruby-lang.org/en/documentation/installation/) ou superior.
* [Faça o fork do repositório](https://help.github.com/articles/fork-a-repo/)

## Configurando o ambiente

Gems necessárias :

``` rb
$ gem install execjs bundler 
```
Faça o clone do repositório:

``` rb 
$ git clone https://github.com/YOUR-USERNAME/jsenv
$ cd jsenv
```

Instale as gems do projeto:

``` rb
$ bundle install
```

Pronto, agora seu ambiente está configurado.

## Mantendo seu repósitorio atualizado

É fundamental manter seu fork sempre atualizado, [Leandro Cavalcante](https://twitter.com/Lezado) escreveu um post explicando como manter seu fork atulizado. Pode ser lido [aqui](http://jsenv.com/blog/2015/02/23/como-sincronizar-um-fork-com-seu-repositorio-original/).


## Colaborando com post(s)

Primeiro passo é criar uma branch com o nome do seu post, exemplo: 

```
$ git checkout -b nome_do_post
```

Crie um novo post

```
$ rake new_post["Ninja em Javascript"]
#Cria um arquivo em source/_posts/2011-07-03-ninja-em-javascript.markdown
``` 

>Edite o arquivo `2011-07-03-ninja-em-javascript.markdown` seguindo o manual de [noções básicas de Blogging](http://octopress.org/docs/blogging/) do Octopress. Confira também um exemplo de post [aqui](https://raw.githubusercontent.com/gmoura/jsenv/master/source/_posts/2015-03-08-usando-o-console-parte-1-console-api.markdown).

Faça o commit de suas alterações

```
$ git add -a -m "Novo post"
```

Faça o push de sua nova branch

```
$ git push -u nome_do_post
```

Crie um pull request relativo a branch do novo post, mais informações de como criar um pull request pode ser lido aqui, [Using pull requests](https://help.github.com/articles/using-pull-requests/).

## Processo de publicação

Seu post será avaliado pelos nossos mantedores, em caso de resalvas, as mesmas serão descritas nos comentários do pull request.

Após o pull request receber três aprovações, seu post será publicado e você será notificado.

## Requisitos mínimos do post

* Conter uma imagem de destaque, dimensão mínima de `1024x768 px`.
* Imagem de destaque deve fazer referência a coisas velhas, [exemplos](https://stocksnap.io/search/vintage/sort/relevance/desc).
* Imagem de destaque deve ser armazenada em `/source/post_images`.
* Adicione o `<!--more-->` após a introdução do post
* Imagens de conteúdo do post devem ser armazenadas em `/source/post_images_content/{nome_do_post}`.

Dúvidas ou sugestões, basta deixar um comentário que responderemos o mais breve possível.
