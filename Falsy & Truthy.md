
### FALSY
- Quando um valor é considerado ~={pink}false=~ em contextos onde um booleano é obrigatório (condicionais e loops)
- ~={pink}false=~
- 0
- -0
- ""
- ~={orange}null=~
- ~={orange}undefined=~
- ~={orange}NaN=~

#### Ex.:
```js
console.log(0 ? "verdadeiro" : "falso") // Retorno: Falso
console.log("" ? "verdadeiro" : "falso") // Reorno: Falso
```

### TRUTHY
- Quando um valor é considerado ~={pink}true=~ em contextos onde um booleano é obrigatório (condicionais e loops)
- ~={pink}true=~
- {}
- []
- 1
- 3.23
- "0"
- "false"
- -1
- Infinity
- -Infinity

**Ex.:**
```js
console.log({} ? "verdadeiro" : "falso") // Retorna verdadeiro
console.log(Infinity ? "verdadeiro" : "falso") // Retorna verdadeiro
```