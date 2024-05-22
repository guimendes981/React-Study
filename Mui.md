## Material UI

Material UI é uma biblioteca de componentes React que implementa o Material Design, um sistema de design criado pelo Google. O Material Design é um sistema de design que foi criado pelo Google em 2014 e é utilizado em diversos produtos da empresa, como o Android e o Google Chrome.

Material UI fornece uma série de componentes prontos para serem utilizados em aplicações React, como botões, barras de navegação, tabelas, entre outros. Além disso, a biblioteca também oferece estilos e temas que podem ser utilizados para personalizar a aparência dos componentes.

### Instalação

Para instalar o Material UI em um projeto React, basta executar o seguinte comando:

```bash

npm install @mui/material @emotion/react @emotion/styled

```

Depois de instalar a biblioteca, é possível importar os componentes desejados e utilizá-los em um projeto React.

### Exemplo

A seguir, um exemplo de como utilizar o componente `Button` do Material UI em um projeto React:

```javascript

import React from 'react'

import Button from '@mui/material/Button'

const App = () => {
    return (
        <Button variant="contained" color="primary">
            Hello, Material UI!
        </Button>
    )
}

export default App

```

Neste exemplo, importamos o componente `Button` do Material UI e o utilizamos em um componente funcional `App`. O botão possui as propriedades `variant` e `color`, que definem o estilo e a cor do botão, respectivamente.