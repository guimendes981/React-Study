# React-Study
Anotations and examples for React

## Propriedades (Props)

Props são propriedades que passamos para um componente, como se fossem atributos de uma tag HTML.

```javascript

import React from 'react'

function Componente(props) { // props é quem contem as propriedades passadas para o componente
    return (
        <div>
            <h1>{props.titulo}</h1> // props.titulo é a propriedade titulo passada para o componente
            <p>{props.texto}</p> // props.texto é a propriedade texto passada para o componente
        </div>
    )
}

export default Componente

```

```javascript

import React from 'react'

import Componente from './Componente' // Importamos o componente

function App() {
    return (
        <div>
            <Componente 
            titulo="Título do componente"  // Passamos a propriedade titulo para o componente
            texto="Texto do componente"  // Passamos a propriedade texto para o componente
            /> 
        </div>
    )
}

export default App

```

