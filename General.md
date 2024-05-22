## Outros termos e funções do react

### Async

Async é uma palavra-chave que indica que uma função é assíncrona. Funções assíncronas são funções que executam de forma assíncrona, ou seja, não bloqueiam a execução do código.

```javascript

const fetchData = async () => {
    const response = await fetch('https://api.example.com/data')
    const data = await response.json()
    console.log(data)
}

```