## Tipagem 

A tipagem de uma linguagem de programação é a forma como ela trata os tipos de dados. Em React e TypeScript, podemos tipar os componentes, props e estados.

### Tipagem de componentes

```typescript

import React from 'react'
 
interface Props { // Criamos uma interface Props, interface é um tipo de dado que define a estrutura de um objeto
    nome: string // Tipamos a prop nome como string
}

const Componente: React.FC<Props> = ({ nome }) => { // Tipamos o componente com o tipo React.FC e passamos o tipo Props
    return <h1>{nome}</h1> // O componente recebe a prop nome
}

export default Componente

```

### Tipagem de props

```typescript

import React from 'react'

interface Props {
    nome: string
}

const Componente: React.FC<Props> = ({ nome }) => {
    return <h1>{nome}</h1>
}


```

### Tipagem de estados

```typescript

import React, { useState } from 'react'

interface Props {
    nome: string
}

const Componente: React.FC<Props> = ({ nome }) => {
    const [state, setState] = useState<string>('') // Tipamos o estado com o tipo string

    return <h1>{nome}</h1>
}

```





