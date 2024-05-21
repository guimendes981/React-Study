## Hooks

Hooks são funções que permitem adicionar funcionalidades ao componente funcional, como estado, ciclo de vida e contexto.

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






