# Exemplo de formulário em React

Neste exemplo, criamos um formulário com dois campos de texto e um botão de envio. Usamos o hook `useForm` para registrar os campos de texto e o evento de envio do formulário.

Quando o formulário é enviado, a função `onSubmit` é chamada e exibe os dados no console.

Para usar o hook `useForm`, importamos a função `useForm` do pacote `react-hook-form`.

```bash

npm install react-hook-form

```

Depois, declaramos a função `FormExample` e usamos o hook `useForm` para registrar os campos de texto e o evento de envio do formulário.

```javascript

const { register, handleSubmit } = useForm()

```

Em seguida, criamos a função `onSubmit` para exibir os dados no console.

```javascript

const onSubmit = data => {
    console.log(data)
}

```

Por fim, criamos o formulário com os campos de texto e o botão de envio.

```javascript

<form onSubmit={handleSubmit(onSubmit)}>
    <input type="text" name="nome" ref={register} />
    <input type="email" name="email" ref={register} />
    <button type="submit">Enviar</button>

</form>


```

Quando o formulário é enviado, a função `onSubmit` é chamada e exibe os dados no console.


Vamos criar um formulário em React usando o hook `useForm`.

```javascript

import React from 'react'
import { useForm } from 'react-hook-form'


const FormExample = () => {
    const { register, handleSubmit } = useForm()

    const onSubmit = data => {
        console.log(data)
    }

    return (
        <form onSubmit={handleSubmit(onSubmit)}>
            <input type="text" name="nome" ref={register} />
            <input type="email" name="email" ref={register} />
            <button type="submit">Enviar</button>
        </form>
    )
}

export default FormExample

```

