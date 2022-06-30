# Currying

Função Curry ou parcial é um método que recebe um parâmetro inicial e retorna uma função curried, que tem como finalidade receber N parâmetros a mais.

```jsx
function myCurry(x, y){
	if(y === undefined){
		return function(y){ //retorna um closure caso y for undefined
			return x + y;
		}
	}

	return x + y;
}

myCurry(5)(5); // retorna 10
```
