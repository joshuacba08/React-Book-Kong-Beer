# Función regular y función flecha

En JavaScript, existen dos formas de declarar funciones: la función regular y la función flecha. Las funciones regulares son la forma antigua de declarar funciones, y las funciones flecha son la forma moderna de declarar funciones. La diferencia entre ambas es que las funciones flecha son más cortas y más fáciles de escribir, sin embargo, las funciones regulares son más flexibles. En este artículo, aprenderemos a declarar funciones regulares y funciones flecha.

## Función regular

La función regular es la forma antigua de declarar funciones. Se declaran usando la palabra clave `function`, seguida del nombre de la función, seguida de paréntesis, seguida de llaves. Dentro de los paréntesis, podemos declarar los parámetros de la función. Dentro de las llaves, podemos declarar el cuerpo de la función.

Sintaxis:

```javascript
function nombre(parametro1, parametro2) {
    // Cuerpo de la función
}
```

Ejemplo:

```javascript
function sumar(a, b) {
    return a + b;
}
```

## Función flecha

La función flecha es la forma moderna de declarar funciones. Se declaran usando una flecha `=>`, seguida de paréntesis, seguida de llaves. Dentro de los paréntesis, podemos declarar los parámetros de la función. Dentro de las llaves, podemos declarar el cuerpo de la función.

Sintaxis:

```javascript
(parametro1, parametro2) => {
    // Cuerpo de la función
}
```

Ejemplo:

```javascript
(a, b) => {
    return a + b;
}
```
Es necesario asignar la función a una variable para poder usarla. Por ejemplo:

```javascript
let sumar = (a, b) => {
    return a + b;
}
```
De esta manera, podemos usar la función sumar en cualquier parte del código. De lo contrario, la función solo se puede usar en el bloque de código donde se declaró ya que su existencia solo es conocida dentro de ese bloque de código.

## Función flecha con un solo parámetro

Si la función flecha tiene un solo parámetro, podemos omitir los paréntesis. Por ejemplo:

```javascript
let cuadrado = x => {
    return x * x;
}
```

## Función flecha con un solo parámetro y un solo retorno

Si la función flecha tiene un solo parámetro y un solo retorno, podemos omitir los paréntesis y las llaves. Por ejemplo:

```javascript
let cuadrado = x => x * x; 
```

## Función flecha sin parámetros

Si la función flecha no tiene parámetros, debemos usar paréntesis vacíos. Por ejemplo:

```javascript
let saludar = () => {
    console.log("Hola");
}
```

## Función flecha sin parámetros y sin llaves

Si la función flecha no tiene parámetros y no tiene llaves, podemos omitir los paréntesis y las llaves. Por ejemplo:

```javascript

let saludar = () => console.log("Hola");
```

## Función flecha con un solo parámetro y sin llaves

Si la función flecha tiene un solo parámetro y no tiene llaves, podemos omitir los paréntesis y las llaves. Por ejemplo:

```javascript

let cuadrado = x => x * x;
```

En resumen, debemos usar la función regular cuando necesitemos flexibilidad, y debemos usar la función flecha cuando necesitemos simplicidad. En la mayoría de los casos, la función flecha es la mejor opción.






