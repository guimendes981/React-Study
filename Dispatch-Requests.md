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


## Redux

#### Redux é uma biblioteca que nos ajuda a gerenciar o estado da aplicação de forma centralizada.

#### Para usar o Redux, precisamos instalar as dependências `redux` e `react-redux`.

```bash

npm install redux react-redux

```

#### Para criar um store, usamos a função `createStore()` do Redux.

```javascript

import { createStore } from 'redux'

const store = createStore(reducer)

```

#### Para criar um reducer, usamos uma função que recebe o estado atual e uma ação, e retorna um novo estado.

```javascript

function reducer(state = initialState, action) {
    switch (action.type) {
        case 'INCREMENT':
            return { count: state.count + 1 }
        case 'DECREMENT':
            return { count: state.count - 1 }
        default:
            return state
    }
}

```

#### Para usar o Redux em um componente, usamos o componente `Provider` do `react-redux`.

```javascript

import { Provider } from 'react-redux'

ReactDOM.render(
    <Provider store={store}>
        <App />
    </Provider>,
    document.getElementById('root')
)

```

#### Para acessar o estado do Redux em um componente, usamos o hook `useSelector` do `react-redux`.

```javascript

import { useSelector } from 'react-redux'

function App() {
    const count = useSelector(state => state.count)

    return (
        <div>
            <h1>{count}</h1>
        </div>
    )
}

```

#### Para disparar uma ação no Redux em um componente, usamos o hook `useDispatch` do `react-redux`.

```javascript

import { useDispatch } from 'react-redux'

function App() {
    const dispatch = useDispatch()

    return (
        <div>
            <button onClick={() => dispatch({ type: 'INCREMENT' })}>Increment</button>
            <button onClick={() => dispatch({ type: 'DECREMENT' })}>Decrement</button>
        </div>
    )
}

```




