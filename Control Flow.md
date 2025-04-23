
### if...else
```js
let temperature = 38
if(temperature >= 37.5){
	console.log("Febre")
} else if(temperature < 37.5 && temperature >= 37){
	console.log("Febre Moderada")
} else {
	console.log("Temperatura Normal")
}
```

### Switch
```js
function calculate(num1, operator, num2) {
	let result
	
	switch(operator) {
		case '+':
			result = num1 + num2
			break
		case '-':
			result = num1 - num2
			break
		case '*':
			result = num1 * num2
			break
		case '/':
			result = num1 / num2
			break
		default:
			console.log("não implementado")
			break
	}
	
}

console.log(calculate(4, '%', 8))
```

### throw & try...catch
```js
// throw
function sayMyName(name="") {
	if(name === ""){
		throw new Error("Nome é um campo obrigatório")
	}
}

//try...catch
try {
	sayMyName()
} catch(e) {
	console.log(e)
}

console.log("Após a função de erro")
```

### for
```js
// break - Para a execução do loop
// continue - Pula a execução do momento
for(let i = 0; i <= 10; i++){
	console.log(i)
}
```
### while
```js
let i = 0
while(i < 10){
	console.log(i)
	
	i++
}
```
### for...of
```js
let name = "Waltuh"
let names = ["Dinho", "Lavalão", "falleN"]

for (let char of name){
	console.log(char) // Retorna: W a l t u h 
}

for (let element of names){
	console.log(element)
}
```
### for...in
```js
let person = {
	name: "Waltuh",
	age: 30,
	weight: 88.6,
}

for(let property in person){
	console.log(property)
	console.log(person[property])
}
```