# Componentes, props y estados

Si pudiésemos resumir React en 3 palabras, estas serían: **componentes**, **props** y **estados**. En este capítulo veremos qué son y cómo funcionan.

![1702292263570](image/01-introducción-a-la-sección/1702292263570.png)

Components, props y states son los tres conceptos clave en React. Virtualmente todo lo que vas a ver o hacer en React se puede clasificar en al menos uno de estos conceptos clave

## Objetivos de esta sección

- Entender qué son los componentes y cómo funcionan.
- Aprender a crear componentes en React.
- Aprender a usar props en React.
- Entender cómo se comunican los componentes entre sí.
- Aprender a usar estados en React.
- Entender qué papel juegan los estados en los componentes.

## Continuación del proyecto Kong Beer

En este capítulo también retomaremos el proyecto Kong Beer que comenzamos en el capítulo anterior. Si no lo has hecho, te recomiendo que lo hagas antes de continuar.

Por el momento solo tenemos la estructura que nos generó Vite, pero en este capítulo comenzaremos a trabajar en el proyecto.

### Limpieza del proyecto

Antes de empezar a trabajar en el proyecto, vamos a hacer una pequeña limpieza. Para ello, vamos a borrar lo siguiente:

#### Logo de Vite `public/vite.svg`

Este archivo no lo vamos a necesitar, por lo tanto, podemos borrarlo. Sin embargo, si lo hacemos, debemos borrar también la referencia a este archivo en `index.html`:

```html
<link rel="icon" href="/vite.svg" />
```

#### Logo de Rect `src/assets/react.svg`

Al eliminar este ar

#### Estilos de Vite `src/index.css`

Si bien mantendremos el archivo `index.css`, vamos a borrar todo su contenido. Esto se debe a que vamos a definir nuestros propios estilos globales en este archivo.

#### Contenido de `src/App.jsx`

Vamos a borrar todo el contenido de `src/App.jsx` y vamos a dejarlo así:

```jsx
import './App.css'

function App() {

  return (
    <div>

    </div>
  )
}

export default App
```

#### Estilos del componente App `src/App.css`

También vamos a borrar todo el contenido de `src/App.css`.


#### Contenido de `README.md`

Vamos a editar el contenido del README.md con el fín de que sea un documento que describa nuestro proyecto. Para ello, vamos a borrar todo el contenido y vamos a dejarlo así:

```md
# Kong Beer

Kong Beer es un e-commerce de cervezas ficticias. Este proyecto fue creado con el fín de aprender React.
```

Ahora sí, ya tenemos nuestro proyecto limpio y listo para empezar a trabajar. En la siguiente sección empezaremos a trabajar en la interfaz de usuario de la aplicación creando nuestros primeros componentes.



