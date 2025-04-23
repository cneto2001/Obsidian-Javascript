
###### Caso no qual ";"  é necessário
```js
/* O JS pensa que deve executar o "1" passando a função como argumento e recebendo de volta outra função */
let number = 1; // ; Utilizado para impedir esse erro

(function(){
	console.log("Olá")
})()
```

###### Operators
- Binary ==> Dois elementos. Ex.: 
```js
let num = 1
num + 1 // + É um operador de soma
```
- Unary ==> Um elemento, cujo valor será incrementalmente modificado:
```js
let num = 1
++num // Aumenta o valor em um
--num // Diminui o valor em um
typeof num // typeof é um operador unário
```
- Ternary
```js
let num = 1
// Se [true] ? faça [ação] : caso contrário [ação]
console.log(true ? "Hello!" : "Nada!")
console.log(num === 1 ? "num = 1" : "num != 1")
```

###### new
- left-hand-side expression
- criar um novo objeto
```js
let name = new String("John")
let age = new Number(117)
// O retorno será composto por dois objetos com suas props e valores
console.log(name, age)
```

###### typeof & delete
```js
const spartan = {
	name: "Noble",
	number: 6,
	isAlive: true,
}
console.log(typeof spartan) // Retorna o tipo. Neste caso, um objeto
// Remove a propriedade, sobrando apenas name & number
delete spartan.isAlive
```

###### Operadores Aritméticos
```js
// Multiplicação: *
console.log(3.2 * 5.5)
// Divisão: /
console.log(12 / 2)
// Soma: +
console.log(12 + 2)
// Subtração
console.log(65 - 18)
// Resto da divisão: %
let remainder
remainder = 11 % 3 // Resultado === 2
// Incremento: ++
let increment = 0
/* Retorna 0 pois, como o operador (++) foi colocado após o nome da variável, o incremento será efetuado somente após, ou seja, o valor estará atualizado apenas na próxima linha */
console.log(increment++) 
console.log(increment) // Retorna 1
console.log(++increment) // Retorna 2, pois o operador foi colocado na frente
// Decremento: --
let decrement = 0
console.log(--decrement) // Retorna -1
console.log(decrement--) // Retorna -1
console.log(decrement) // Retorna -2
// Exponencial: **
console.log(2 ** 3)
```

###### Grouping Operator
```js
// Grouping Operator: ()
// Multiplicação é efetuada primeiro
let total = 2 + 3 * 5 // total === 17
// Soma é efetuada primeiro
total = (2 + 3) * 5 // total === 30
```

