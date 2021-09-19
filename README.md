[![Badge](https://img.shields.io/badge/python-3.2.6-%233776AB)](https://www.python.org/)
[![Badge](https://img.shields.io/badge/django-3.2.7-%23%23092E20)](https://www.djangoproject.com/)

<br />
<p align="center">
  <a href="https://www.djangoproject.com/">
    <img src="https://static.djangoproject.com/img/logos/django-logo-negative.svg" alt="Logo">
  </a>
</p>
<p align="center">
    Tutorial em código da documentação do <strong>Django.</strong>
</p>

<br/>

## **Tabela de conteúdos**
======================

   * [Sobre](#sobre-)
   * [Instalação](#instalação-)
   * [Como usar](#como-usar-)
   * [Referencias](#referencias-)



<br/>

## **Sobre** 📄
Este projeto é um estudo feito por mim Leonardo C. Muniz sobre a biblioteca e tutoriais, iniciais, do **Django**. E tem o intuito de ser útil a todos que tiverem dificuldes na documantação podem usar este repositório como guia de por onde ir. Neste projeto é feito um sistema de votações aonde serão cadastradas algumas questões via linha de comando e/ou painel de administrador e o usuário podera votar em qualquer uma das alternativas das questões


<br/>

## **Instalação** 🔨
Para este projeto estou utilizando o anaconda 3 versão **conda 4.10.1** para poder criar um ambiente virtual, o que é bem simples de fazer, basta abrir o terminal do anaconda e digitar o seguinte código:

<br/>

```
 $ conda create nome_ambiente_virtual
```

E ele irá criar para você um ambiente virtual pronto para uso, neste aqui ele criou com os seguintes pacotes instalados:
- asgiref==3.4.1
- certifi==2021.5.30
- Django==3.2.7
- pytz==2021.1
- sqlparse==0.4.2
- typing-extensions==3.10.0.2
- wincertstore==0.2  

e está pronto!

<br/>


## **Como usar** 👨‍🏭
Após fazer a instalação de todos os pacotes necessários você pode clonar este repositório e usa-lo como guia, nesse caso abra seu terminal na pasta do repositório e siga os seguintes passos:

```
- Para rodar o servidor digite no terminal:
$ python manage.py runserver

- Para visualizar a aplicação rodando digite no seu browser:
http://localhost:8000/polls/
```

<br/>

Abrindo o código no seu editor texto favorito você irá ver a seguinte disposição de arquivos:
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


Explicando o que cada pasta ou arquivo faz:

- **Pasta [mysite]:** Todo sistema feito em Django são chamados de *projeto*, no caso deste repositório coloquei como **mysite**, mas pode por o nome que quiser.

  - **mysite/__pycache__/:** aqui estaram todas as alterações no banco.

  - **mysite/settings.py:** aqui estão armazenadas todas as configurações importantes como chave de segurança, aplicações, banco de dados e entre outras coisas.

  - **mysite/urls.py:** se encontra aqui as rotas do projeto, tanto as principais quanto as de aplicações.

<br/>

- **Pasta [polls]:** Todo projeto irá precisar de aplicações para funcionar, seja de login, carrinho, formulário, entre outras. Elas nada mais são do que aplicações web que fazem algo no seu site, e neste projeto nosso app principal e o de votação de questões

  - **polls/__pycache__/:** aqui estaram todas as alterações no banco.

  - **polls/migrations/:** nesta pasta estaram registradas todas as alterações no banco.

  - **polls/static/:** aqui estão todos os arquivos estáticos que cada app poderá vir a ter como arquivos css ou imagens.

  - **polls/templates/:** esta pasta contem o *"rosto"* da nossa aplicação, aqui estão todos os arquivos html que serão renderizados de forma dinamica para o cliente.

  - **polls/admin.py:** neste arquivo será aonde você conseguira fazer toda e qualquer configuração na pagina de administrador.

  - **polls/models.py:** este arquivo é a conecção da aplicação com o banco aonde você poderá contruir todos os campos que cada tabela irá precisar.

  - **polls/tests.py:** toda e qualquer parte do seu projeto vai precisar ser testada, testes automatizados são nossos amigos e mostraram o que potencialmente pode estar acontecendo de errado com nossa aplicação, normalmente esses são os maiores arquivos dos projetos.

  - **polls/urls.py:** assim como em *"mysite/urls.py"* aqui estão listadas todas as urls que nossa aplicação irá fornecer para o nosso usuário. 

  - **polls/views.py:** o arquivo *"views"* independente age como o motor do app, aqui é aonde estão as funções de listagem, cadastro, formulário entre outras que se relacionam com os templates html e o arquivo de rotas *"urls"* para ser apresentado ao cliente.

<br/>

Prontinho !! Caso esteja utilizando este para mexer no código ou travou no tutorial você já sabe mais ou menos para o que cada arquivo ou pasta servem.

<br/>

## **Referencias** 📚

Para você que leu este README até aqui [este é a documentação mencionada](https://www.djangoproject.com/start/) do nosso projetinho de questões e votação, que é dividida em 7 partes.

<br/>

[**1° parte - configuração do ambiente**](https://docs.djangoproject.com/pt-br/3.2/intro/tutorial01/)

Nesta introdução é ensinado como criar um projeto, o que cada arquivo faz e também mostra como rodar ele no navegador.

<br/>

[**2° parte - criar o banco, o primeiro modelo e um pouco do admin**](https://docs.djangoproject.com/pt-br/3.2/intro/tutorial02/)

Vamos criar o modelo das tabelas de questões e alternativas para as tabelas no banco, cadastrar algumas informações via Shell e também ver como funciona o painel de administrador do Django.

<br/>

[**3° parte - trabalhando na views**](https://docs.djangoproject.com/pt-br/3.2/intro/tutorial03/)

Iremos dar uma atenção para as views, criando algumas funcionalidades como listar e detalhar questões também vamos integralas as URLs para que seja possível ver o que tem no banco.

<br/>

[**4° parte - aplicando templates**](https://docs.djangoproject.com/pt-br/3.2/intro/tutorial04/)

Utilizar as views para retornar informações é util porém será muito melhor utilizando nossas pasta de templates para que possamos trabalhar com html para mostrar as questões

<br/>

[**5° parte - desenvolvimento de testes**](https://docs.djangoproject.com/pt-br/3.2/intro/tutorial05/)

"Testes vão salvar seu tempo" e de fato irão, iremos desenvolver testes automatizados de coisas que podem acontecer na nossa aplicação, como o usuario postar uma questão no futuro, se faz pouco tempo que a questão foi postada, se faz muito tempo e entre outras testes de segurança.

<br/>

[**6° parte - estilizando o projeto**](https://docs.djangoproject.com/pt-br/3.2/intro/tutorial06/)

Todo bom projeto precisa de uma visualização um pouco mais agradavel, logo, vamos trabalhar com arquivos estaticos adicionando css aos templates.

<br/>

[**7° parte - desenvolvendo o admin**](https://docs.djangoproject.com/pt-br/3.2/intro/tutorial07/)

Um ponto forte do django é o seu painel de administrado, porém é sempre poder ter um painel que atenda todos as nossas necessidades então vamos editar-lo um pouco.



