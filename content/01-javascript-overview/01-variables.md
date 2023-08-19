# Variables

Las variables almacenan datos que se pueden configurar, actualizar y recuperar cuando sea necesario. Los valores que se asignan a una variable pertenecen a un tipo. En JavaScript, los tipos disponibles son número, cadena, booleano, función y objeto. También tenemos undefined y null, junto con matrices, fechas y expresiones regulares.

## Declaración de variables

```javascript
    var a = 1; // Variable global
    let b = 2; // Variable local
    const c = 3; // Constante
```

## Cuando usar var, let o const

- var: Es la forma antigua de declarar variables. No se recomienda su uso.
- let: Es la forma moderna de declarar variables. Se recomienda su uso.
- const: Es la forma moderna de declarar constantes. Se recomienda su uso.

## Que es una variable global

Una variable global es una variable que se puede acceder desde cualquier parte del código. Se recomienda no usar variables globales.

## Que es una variable local

Una variable local es una variable que solo se puede acceder desde el bloque de código donde se declaró.

## Que es una constante

Una constante es una variable que no se puede actualizar. Se recomienda usar constantes en lugar de variables globales.

En JavaScript, las constantes se declaran usando la palabra clave const.

Ejemplo:

```javascript
    const PI = 3.1416;
```

Quizás se pregunte por qué usar constantes en lugar de variables globales. La respuesta es que las constantes son más seguras. Si intenta actualizar una constante, JavaScript arrojará un error.

## Variable let

La palabra clave let se usa para declarar variables locales. Las variables locales solo se pueden acceder desde el bloque de código donde se declararon.

Además, las variables locales declaradas con let pueden actualizarse, pero no pueden redeclararse.

## Tipos de datos

```javascript
    let a = 1; // Number
    let b = "Hola"; // String
    let c = true; // Boolean
    let d = function() {}; // Function
    let e = {}; // Object
    let f = []; // Array
    let g = undefined; // Undefined
    let h = null; // Null
```

## Visualizar el valor de una variable por consola

Si queremos ver el valor de cada variable que declaramos, podemos usar console.log para hacerlo, como se indica en el siguiente fragmento de código:

```javascript
    let a = 1; // Number
    let b = "Hola"; // String
    let c = true; // Boolean
    let d = function() {}; // Function
    let e = {}; // Object
    let f = []; // Array
    let g = undefined; // Undefined
    let h = null; // Null

    console.log(a);
    console.log(b);
    console.log(c);
    console.log(d);
    console.log(e);
    console.log(f);
    console.log(g);
    console.log(h);
```
