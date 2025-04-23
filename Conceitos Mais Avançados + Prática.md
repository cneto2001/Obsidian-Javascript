### Concatenação e Interpolação
```js
let age, isHuman

name = "Carlos"
age = 18
isHuman = true
// Escrita de texto + variáveis
console.log("A idade do " + name + " é de " + age " anos.")

// Interpolando valores com template literals or template strings
console.log(`O ${name} tem ${age} anos de idade.`)
```

### Objects
```js
const person = {
	name: "John",
	age: 30,
	overtimeHours: 15.5,
	isAdmin: true, 
}
// Acessar um dado específico do objeto
console.log(person.age)
```

### Arrays
```js
// A primeira posição é 0

const animals = [
	"Lion", // pos 0
	"Monkey", // pos 1
	"Cat", // pos 2
	{
		name: "Raven",
		age: 2,
	},
]
// Acessar valores dentro do array
animals[2] // acessa o valor Cat
console.log(animals[3]) // Mostra o valor da variável (Raven e 2) no console
// É recomendado utilizar apenas dados do mesmo tipo em um array. Ex.:
const people = [
	"Marcus",
	"David",
	"Alek",
	"Sabrina",
	"Julia",
	"Stephanie",
]

const evenNums = [
	2,
	4,
	6,
	8,
	10
]

const classes = [
	{
		class: "Mage",
		level: 2,
		isVulnerable: true,
	},
	{
		class: "Paladin",
		level: 3,
		isVulnerable: false,
	},
	{
		class: "Ranger",
		level: 3,
		isVulnerable: true,
	},
	{
		class: "Fighter",
		level: 2,
		isVulnerable: false,
	},
]
```

