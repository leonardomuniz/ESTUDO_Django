[![Badge](https://img.shields.io/badge/python-3.2.6-%233776AB)](https://www.python.org/)
[![Badge](https://img.shields.io/badge/django-3.2.7-%23%23092E20)](https://www.djangoproject.com/)

<br />
<p align="center">
  <a href="https://www.djangoproject.com/">
    <img src="https://static.djangoproject.com/img/logos/django-logo-negative.svg" alt="Logo">
  </a>
</p>
<p align="center">
    Tutorial exemplificado em código da documentação do <strong>Django.</strong>
</p>

<br/>

## **Tabela de conteúdos**
======================

   * [Sobre](#sobre-)
   * [Instalação](#instalacao-)
   * [Como usar](#como-usar)
   * [Referencias](#tecnologias)



<br/>

## **Sobre** 📄
Este projeto é um estudo feito por mim sobre a biblioteca e tutorial fornecidos pelo framework **Django**, e também é claro para todos aqueles que possam vir a ter algum tipo de dificuldade com o tutorial poder usar este repositório como guia de por onde ir, seja bem-vindo(a)!!


<br/>

## **Instalação** 🔨
Para este projeto estou utilizando o anaconda 3 versão **conda 4.10.1** para poder criar um ambiente virtual, o que é bem simples, basta abrir o terminal e digitar o seguinte código:

<br/>

```
 $ conda create nome_venv
```

E ele irá criar para você um ambiente virtual pronto para uso, nesse aqui ele criou com os seguintes pacotes instalados:
- asgiref==3.4.1
- certifi==2021.5.30
- Django==3.2.7
- pytz==2021.1
- sqlparse==0.4.2
- typing-extensions==3.10.0.2
- wincertstore==0.2  

e está pronto para uso !

<br/>


## **Como usar** 👨‍🏭
Após fazer a instalação de todos os pacotes necessários você pode clonar este repositório e usa-lo como guia, nesse caso:

```
- Para rodar o servidor digite no terminal:
$ python manage.py runserver

- Para visualizar a aplicação rodando digite no seu browser:
http://localhost:8000/polls/
```

<br/>

Abrindo o código no seu editor testo favorito você irá ver a seguinte disposição de arquivos:
```
├── mysite/
│   ├── __pychache__/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.js
├── polls/
│   ├── __pychache__/
│   ├── migrations/
│   ├── statics/
│   ├── templates/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── test.py
│   └── urls.py
├── db.sqlite3
├── manapy.py
└── README.md
```

<br/>


Explicando de cima para baixo o cada coisa faz:

- **Pasta [mysite]:** Todo sistema feito em Django são chamados de *projeto* e você da o nome para ele quando você está criando ele no terminal, no caso o deste repositório segui a documentação e coloquei como **mysite**, mas pode ser modificado posteriormente.

  - **mysite/__pycache__/:** aqui estaram todas as alterações no banco.

  - **mysite/settings.py:** esta é uma das partes mais importantes de todo o projeto, aqui estão armazenadas todas as aplicações do projeto *(será explicado na pasta 'polls')*, arquivo de urls, templates, conexão ao banco e diversas outras configurações necessárias.

  - **mysite/urls.py:** aqui estam registradas todas as rotas de acesso da aplicação, tanto do projeto principal quanto aplicações.

<br/>

- **Pasta [polls]:** Todo projeto feito em Django irá precisar de apps para funcionar, seja uma aplicação de login, carrinho, postagem entre outras, aplicações nada mais são que aplicações web que fazem algo no seu site.

  - **polls/__pycache__/:** aqui estaram todas as alterações no banco.

  - **polls/migrations/:** aqui estaram registradas todas as alterações no banco.

  - **polls/static/:** essa pasta está destinada a todos os arquivos estáticos que cada app poderá vir a ter como arquivos css, imagens, javascript e entre outras coisas.

  - **polls/templates/:** esta pasta contem o *"rosto"* da nossa aplicação, aqui estão todos os arquivos html que serão renderizados de forma dinamica mostrando dados para o cliente.

  - **polls/admin.py:** neste arquivo será aonde você conseguira fazer toda e qualquer configuração na pagina de administrador.

  - **polls/models.py:** este arquivo é a conecção da aplicação com o banco aonde você passara todos os campos que cada tabela irá precisar.

  - **polls/tests.py:** toda e qualquer parte do seu projeto vai precisar ser testada, testes automatizados são nossos amigos e mostraram o que potencialmente pode estar acontecendo de errado com nossa aplicação, normalmente esses são os maiores arquivos dos projetos.

  - **polls/urls.py:** assim como em *"mysite/urls.py"* aqui estão listadas todas as urls que nossa aplicação irá fornecer para o nosso usuário. 

  - **polls/views.py:** o arquivo *"views"* independente da aplicação é engrenagem ou motor do app, aqui é aonde você cria funções de listagem, cadastro, formulário entre outras funcionalidades que se relacionam seus respectivos arquivos html da pasta templates e são referenciados no arquivo *"urls"* para ser apresentado ao cliente.

<br/>

Prontinho !! Apartir daqui caso você esteja olhando dentro das pastas ou arquivos para entender o código ou travou em alguma parte do tutorial você já sabe mais ou menos para o que cada arquivo principal serve !!

<br/>

## **Referencias** 📚

Para você que leu este README até aqui [este é a documentação mencionada](https://www.djangoproject.com/start/), que é dividida em 7 partes.

<br/>

[**1° parte - configuração do ambiente**](https://docs.djangoproject.com/pt-br/3.2/intro/tutorial01/)

Nesta parte da documentação é explicado como criar um projeto e uma aplicação, além de explicar o que cada arquivo faz também mostra como rodar ela no navegador.

<br/>

[**2° parte - criar o banco, o primeiro modelo e um pouco do admin**](https://docs.djangoproject.com/pt-br/3.2/intro/tutorial02/)

Aqui como diz o titulo iremos criar um modelo para nossa aplicação, criar estas tabelas no banco, cadastrar algumas informações nele via Shell do python e também ver como funciona a parte administrativa do Django.

<br/>

[**3° parte - trabalhando na views**](https://docs.djangoproject.com/pt-br/3.2/intro/tutorial03/)

Como bem dito na parte de como usar este repositório e o que cada arquivo faz, iremos dar uma trabalhada melhor na views, criando algumas funcionalidades para listar e detalhar questões, e trabalhando com URLs.

<br/>

[**4° parte - aplicando templates**](https://docs.djangoproject.com/pt-br/3.2/intro/tutorial04/)

Como é mostrado  na parte 3 do tutorial, aqui iremos fazer com que nossas views retornem alguma coisa em formato de html, assim poderá ser mais fácil de ver o que estamos buscando do nosso banco de dados.

<br/>

[**5° parte - desenvolvimento de testes**](https://docs.djangoproject.com/pt-br/3.2/intro/tutorial05/)

"Testes vão salvar seu tempo" e de fato irão, nós iremos desenvolver testes automatizados de coisas que podem acontecer na nossa aplicação, como por exemplo o usuário postar uma questão no futuro, se a questão está em algum periodo na qual não deveria estar e entre outras coisas.

<br/>

[**6° parte - estilizando o projeto**](https://docs.djangoproject.com/pt-br/3.2/intro/tutorial06/)
Todo bom projeto precisa de uma visualização um pouco mais agradavel, logo nesta parte vamos descobrir como carregar arquivos estáticos para nossa aplicação como css e imagens.

<br/>

[**7° parte - desenvolvendo o admin**](https://docs.djangoproject.com/pt-br/3.2/intro/tutorial07/)
Um dos pontos principais do django é poder utilizar da funcionalidade administrador para ter um painel de controle completamente funcional, mas as vezes queremos poder ter um painel com um pouco mais da nossa cara, este é o capítulo para isso.



