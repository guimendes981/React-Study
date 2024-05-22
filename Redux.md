## Redux.js

Redux é uma biblioteca JavaScript de código aberto para gerenciar o estado de um aplicativo. É mais comumente usado com bibliotecas como React ou Angular para criar interfaces de usuário interativas. O Redux foi criado por Dan Abramov e Andrew Clark em 2015.

### Conceitos principais

- **Store**: A store é um objeto que contém o estado da aplicação. Ela é a única fonte de verdade do estado e é acessível por todos os componentes da aplicação.

- **Dispatch**: O dispatch é uma função que envia uma action para a store. Ele é usado para disparar uma mudança de estado na aplicação.

- **Actions**: As actions são objetos que descrevem uma mudança de estado. Elas são enviadas para a store e são processadas pelos reducers.

- **Reducers**: Os reducers são funções que especificam como o estado da aplicação muda em resposta a uma action. Eles recebem o estado atual e uma action como argumentos e retornam o novo estado.

- **Middleware**: O middleware é uma camada entre o dispatch e os reducers que permite

### Instalação

Para instalar o Redux em um projeto, basta executar o seguinte comando:

```bash

npm install redux

```

Depois de instalar o Redux, é possível criar uma store e utilizar os conceitos de actions, reducers e dispatch para gerenciar o estado da aplicação.

### Exemplo

A seguir, um exemplo de como criar uma store e utilizar os conceitos de actions, reducers e dispatch em um projeto React:

```javascript

import { createStore } from 'redux'

// Reducer
const counterReducer = (state = 0, action) => {
    switch (action.type) {
        case 'INCREMENT':
            return state + 1
        case 'DECREMENT':
            return state - 1
        default:
            return state
    }
}

// Store

const store = createStore(counterReducer)

// Actions

const increment = () => {
    return {
        type: 'INCREMENT'
    }
}

const decrement = () => {
    return {
        type: 'DECREMENT'
    }
}

// Dispatch

store.dispatch(increment())

console.log(store.getState()) // Output: 1

store.dispatch(decrement())

console.log(store.getState()) // Output: 0

```

Neste exemplo, criamos um reducer `counterReducer` que especifica como o estado da aplicação muda em resposta a uma action. Em seguida, criamos uma store com o reducer e utilizamos as actions `increment` e `decrement` para disparar mudanças de estado na aplicação. Por fim, utilizamos o dispatch para enviar as actions para a store e exibimos o estado atual da aplicação no console.

O Redux é uma ferramenta poderosa para gerenciar o estado de um aplicativo e facilita a comunicação entre os componentes da aplicação. Ele é amplamente utilizado em aplicações React para manter o estado da aplicação de forma centralizada e previsível.
[]: # (end)


