## Materialize CSS

Materialize css é um framework front-end que segue o conceito de Material Design, criado pela Google. O Materialize é um framework que possui uma série de componentes prontos para serem utilizados, como botões, cards, formulários, entre outros. Além disso, o Materialize possui um sistema de grid que facilita a criação de layouts responsivos.

### Instalação

Para instalar o Materialize em um projeto, basta adicionar o link do arquivo CSS do Materialize no arquivo HTML do projeto:

```html

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/materialize/1.0.0/css/materialize.min.css">

```

Depois de adicionar o link do arquivo CSS, é possível utilizar os componentes do Materialize no projeto.

### Exemplo

A seguir, um exemplo de como utilizar o componente `Button` do Materialize em um projeto:

```javascript

import React from 'react'
import 'materialize-css/dist/css/materialize.min.css'

const App = () => {
    return (
        <button className="btn">Hello, Materialize!</button>
    )
}

export default App

```

Neste exemplo, importamos o arquivo CSS do Materialize e utilizamos a classe `btn` para estilizar o botão. O Materialize possui uma série de classes CSS que podem ser utilizadas para estilizar os componentes.

