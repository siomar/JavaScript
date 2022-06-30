# Promise

É um objeto para tratar com processos assíncrono (Promise de "Promessa”).

```jsx
const promessa = new Promise(
	(resolve,reject) => {
		try {
			resolve(functionX());//retorno de sucesso
		} catch(error){
			reject(error);//retorno de erro
		}
	}
);

promessa.then(
	() = >{}// case sucesso
).catch(
	() => {}// case rejeicao
).finally(
	() => {}// case finalizado
)
```
