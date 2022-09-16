### Install and configure tailwindcss in the project
```bash
# Install tailwind and others dependecies
$ npm install -D tailwindcss postcss autoprefixer

# Init tailwind in the project
$ npx tailwindcss init -p
```

Procure pelo arquiv **tailwind.config.cjs** e vamos fazer uns ajustes nele,
deixe-o como mostra o exemplo abaixo:
```js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ['./src/**/*.tsx'],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

Agora crie dentro do seu projeto uma pasta chamada `styles` e dentro um arquivo 
chamado `main.css`, dentro do `main.css` de ver esse conteudo:
```js
@tailwind base;
@tailwind components;
@tailwind utilities;
```

Para finalizar faca a importacao dos styles no seu `App.tsx` como no exemplo abaio:
```js
import './styles/main.css';

function App() {
  return <h1>Hello World!</h1>
}

export default App
```