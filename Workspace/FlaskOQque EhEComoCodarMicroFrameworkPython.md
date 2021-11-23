- [Full stack](https://blog.geekhunter.com.br/category/full-stack/)

# Flask: o que é e como codar com esse micro framework Python

- setembro 23, 2020
- [2 Comments](https://blog.geekhunter.com.br/flask-framework-python/#disqus_thread)

O objetivo deste artigo é mostrar de forma prática e objetiva sobre como começar a codar com Flask! 😁

Existem outros [frameworks de Python](https://blog.geekhunter.com.br/os-5-melhores-frameworks-de-python/), escolha o melhor para o seu projeto!

**Conteúdo** [ocultar](https://blog.geekhunter.com.br/flask-framework-python/#) 

[1 O que é o Flask?](https://blog.geekhunter.com.br/flask-framework-python/#O_que_e_o_Flask)

[1.1 WSGI](https://blog.geekhunter.com.br/flask-framework-python/#WSGI)

[1.2 Werkzeug](https://blog.geekhunter.com.br/flask-framework-python/#Werkzeug)

[1.3 Jinja2](https://blog.geekhunter.com.br/flask-framework-python/#Jinja2)

[2 Preciso saber programar em Python para utilizar o Flask?](https://blog.geekhunter.com.br/flask-framework-python/#Preciso_saber_programar_em_Python_para_utilizar_o_Flask)

[2.1 Este artigo é para mim?](https://blog.geekhunter.com.br/flask-framework-python/#Este_artigo_e_para_mim)

[2.2 O que eu utilizei para criar esse artigo](https://blog.geekhunter.com.br/flask-framework-python/#O_que_eu_utilizei_para_criar_esse_artigo)

[3 Flask Tutorial](https://blog.geekhunter.com.br/flask-framework-python/#Flask_Tutorial)

[3.1 Preparando o ambiente](https://blog.geekhunter.com.br/flask-framework-python/#Preparando_o_ambiente)

[3.2 Utilizando o PIP](https://blog.geekhunter.com.br/flask-framework-python/#Utilizando_o_PIP)

[3.3 Instalando o Flask](https://blog.geekhunter.com.br/flask-framework-python/#Instalando_o_Flask)

[3.4 Escrevendo o primeiro código em Flask](https://blog.geekhunter.com.br/flask-framework-python/#Escrevendo_o_primeiro_codigo_em_Flask)

## **O que é o Flask?**

Flask é um micro framework que utiliza a linguagem Python para criar aplicativos Web.

Não se deixe enganar pelo prefixo “micro”, em algumas extensões o Flask é poderoso e ideal para quem busca:

- Simplicidade;
- Rapidez;
- Soluções para projetos pequenos;
- Aplicações robustas.

Lançado em 2010 e desenvolvido por Armin Ronacher, a estrutura do **Flask permite desenvolver aplicativos da web facilmente**.

Ronacher ganhou fama por liderar uma comunidade de entusiastas do Python chamada Poocco. O Flask é baseado no kit de ferramentas Werkzeg WSGI e na biblioteca Jinja2. Ambos são projetos herdados da Poocco.

### WSGI

A Web Server Gateway Interface (Web Server Gateway Interface, WSGI) tem sido usada como um padrão para o desenvolvimento de aplicativos da Web em Python.

Em suma, WSGI é a especificação de uma interface comum entre servidores e aplicativos da web.

### Werkzeug

O Werkzeug é uma das bases do Flask, um kit de ferramentas WSGI que implementa funções como *requests*, por exemplo.

### Jinja2

O Jinja2 é um sistema de *web template* que combina um modelo com uma fonte de dados específica para renderizar uma página da web.

Isso permite que você passe variáveis Python para modelos HTML como este:

```
<html>
    <head>
        <title>{{ title }}</title>
    </head>
    <body>
        <h1>Hello {{ username }}</h1>
    </body>
</html>
```

Para saber mais sobre as bases do Flask, seu criador e a parte mais estrutural do framework, confira esta apresentação de Eduardo Mendes, na FlaskConf 2019:

<iframe title="Introdução ao Flask - [FlaskConf 2019]" width="820" height="461" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen="" data-src="https://www.youtube.com/embed/Snxl0T8ugeI?feature=oembed&amp;enablejsapi=1&amp;origin=https://blog.geekhunter.com.br" class=" lazyloaded" data-gtm-yt-inspected-1_19="true" style="box-sizing: border-box; max-width: 100%; position: absolute; inset: 0px; width: 620px; height: 348.75px; border: 0px;"></iframe>

Introdução ao Flask – [FlaskConf 2019]

## **Preciso saber programar em Python para utilizar o Flask?** 

Sim, é necessário que você já tenha algum conhecimento na linguagem Python para começar a usar o Flask.

Mas não se preocupe, caso você não tenha experiência nessa linguagem, o Python é uma linguagem relativamente simples de se aprender. Nesse artigo tem algumas dicas para você iniciar a sua [carreira como desenvolvedor Python](https://blog.geekhunter.com.br/passos-para-iniciar-a-sua-carreira-de-desenvolvedor-na-linguagem-python/).

Se você já programa em outras linguagens, será mais fácil ainda aprender a usar o Python. Com um pouco de dedicação, pesquisas e estudos, em alguns dias você já terá o conhecimento necessário para começar a desenvolver com Python.

Agora, se já possui experiência com Python, você pode querer dar uma olhada nas [**oportunidades para desenvolvedores Python**](https://www.geekhunter.com.br/vagas-python). Temos vagas sendo criadas e preenchidas todos os dias, por isso não perca tempo 😉

### Este artigo é para mim?

Se você tem conhecimentos em Python e quer começar a desenvolver aplicativos Web utilizando o Flask, esse artigo é para você mesmo!

Vou te mostrar como configurar o ambiente e dar os primeiros passos no Flask, tudo de forma prática.

### O que eu utilizei para criar esse artigo

Foi utilizado o Sistema Operacional Linux, uma distribuição Ubuntu, versão 18.04.03 LTS para ser mais preciso.

Python na versão 3.6 e o editor de códigos [Visual Studio Code](https://blog.geekhunter.com.br/melhores-extensoes-para-visual-studio-code-em-2020/).

## Flask Tutorial

Então, sem muita enrolação, vamos começar a falar diretamente mais de códigos com um tutorial especial do framework flask!

### **Preparando o ambiente**

O primeiro passo é criar um diretório onde você vai salvar os seus exemplos de Flask. No meu caso eu escolhi criar o diretório “flask” dentro do diretório de “Documentos”.

Você pode fazer isso via terminal. Navegue até o Diretório “Documentos” e crie o diretório “flask”.

Se você já tem familiaridade com comandos no terminal, vai ser super tranquilo pra você, caso não tenha experiência com linha de comando, não se importe em criar diretórios e arquivos utilizando a interface gráfica do seu sistema.

Porém, alguns comando deverão ser digitados no terminal, então vale a pena já ir treinando. 

Abra o seu terminal e digite os comandos:

```
cd Documentos
mkdir flask
```

Deve ficar como mostrado na imagem abaixo:

![flask python](https://blog-geek-midia.s3.amazonaws.com/wp-content/uploads/2020/01/31184542/1-1.png)

Repare que o terminal não nos deu nenhuma saída visual após executarmos o comando “mkdir flask”, mas não se preocupe, nesse caso é a forma dele nos dizer que está tudo bem e o diretório foi criado. Caso houvesse algum erro seríamos avisados.

Bom, criado o nosso diretório para organizar os nossos exemplos agora podemos começar a desenvolver.

Vamos acessar o diretório “flask” e criar um diretório chamado “hello_world” e dessa vez já navegar até ele, que vai conter os nossos primeiros códigos em Flask:

```
cd flask
mkdir hello_world
cd hello_world
```

Até agora temos o diretório “flask” que irá conter os nosso exemplos, dentro dele temos o diretório “hello_world” que será o nosso primeiro exemplo.

Ficará assim:

![flask hello world](https://blog-geek-midia.s3.amazonaws.com/wp-content/uploads/2020/01/31184556/2-1.png)

Agora, estando dentro do diretório “hello_world” precisamos criar um ambiente de desenvolvimento virtual, que no Python é chamado de “venv”.

Esse ambiente virtual é isolado, nos permitindo instalar dependências apenas para o projeto que estamos trabalhando. Para criar esse ambiente virtual basta usar seguinte comando:

```
python3 -m venv venv
```

Esse comando pode ser explicado em duas partes:

A primeira “`python3 -m venv`”, diz ao Python para criar um ambiente virtual.

A segunda “`venv`”, venv é o nome que você escolhe para o seu ambiente virtual.

![flask tutorial](https://blog-geek-midia.s3.amazonaws.com/wp-content/uploads/2020/01/31184607/3-1.png)

Após criar o ambiente virtual use o comando “ls” para verificar que um diretório chamado “venv” foi criado dentro do nosso diretório “hello_world”. Se ao criar o ambiente virtual você escolheu o nome “ambiente_hello_world”, o diretório criado será o “ambiente_hello_world”. Eu sugiro que você siga conforme está no exemplo.

Nesse passo iremos ativar o nosso ambiente virtual com o seguinte comando:

```
source venv/bin/activate
```

Até então temos:

![flask ambiente virtual](https://blog-geek-midia.s3.amazonaws.com/wp-content/uploads/2020/01/31184616/4-1.png)

Repare que agora temos (venv) no início do nosso terminal indicando que estamos no ambiente virtual. Para desativar o ambiente virtual o comando usado é o “deactivate”, mas não utilize-o ainda, todos os comandos a seguir devem ser executados com o ambiente virtual ativado.

### **Utilizando o PIP**

O pip é instalador de pacotes do Python. A primeira coisa que vamos fazer é atualizá-lo com o seguinte comando:

```
pip install --upgrade pip
```

A versão atual, no momento que este artigo está sendo escrito é a 20.0.2

![Flask PIP](https://blog-geek-midia.s3.amazonaws.com/wp-content/uploads/2020/01/31184623/5-1.png)

### **Instalando o Flask**

Agora vamos instalar o Flask com o comando:

```
pip install flask
```

Já temos o necessário para escrever o nosso primeiro código em Flask.

![instalar flask](https://blog-geek-midia.s3.amazonaws.com/wp-content/uploads/2020/01/31184632/6-1.png)

Agora, para facilitar vamos usar um editor de códigos, eu vou utilizar o Visual Studio Code, porém, fique a vontade para usar o de sua preferência.

O nosso primeiro arquivo vai se chamar “application.py” ele será responsável por executar a nossa aplicação. Você pode criá-lo via terminal ou diretamente no seu editor de texto.

Se você estiver no Visual Studio Code, assim como eu, ele poderá criar um diretório “.vscode” que irá conter um arquivo “settings.json”, porém, ele não será importante para nós nesse momento, podemos ignorá-lo.

### **Escrevendo o primeiro código em Flask**

Chegou a hora de por a mão na massa para valer, vamos lá!

#### **Executando o código**

Antes de executarmos o código precisamos exportar a variável FLASK_APP que é necessária para dizer ao Flask como carregar a aplicação.

E já vamos aproveitar para ativar o modo debug exportando a variável FLASK_DEBUG, que já atualiza a nossa aplicação sempre que fazemos alguma alteração no código. Faremos isso com os seguintes comandos:

```
export FLASK_APP=applicaiton.py
export FLASK_DEBUG=1
```

Confira como ficou:

![código flask](https://blog-geek-midia.s3.amazonaws.com/wp-content/uploads/2020/01/31184847/7-2.png)

Agora podemos rodar a nossa aplicação com o seguinte comando

```
flask run
Voilá:
```

![flask run](https://blog-geek-midia.s3.amazonaws.com/wp-content/uploads/2020/01/31184902/8-2.png)

Por fim, acesse o endereço [http://127.0.0.1:5000](http://127.0.0.1:5000/). Assim finalizamos o primeiro exemplo em Flask!

Se você chegou até aqui e conseguiu visualizar o resultado no seu navegador, parabéns!

E agora você deve estar dizendo “Isso foi muito simples”, “Eu gostei do Flask, quero aprender mais!”.

Vamos aprender um pouco mais sobre as rotas e passar alguns parâmetros para elas!

Como estamos iniciando, vamos criar um projeto novo, a repetição irá ajudar você a memorizar a estrutura do projeto, portanto evite copiar e colar, digite os comandos e os códigos novamente.

A primeira coisa a fazer é desativar o ambiente virtual, pois iremos criar um novo. Use o comando:

```
deactivate
```

Confira como ficará:

![img](https://blog-geek-midia.s3.amazonaws.com/wp-content/uploads/2020/01/31184925/9-2.png)

Agora vamos criar um novo projeto dentro do diretório flask, esse exemplo terá o nome de “rotas0” para mostrar um pouco mais sobre a utilização das rotas e como passar um parâmetro para elas. Para isso precisamos voltar um diretório, use o comando:

```
cd ..
```

![img](https://blog-geek-midia.s3.amazonaws.com/wp-content/uploads/2020/01/31184938/10-2.png)

Neste momento eu vou descrever os passos e deixar os comandos utilizados, caso você tenha alguma dúvida sobre a criação do projeto, volte no primeiro exemplo para mais detalhes.

#### Criando a pasta do projeto

```
mkdir rotas0
```

#### Acessando o diretório criado

```
cd rotas0
```

#### Criando o ambiente virtual

```
python3 -m venv venv
```

#### Ativando o ambiente virtual

```
source venv/bin/activate
```

#### Atualizando o pip

```
pip install --upgrade pip
```

#### Instalando o Flask

```
pip install flask
```

Agora é só criar o arquivo “application.py” que contém o nosso código Flask.

Isso é o suficiente para um primeiro contato com o Flask. Faça agora alguns testes, tente criar rotas novas e trabalhar com os argumentos vindos delas.

Qualquer dúvida, deixe seu comentário!