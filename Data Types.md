
**ECMAScript** ==> Orgão que padroniza o JS.

# Data Types
- Primitive/Primitive value
- Structural
- Structural Primitive

### Primitive
- String
- Number
- Boolean
- undefined
- Symbol
- BigInt

### Structural
- **Object**
	- Array
	- Map
	- Set
	- Date
	- ...
- Function

### Structural Root Primitive
- null

~={orange}string=~ ==> Cadeia de caracteres.
	Valores são atribuídos por meio de:	
```js
"" // aspas duplas
'' // aspas simples
`` // template literals ou template strings ==> Também permitem múltiplas linhas. Além disso permitem a interpolação/expressões de linguagem. 
```

~={orange}number=~ ==> Identificadores para números.
```js
33       // inteiros
	12.5     // reais - double
NaN      // Not a Number
Infinity // infinito
```

~={orange}boolean=~ ==> Booleano. Apenas dois valores.
```js
true  // verdadeiro
false // falso
```

~={orange}undefined=~ ==> Indefinido. ==> Represents the lack of any assigned value. 

~={orange}null=~ ==>
- Nulo
- Objeto que não possui conteúdo
- != ~={orange}undefined=~
- **null represents a value intentionally defined as "blank"**

~={orange}Object=~ ==> Dado estrutural.
- Propriedades/Atributos
- Funcionalidades/Métodos
```js
{propriedade: "valor"}
// Ex.:
{
name: "Carlos",
age: 23,
floor: function(){
	console.log('floor')
},
}
```

~={orange}Array=~ ==> Lista.
- Agrupamento de dados
```js
// Ex.:
[
"Leite",
"Ovos",
2,
3,
]
```

