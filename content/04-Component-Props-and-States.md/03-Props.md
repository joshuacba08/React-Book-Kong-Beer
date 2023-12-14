# Props

En la sección anterior creamos un componente `Button` que representaba un botón. Sin embargo, este componente no era muy útil porque siempre mostraba el mismo texto o el mismo color. En esta sección vamos a aprender a hacer que nuestros componentes sean más dinámicos usando props.

## ¿Qué son los Props?

Las “props” son una forma abreviada de propiedades, y simplemente se refieren a los datos internos de un componente en React. Se escriben dentro de llamadas a componentes y se pasan a componentes. 

Las props son argumentos que se pasan a un componente. Son como los argumentos de una función, pero para componentes de React. 

Además las props son la forma de comunicación entre componentes. Si queremos pasar datos de un componente a otro, lo hacemos a través de props desde su componente padre al componente hijo.

## ¿Cómo se ven los Props?

Para ilustrar cómo las props se ven en la práctica, podemos considerar el siguiente componente `Button`:

![1702503121117](image/03-Props/1702503121117.png)

Cómo se puede observar, este componente recibe 4 props:

- **label**: que es el texto que se va a mostrar en el botón.
- **variant**: que es el tipo de botón que se va a mostrar. Puede ser `primary` o `secondary` por ejemplo.
- **onClick**: que es la función que se va a ejecutar cuando se haga click en el botón.
- **Icon**: que es el ícono que se va a mostrar en el botón.

Tal vez te estés preguntando ¿Cómo se pasan las props a un componente? Bueno, las props se pasan como argumentos a los componentes. Por ejemplo, si queremos pasarle la prop `label` al componente `Button`, lo hacemos de la siguiente manera:


