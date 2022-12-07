# 🏓 Api_Ping-Pong 🏓

API desenvolvida em Python para um trabalho da faculdade, cuja função é receber um parâmetro "Ping" e retornar "Pong" e caso receba "Pong" retorna "Ping". Optamos por utilizar o Replit para deploy da API

## Tecnologias Utilizadas 🤖

- Flask é um micro-framework utilizado para criar microsserviços (APIs). 
- Json é um dicionario do Python utilizado para realizar requisições. 
- Replit é um site onde podemos criar/desenvolver/manter aplicações online.

## Pré-Requisítos 

Para iniciarmos nossa API é necessario acessar o link:

>https://replit.com

- Baixar a biblioteca do Flask, para isso na aba "Ferramentas" acesse "Packages" e pesquise por Flask

## Início 

Para dar inicio a nossa API precisamos importa a biblioteca Flask e Json e inicializa-lá. Para isso utilizamos os comandos:
````
from flask import Flask,jsonify,request
app = Flask(__name__)
````

## Rota

Para definirmos a rota de destino de cada função utilizamos o comando:
````
@app.route('{endereço}')
````

## Programação 

Criaremos 3 funções básicas:

- 1ª Função: homepage() onde estará sua página inicial
````
@app.route('/')
def homepage():
  return 'API no ar!'
````
- 2ª Função: ping() onde irá retornar "Pong"
````
@app.route('/ping')
def ping():
  return jsonify('Pong')
````

- 3ª Função: pong() onde irá retornar "Ping"

````
@app.route('/pong')
def pong():
  return jsonify ('Ping')
````

## Fim

E por fim para terminar nossa API basta acrescentarmos o comando de host do Replit
````
app.run(host='0.0.0.0')
````
## Como rodar

Para rodar sua API basta acessar o link gerado pelo Replit, caso queira acessar o nosso, segue o link 
>https://api.vocs.repl.co/

## Código
>https://replit.com/@vocs/API#main.py

### Desenvolvedores

Créditos ao Leandro Pellegrini Fodi e Vítor de Oliveira Celestino da Silva

