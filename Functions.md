
### Function Statement
```js
function createPhrases(){
	console.log("Bish Bash Bosh")
}
// Call function
createPhrases()
```

```js
// function expression / function anonymous
const sum = function(x, y){
	let result = x + y
	return result
}
let num1 = 34
let num2 = 25

sum(2,3) // arguments i.e. args
console.log{`A soma eh ${sum(num1, num2)}`}
```

### Function Scope
```js
let subject = "create video" // 1

function createThink(subject){ // 2
	subject = "study"
	return subject
}

console.log(createThink(subject))
console.log(subject)
// A variável subject é diferente nos dois casos pois, no escopo da função, ela existe como uma variável separada, não possuindo relação com a variável declarada em 1.
```

### Function Hoisting
```js
// Neste caso a função é chamada com sucesso
sayMyName()

function sayMyName(){
	console.log("Heisenberg")
}
// Neste caso a função não é chamada com sucesso
walterResponse()

const walterResponse = function(){
	console.log("You're goddamn right")
}
// i.e. ao realizar uma função pela maneira de expressão (function expression / function anonymous), ela não sofrerá elevação
```

### Arrow Function
```js
// Geralmente atribuída por constante
// Não sofre hoisting
const sayMyName = () => {
	console.log("Heisenberg")
}

sayMyName()
```

### Callback Function
```js
function sayMyName(name) {
	console.log("Antes de executar a callback function")
	
	name()
	
	console.log("Depois de executar a callback function")
}

sayMyName(
	() => 
	{
		console.log("Estou em uma callback")	
	}
)
```

### Function Constructor
```js
// expressão new
// criar um novo objeto
// this keyword
function Person(){
	this.name = name
	this.walk = function() {
		return this.name "andando"
	}
}
const carlos = new Person("Carlos")
const joao = new Person("Joao")
console.log(carlos)
console.log(joao.walk())
```