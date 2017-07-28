# Utilizando o Json Server

As vezes precisamos de um banco de dados simples, rápido e sem muita complicação.

Utilizar JSON já é uma unanimidade, mas sempre temos que pensar em algo para gerenciar e servir esse aquivo.

Criar uma aplicação que lê esse arquivo e serve no formato rest :(

Com o Json Server isso não é necessário.

Ele é um aplicativo feito em NodeJS que serve seus arquivos JSON.

Inicialmente é feito para ambiente de desenvolvimento, mockups e testes em geral.

## Instalando

```
npm install -g json-server
```

## Criando um JSON

Vamos criar um json localmente com algo semelhante a:

```
{
	"produtos" : [
		{
			"id": 1,
			"name": "Pão Francês"
		}
	]
}
```

Salvando o arquivo como db.json.

Depois disso, basta executar o comando

```
json-server --watch db.json
```

O --watch faz com que qualquer modificação no arquivo seja vista pelo servidor.

Agora, temos acesso ao servidor, indicado no terminal :D

```
Resources
http://localhost:3000/produtos

Home
http://localhost:3000
```

Basta acessar o servidor no seu navegador e ter uma api pronta para ser utilizada.

Seu servidor REST está pronto para receber POST's, GET's ou DELETE's.

É isso ;)

Material baseado nas explicações vistas aqui:

https://www.youtube.com/watch?v=VrPByfYy9PE

Aplicativo insteressante para testar:

https://www.getpostman.com/