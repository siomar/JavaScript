# Callback

Função callback é uma método que recebe outro método como parâmetro

```jsx
function myCallback(outrometodo){
	//escopo do metodo
	var a = 2, b = 2;

	outrometodo(a+b);
}

myCallback(//chamando um callback
	(retorno) => {
		console.log(retorno);// 4
	}
);
```
