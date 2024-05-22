## Tipagem 

A tipagem de uma linguagem de programação é a forma como ela trata os tipos de dados. Em React e TypeScript, podemos tipar os componentes, props e estados.

### JS VS TS

- JavaScript é uma linguagem de programação de alto nível, interpretada e orientada a objetos.
- TypeScript é um superconjunto de JavaScript que adiciona tipagem estática à linguagem.

#### Vantagens do TypeScript

- Evita erros de tipagem
- Facilita a manutenção do código
- Melhora a produtividade
- Facilita a leitura do código

#### Exemplo de código em JavaScript

```javascript

const soma = (a, b) => {
    return a + b
}

```

#### Exemplo de código em TypeScript

```typescript

const soma = (a: number, b: number): number => {
    return a + b
}

```

### JSX VS TSX

- JSX é a extensão de arquivo usada para arquivos JavaScript que contêm código React.
- TSX é a extensão de arquivo usada para arquivos TypeScript que contêm código React.

### Tipos primitivos

- string
- number
- boolean
- null
- undefined

### Tipos de objetos

- object
- array
- function

### Tipos de dados

- any
- void
- never

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





