
**JS é uma linguagem baseada em protótipos (prototype-based language).**



### `__proto__`
- Propriedade criada referenciando um objeto ascendente(anterior).
- Contém várias funcionalidades e propriedades que são herdadas na criação de um tipo de dado. Isso é chamado de prototype chain.
- A maioria dos tipos de dado no **JS** são encapsulados por um objeto, trazendo várias funcionalidades, como o .length para o tipo String.

### Type Conversion(typecasting) vs Type Coersion

~={pink}Type Conversion=~ ==> Dev explicitamente altera um dado de um tipo para outro.

~={pink}Type Coersion=~ ==> Javascript implicitamente realiza a troca implicitamente. Além disso, o JS também, em alguns casos, utiliza o Type Conversion de forma implícita.

```js
// Coersion
console.log('9' + 5) // Retorna 95, concatenação. Number => String
// Conversion
console.log(Number('9') + 5) // String => Number. Retorna 14, soma
```

### Strings e Arrays

###### Tamanho de Strings
```js
let word = "Wenomechainasama"
let num = 739412
console.log(word.length) // Retorna o tamanho da string
console.log(String(num).length) // Retorna a quantidade de números
```
###### Casas Decimais
```js
let num = 461285.218384284
// Retorna o num com duas casas decimais e substitui o ponto pela vírgula
console.log(num.toFixed(2).replace(".", ","))
```

######  Uppercase & Lowercase
```js
let word = "Wenomechainasama"
let word2 = "Tumajarbisaun"
console.log(word.toUpperCase()) // Transforma todas as letras em maiúsculas
console.log(word2.toLowerCase()) // Transforma todas as letras em minúsculas
```

```js
let phrase = "agarafile tha tonai gonabi a gunay"
// Separa a String em partes, sempre que houver um espaço em branco
let splitArray = phrase.split(" ")
// Junta todas as strings no Array, utilizando o underscore como separador
let phraseWithUnderscore = splitArray.join("_") 
console.log(phraseWithUnderscore) /* Retorna a string: 
agarafile_tha_tonai_gonabi_a_gunay */
```

###### Verificar a existência de uma palavra em uma String
```js
let phrase = "Penso logo Existo"
console.log(phrase.includes("logo")) // Retorna verdadeiro. É case-sensistive
```

###### Criar um Array com construtor
```js
let myArray = new Array('a', 'b', 'c')
console.log(myArray)
// Cria um Array com dez posições vazias
let anotherArray = new Array(10)
```

###### Contar elementos de um Array
```js
console.log(["a", "b", "c", "d", "e", "f",].length)
```

###### Transformar uma cadeia de caracteres em elementos de um Array
```js
let word = "Existence"
console.log(Array.from(word))
```

###### Array Methods
```js
let techs = ["html", "css", "js"]
// Adicionar um item no fim de um Array
console.log(techs.push("nodejs"))
// Adicionar um item no início de um Array
console.log(techs.unshift("sql"))
// Remover do fim
techs.pop()
// Remover do começo
techs.shift()
// Pegar somente alguns elementos do Array
console.log(techs.slice(1,3))
// Encontrar a posição de um elemento no Array
let index = techs.indexOf("css")
```