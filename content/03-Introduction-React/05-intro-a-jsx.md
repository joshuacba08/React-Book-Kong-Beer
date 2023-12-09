# Introducción a JSX

## Objetivos de esta sección

- Entender qué es JSX y qué ventajas nos ofrece.
- Aprender a usar JSX en nuestros proyectos.

## Introducción a JSX

Bienvenido a JSX, una extensión de sintaxis para JavaScript. Muchos concuerdan que JSX es una de las grandes genialidades de React, sin embargo también es uno de los temás más controversiales relacionados con React.

El equipo de Facebook lanzo JSX en 2013 como parte de React para proveer una sintaxis concisa y familiar para crear árboles complejos de DOM con atributos. Desde entonces, JSX se ha convertido en la forma más popular de escribir componentes de React. Además, es mucho más fácil de leer ya que es parecido a HTML y XML.

### ¿Qué es JSX?

A grandes rasgos JSX es una combinación de JavaScript (JS) y XML (X). Es una forma elegante de escribir código JavaScript junto a una sintaxis similar a HTML.

### Sintaxis

La sintaxis de JSX es muy similar a la de HTML. Veamos a continuación un ejemplo de JSX:

```jsx
const element = <h1>Hello, world!</h1>;
```

Como se puede ver, podemos escribir una suerte de HTML dentro de JavaScript usando JSX y nuestro editor de código nos ayudará a identificar los errores de sintaxis.

### Consideraciones

Veremos algunas consideraciones que nos ayudarán a entender mejor cómo funciona JSX.

#### JSX no es HTML

JSX es una extensión de JavaScript, por lo tanto, lo que veamos que se parezca a HTML dentro del código en realidad es XML.

#### className en lugar de class

En JSX, se usa `className` en lugar de `class` para definir clases CSS, esto se debe a que class es una palabra reservada en JavaScript para crear clases (Recordemos que JavaScript es un lenguaje orientado a objetos).

###### Ejemplo

```jsx
const element = <h1 className="greeting">Hello, world!</h1>;
```

#### Expresiones de JavaScript

Podemos usar expresiones de JavaScript dentro de JSX, para esto debemos encerrarlas entre llaves `{}`.

###### Ejemplo

```jsx
const name = 'Josh Perez';
const element = <h1>Hello, {name}</h1>;
```

Si renderizamos este elemento en el DOM, el contenido de la etiqueta `<h1>` será `Hello, Josh Perez`. Esto se debe a que dentro del XML podemos usar expresiones de JavaScript (una expresion de Javascript es todo aquello que se puede evaluar y que devuelve un valor como variables, operaciones aritméticas, operaciones lógicas, funciones, estructuras de datos, etc.).

**Nota:** JSX no es un requisito para usar React. Es posible escribir código React sin JSX, pero la mayoría de las personas lo encuentran útil como ayuda visual cuando trabajan con interfaces de usuario dentro del código JavaScript. También permite a React mostrar mensajes de error y advertencias más útiles.


## Creando un componente con JSX

Vamos a crear un componente con JSX para aplicar lo recientemente aprendido. Para esto, vamos a separar nuestro componente `Button` en un archivo aparte llamado `Button.jsx`, por el momento no vamos a importar el archivo ni montarlo dentro de un componente, solo vamos a ver cómo se ve JSX.

###### `Button.jsx`

```jsx
const Button = () => {
  return (
    <button className="button">
      Click me!
    </button>
  );
};

export default Button;
```

Cómo se puede apreciar, tendremos una función que retorna un elemento JSX. En este caso, el elemento JSX es un botón con una clase CSS llamada `button` y un texto que dice `Click me!`.




