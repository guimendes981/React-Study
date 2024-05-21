# Requisições para API com axios e dispatch de actions com redux-thunk


#### Tipos de requisições HTTP

- GET: Buscar dados
- POST: Enviar dados
- PUT: Atualizar dados
- DELETE: Deletar dados
- PATCH: Atualizar dados, mas de forma parcial


#### Para buscar dados de uma API, podemos usar o axios, que é um cliente HTTP baseado em Promises.

#### Para fazer requisições para uma API, podemos usar o método `axios.get()`, que recebe como parâmetro a URL da API.

```javascript

import axios from 'axios'

axios.get('https://jsonplaceholder.typicode.com/posts')
    .then(response => {
        console.log(response.data)
    })

```

#### Para fazer requisições com métodos diferentes de GET, podemos passar o método como segundo parâmetro do método `axios.get()`.

```javascript

import axios from 'axios'

axios.post('https://jsonplaceholder.typicode.com/posts', {
    title: 'foo',
    body: 'bar',
    userId: 1
})
    .then(response => {   //usamos then para pegar a resposta da requisição e fazer algo com ela
        console.log(response.data)
    })

```


