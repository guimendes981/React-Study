# Loops de repetição e if/else

Loops são estruturas de repetição que nos permitem executar um bloco de código várias vezes. Entre os mais usados temos os seguintes:

### for

Usamos o for para percorrer um bloco de código um número específico de vezes.

```javascript

for (let i = 0; i < 10; i++) {
    console.log(i)
}

```

### forEach

Usamos o forEach para percorrer um array, ele recebe uma função de callback que é executada para cada item do array.

```javascript

const array = [1, 2, 3, 4, 5]

array.forEach(item => {
    console.log(item)
})

```

### map

Usamos o map para percorrer um array e retornar um novo array com os itens modificados.

```javascript

const array = [1, 2, 3, 4, 5]

const newArray = array.map(item => item * 2)

console.log(newArray)

```

### while

Usamos o while para executar um bloco de código enquanto uma condição for verdadeira.

```javascript

let i = 0

while (i < 10) {
    console.log(i)
    i++
}

```

### do...while

Usamos o do...while para executar um bloco de código uma vez e depois repetir enquanto uma condição for verdadeira.

```javascript

let i = 0

do {
    console.log(i)
    i++
} while (i < 10)

```



