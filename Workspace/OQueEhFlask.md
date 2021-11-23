# O que é Flask?

Veja neste artigo o que é o Flask, principal micro-framework do ecossistema Python.

 mais de 2 anos atrás

[Artigos](https://www.treinaweb.com.br/blog)O que é Flask?

Escrito em [Python](https://www.treinaweb.com.br/blog/o-que-e-python/) e disponível sobre a licença BSD (Licença de código aberto), o Flask é um micro-framework multiplataforma que provê um modelo simples para o desenvolvimento web.



![Flask - Fundamentos](https://d2knvm16wkt3ia.cloudfront.net/assets/svg-icon/flask.svg)

##### CursoFlask - Fundamentos

[Conhecer o curso](https://www.treinaweb.com.br/curso/flask-fundamentos)



## Mas afinal, o que é um Micro-framework?

Já falamos aqui no blog [o que é um micro-framework](https://www.treinaweb.com.br/blog/o-que-e-um-micro-framework/), mas para relembrar:

Um Micro-Framework são Frameworks modularizados que possuem uma estrutura inicial muito mais simples quando comparado a um [Framework](https://www.treinaweb.com.br/blog/para-que-serve-um-framework/) convencional.

Podemos dizer que o micro-framework é uma versão minimalista destes frameworks, sendo bastante utilizado para criação de microsserviços, como APIs RESTful.

No artigo anterior, fizemos uma comparação de objetos do mundo real para exemplificar o funcionamento de um micro-framework:

Pense em um Micro-Framework como uma peça de lego. Inicialmente, um projeto criado com o micro-framework possui apenas o básico para funcionar, (normalmente, sistema de rotas), porém, ao decorrer do projeto, podem haver necessidades para utilização de outros recursos como, conexão de banco de dados, sistemas de templates, envio de email, etc. A partir desta necessidade, novas bibliotecas são “encaixadas” no projeto, como uma estrutura de lego.

![img]()



![Flask - Desenvolvimento de APIs REST](https://d2knvm16wkt3ia.cloudfront.net/assets/svg-icon/flask.svg)

##### CursoFlask - Desenvolvimento de APIs REST

[Conhecer o curso](https://www.treinaweb.com.br/curso/flask-desenvolvimento-de-apis-rest)



## De volta ao Flask…

Lançado em 2010 e desenvolvido por Armin Ronacher, o Flask é um micro-framework destinado principalmente a pequenas aplicações com requisitos mais simples, como por exemplo, a criação de um site básico.

Possui um núcleo simples e expansível que permite que um projeto possua apenas os recursos necessários para sua execução (conforme surja a necessidade, um novo pacote pode ser adicionado para incrementar as funcionalidades da aplicação).

## Características do Flask

- Simplicidade: Por possuir apenas o necessário para o desenvolvimento de uma aplicação, um projeto escrito com Flask é mais simples se comparado aos frameworks maiores, já que a quantidade de arquivos é muito menor e sua arquitetura é muito mais simples.
- Rapidez no desenvolvimento: Com o Flask, o desenvolvedor se preocupa em apenas desenvolver o necessário para um projeto, sem a necessidade de realizar configurações que muitas vezes não são utilizadas.
- Projetos menores: Por possuir uma arquitetura muito simples (um único arquivo inicial) os projetos escritos em Flask tendem a ser menores e mais leves se comparados a frameworks maiores.
- Aplicações robustas: Apesar de ser um micro-framework, o Flask permite a criação de aplicações robustas, já que é totalmente personalizável, permitindo, caso necessário, a criação de uma arquitetura mais definida.

## Exemplo de uma aplicação Flask

Abaixo podemos ver um exemplo de uma aplicação em Flask. Podemos notar o quão simples criar uma aplicação web pode ser:

Copiar

```python
from flask import Flask
app = Flask(__name__)

@app.route("/")
def index():
    return 'Bem-vindo a TreinaWeb!'

if __name__ == "__main__":
    app.run()
```

## Podemos concluir que…

O Flask é uma excelente alternativa para o desenvolvimento de aplicações utilizando o Python. Ele é o principal concorrente do [Django](https://www.treinaweb.com.br/blog/o-que-e-django/), apesar de ser considerado um micro-framework.

Aqui no blog da TreinaWeb fizemos um comparativo entre o [Django e o Flask](https://www.treinaweb.com.br/blog/django-ou-flask-eis-a-questao/), caso esteja em dúvida em qual framework utilizar, vale a pena a leitura.