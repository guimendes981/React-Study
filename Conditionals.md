# Condicionais e verificações

Usamos condicionais e verificações para executar um bloco de código dependendo de uma condição.

### if/else

Usamos o if/else para executar um bloco de código se uma condição for verdadeira e outro bloco se a condição for falsa.

```javascript

const idade = 18

if (idade >= 18) {
    console.log('Maior de idade')
} else {
    console.log('Menor de idade')
}

```

### Ternários

Usamos o operador ternário para fazer uma operação condicional em uma linha.

```javascript

const idade = 18

const mensagem = idade >= 18 ? 'Maior de idade' : 'Menor de idade'

console.log(mensagem)

```

### switch

Usamos o switch para executar um bloco de código dependendo do valor de uma variável.

```javascript

const dia = 'segunda'

switch (dia) {
    case 'segunda':
        console.log('Hoje é segunda-feira')
        break
    case 'terça':
        console.log('Hoje é terça-feira')
        break
    default:
        console.log('Hoje é outro dia')
}

```

### break

Usamos o break para sair de um loop ou de um switch.

```javascript

for (let i = 0; i < 10; i++) {
    if (i === 5) {
        break
    }
    console.log(i)
}

```