## Contextos em React

Contextos são uma forma de compartilhar dados entre componentes sem precisar passar props manualmente em cada nível da árvore de componentes.

### Criando um contexto

Para criar um contexto, usamos a função `createContext` do React.

```javascript

// Cria um contexto
const Context = createContext()

```

### Provedor

Para compartilhar dados com os componentes filhos, usamos o componente `Provider`.

```javascript

// Provedor
<Context.Provider value={data}>
    <Componente />
</Context.Provider>

```

### Consumidor

Para consumir os dados do contexto, usamos o componente `Consumer`.

```javascript

// Consumidor
<Context.Consumer>
    {data => <Componente data={data} />}

</Context.Consumer>

```

### useContext

Podemos usar o hook `useContext` para consumir os dados do contexto.

```javascript

// Usa o contexto
const data = useContext(Context)

```

### Exemplo

```javascript

// Cria um contexto
const Context = createContext()

// Provedor
<Context.Provider value={data}>
    <Componente />
</Context.Provider>

// Consumidor
<Context.Consumer>
    {data => <Componente data={data} />}
</Context.Consumer>

// Usa o contexto
const data = useContext(Context)

```

### Exercícios
