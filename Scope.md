
**Escopo** ==> Determina a visibilidade de alguma variável.

### Block Statement
```js
{
	let x = 0
	console.log(x)
} 
```

O bloco criará um novo escopo. Chamamos de "Block-Scoped"

### var
```js
// var é global e poderá funcionar fora de um escopo de bloco
// Além de ser global, é também local
// Hoisting ==> Elevação. Eleva o x.
console.log("> existe x antes do bloco?", x)

{
	var x = 0
}

console.log("> existe x antes do bloco?", x)
// A primeira chamada da função retornará undefined, pois x possui escopo global, portanto existe, porém 
```

### let e const
```js
// const e let são locais
console.log("> existe y", y) // 1
{
	console.log("> existe y", y) // 2
	let y = 0
	console.log("> existe y", y) // 3
}
// 1 Não funcionará pois não está dentro do escopo
// 2 Não funcionará pois y ainda não foi inicializado
// 3 Funcionará
// O escopo funciona da mesma forma para const, a única diferença sendo a imutabilidade do valor atribuído ao mesmo
```

### Variable Naming
- JS é case-sensistive
- JS aceita a cadeia de caracteres Unicode

#### Permitido
- Iniciar com caracteres especiais: $ _
- Iniciar com letras
- Colocar acentos

#### Não é Permitido
- Iniciar com números
- Inserir espaços vazios no nome

#### Ideal
- Criar nomes coerentes, que expliquem o que a variável é ou a sua função
- camelCase
- snake_case
- Escrever em inglês

### Variable Declaration
```js
let name, age, isHuman // Agrupamento de declarações
name = "Carlos"
age = 23
isHuman = true
```

