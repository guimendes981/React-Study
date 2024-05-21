# React-Study
Anotations and examples for React

## Ciclo de vida de um componente usando useEffect

#### 1. Montagem

```javascript

useEffect(() => {
    // Executa uma vez
    // Ideal para fazer requisições
    // componentDidMount

    console.log('Montou')
}, [])

```

#### 2. Atualização

```javascript

useEffect(() => {
    // Executa toda vez que o componente atualiza
    // componentDidUpdate

    console.log('Atualizou')
}), [variavelDeEstado] // Array de dependências que dispara o useEffect toda vez que a variável de estado mudar

```

#### 3. Desmontagem

```javascript

useEffect(() => {
    //Usamos o return para retornar uma função anônima, assim retornamos quando o componente é desmontado
    return () => {
        // Executa quando o componente é desmontado
        // componentWillUnmount

        console.log('Desmontou')
    }
}, [])

```

#### Podemos usar o useEffect para fazer mais de uma coisa

```javascript

useEffect(() => {
    // Executa uma vez
    // Ideal para fazer requisições
    // componentDidMount

    console.log('Montou')

    return () => {
        // Executa quando o componente é desmontado
        // componentWillUnmount

        console.log('Desmontou')
    }
}, [variavelDeEstado]) // Array de dependências que dispara o useEffect toda vez que a variável de estado mudar

```

## Hooks

#### useState

```javascript

// Declara e seta o e valor da variável de estado
const [state, setState] = useState('')

```

#### useEffect

```javascript

// Executa uma função toda vez que o componente atualiza
useEffect(() => {
    console.log('Atualizou')
}, [variavelDeEstado]) // Array de dependências que dispara o useEffect toda vez que a variável de estado mudar

```

#### useContext

```javascript

// Cria um contexto
const Context = createContext()

// Usa o contexto
const context = useContext(Context)

```

#### useNavigate

```javascript

// Navega entre as rotas
const navigation = useNavigate()

navigation.navigate('/rota')

```

#### useForm

```javascript

// Cria um formulário
const form = useForm()

form.handleChange('nome', 'valor')

```






