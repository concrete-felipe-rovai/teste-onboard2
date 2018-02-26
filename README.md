[1]: https://www.saraiva.com.br/scrum-a-arte-de-fazer-o-trabalho-na-metade-do-tempo-9381460.html?pac_id=123134&gclid=EAIaIQobChMIkemf3eXD2QIVTlmGCh12GgibEAQYASABEgId7fD_BwE
[2]: https://br.udacity.com/course/intro-to-devops--ud611
[3]: https://hub.docker.com/

# ON-Board

  Abaixo será definido um tutorial para seguir de treinamentos:
  
## Ler Scrumbook

Você deve ler o livro a seguir para entender o framework Scrum, como funciona, como se aplica, entre outras coisas - [Scrum - A Arte de Fazer o Trabalho na Metade do Tempo][1]

<img src="https://images.livrariasaraiva.com.br/imagemnet/imagem.aspx/?pro_id=9381460&qld=90&l=430&a=-1" width="150">

## Agile

Nesta etapa, você deve estudar os frameworks abaixo:
* SCRUM
* Kanban
* Extreme Programming

No final dos estudos você deve montar uma apresentação com tudo sobre o que aprendeu referente a estes frameworks.

## Learn the basics about DevOps

Aqui você deve realizar o curso [Intro to DevOps][2] .
Detalhe, você deve solicitar ao seu gestor a criação de contas na AWS, GCP e Azure para concluir algum dos labs.
Quando finalizado, monte uma apresentação sobre o que aprendeu.

## Learn GitHub

## Use Bitbucket

## Learn about git

## Learn basics about docker

Realizar as tarefas abaixo:

* Criar uma imagem com um site mostrando a frase "Hello World!"
* Criar uma conta no [Docker Hub][3] e fazer o upload da imagem que você criou no passo anterior.
* Utilize 2 imagens já disponíveis no Docker Hub para subir uma aplicação linkada ( exemplo Wordpress + MySQL )

```shell

1. Crie o arquivo stack-teste.yml com o comando abaixo:
touch stack-teste.yml

2. Coloque o conteúdo abaixo dentro do arquivo stack-teste.yml

version: '3.1'

services:

  wordpress:
    image: wordpress
    restart: always
    ports:
      - 8080:80
    environment:
      WORDPRESS_DB_PASSWORD: example

  mysql:
    image: mysql:5.7
    restart: always
    environment:
      MYSQL_ROOT_PASSWORD: example
```

