# Closures

Closure é uma função que "memoriza" seu contexto léxico (ou ambiente) no qual foi criada.

```jsx
const myClosure = function(param1){
    return function (param2) {
        return param1 + param2;
    }
};

//chamando função myClosure

const newFunc = myClosure(5); // 5 = param1
newFunc(4); // 9 <--resultado
```

 

Quando utilizamos Closure, como no exemplo a cima, enviamos o primeiro parâmetro (5) que será memorizado e criamos uma nova instância de **myClosure** armazenada em **newFunc**, as chamativas da função **newFunc** irá fazer a soma do valor enviado com o valor memorizado (4 + 5 = 9).

Método com parâmetro privado

```jsx
const myClosure = function(){
		var data = 50;// parametro privado
    this.getData = function () {// método publico
        return data;
    }
};

//chamando função myClosure

const newFunc = new myClosure();
newFunc.data // undefined
newFunc.getData(); // 50 <--resultado
```