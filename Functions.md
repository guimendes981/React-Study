## Funções em React

Funções são blocos de código que executam uma tarefa específica. Em React, usamos funções para criar componentes e manipular o estado da aplicação.

### Componentes

Componentes são funções que retornam elementos React. Eles podem ser criados como funções ou classes.

```javascript

// Função que retorna um elemento React
const Componente = () => {
    return <h1>Olá, mundo!</h1>
}

```

### Função comum

Podemos criar funções comuns para executar tarefas específicas.

```javascript

// Função que soma dois números
const soma = (a, b) => {
    return a + b
}

```

### Função anônima

Podemos criar funções anônimas sem nome.

```javascript

// Função anônima que exibe uma mensagem
const mensagem = () => {
    console.log('Olá, mundo!')
}

```

### Arrow function

Arrow functions são uma forma mais curta de escrever funções em JavaScript.

```javascript

// Arrow function que exibe uma mensagem
const mensagem = () => console.log('Olá, mundo!')

```

### Callback

Callbacks são funções que são passadas como argumentos para outras funções.

```javascript

// Função que recebe um callback
const executar = (callback) => {
    callback()
}

// Callback que exibe uma mensagem
const mensagem = () => console.log('Olá, mundo!')

executar(mensagem)

```

### Eventos

Podemos usar funções para manipular eventos em React.

```javascript

// Função que exibe uma mensagem
const mensagem = () => console.log('Olá, mundo!')

// Elemento com evento de clique
<button onClick={mensagem}>Clique aqui</button>

```

### Função assíncrona

Funções assíncronas são funções que retornam uma Promise, permitindo o uso de `await` para esperar a resolução da Promise.

```javascript

 const fetchData = async () => {
     const response = await fetch('https://api.example.com/data')
     const data = await response.json()
     console.log(data)
 }

```

### Promises

Promises são objetos que representam a eventual conclusão ou falha de uma operação assíncrona.

```javascript

// Função que retorna uma Promise

const fetchData = () => {
    return new Promise((resolve, reject) => {
        fetch('https://api.example.com/data')
            .then(response => response.json())
            .then(data => resolve(data))
            .catch(error => reject(error))
    })
}

```