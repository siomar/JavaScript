# Funções

Funções no JavaScript são Objetos de primeira classe que fornecem um escopo próprio, usadas para definir um conjunto de instruções que executa uma tarefa.

Declaração normal

```jsx
function myFunction(a, b){// parametros a e b
	//escopo da função
	return a + b;
}
```

Função Construtora

```jsx
function Carro(modelo, ano) {
	//Boa prática usar a Primeira letra como maiuscula para declarar uma funcao construtora
	this.modelo = modelo;
	this.ano = ano;
}

const carro1 = new Carro("HB20", "2019");// uso de new para criar uma instancia de Carro
```

Função anonima

```jsx
const myFunction = function() {
	//escopo da função
	return 2 + 5;
}
```

Arrow Function

```jsx
const arrow = () => {// arrow por conta do '=>'
	//escopo da função
};
```

Função assíncrona

```jsx
const assincrono = async () => {
	//escopo da função
	//uso de await para executar um processo de forma sincrona

	const cep = await getCEP("12252-342");

	return cep;
};
```
