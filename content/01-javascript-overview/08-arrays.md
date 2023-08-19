# Arrays o Arreglos

Un array es una estructura de datos que nos permite almacenar varios valores en una misma variable. Estos valores pueden ser de cualquier tipo de dato, incluso otros arreglos.

Los arrays son la estructura más simple que existe. De hecho, los arrays son la base de todas las estructuras de datos que existen. Por ejemplo, las listas enlazadas, las pilas, las colas, los árboles, los grafos, etc. son estructuras de datos que se basan en los arrays.

Es debido a su simplicidad que podemos encontrarlos presentes en todos los lenguajes de programación.

## Sintaxis

```javascript
    let arreglo = [];
```
Los arrays se declaran usando corchetes. Dentro de los corchetes se colocan los valores que queremos almacenar en el array. Estos valores se separan por comas.

## Index o Índice de un array

Los arrays son estructuras de datos indexadas. Esto quiere decir que cada valor que se almacena en un array tiene un índice asociado. Este índice nos permite acceder al valor que queremos. El índice de un array es un número entero que empieza en cero y termina en la cantidad de elementos del array menos uno.

## Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];
    let nombres = ["Juan", "Pedro", "María", "Diana"];
    let mixto = [1, "Pedro", true, null, undefined, {}];
    let arreglo = [];
```

## Acceder a un elemento de un array

Para acceder a un elemento de un array, se usa el nombre del array seguido del índice del elemento entre corchetes.

## Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];
    let nombres = ["Juan", "Pedro", "María", "Diana"];
    let mixto = [1, "Pedro", true, null, undefined, {}];
    let arreglo = [];

    console.log(numeros[0]); // 1
    console.log(nombres[1]); // Pedro
    console.log(mixto[2]); // true
```

## Actualizar un elemento de un array

Para actualizar un elemento de un array, se usa el nombre del array seguido del índice del elemento entre corchetes, y se asigna el nuevo valor.

## Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];
    let nombres = ["Juan", "Pedro", "María", "Diana"];
    let mixto = [1, "Pedro", true, null, undefined, {}];
    let arreglo = [];

    numeros[0] = 10;
    nombres[1] = "Pedra";
    mixto[2] = false;

    console.log(numeros[0]); // 10
    console.log(nombres[1]); // Pedra
    console.log(mixto[2]); // false
```

## Longitud de un array

La longitud de un array es la cantidad de elementos que tiene. Para obtener la longitud de un array, se usa la propiedad length.

## Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];
    let nombres = ["Juan", "Pedro", "María", "Diana"];
    let mixto = [1, "Pedro", true, null, undefined, {}];
    let arreglo = [];

    console.log(numeros.length); // 5
    console.log(nombres.length); // 4
    console.log(mixto.length); // 6
    console.log(arreglo.length); // 0
```

## Agregar un elemento al final de un array

Para agregar un elemento al final de un array, se usa el método push.

## Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];
    let nombres = ["Juan", "Pedro", "María", "Diana"];
    let mixto = [1, "Pedro", true, null, undefined, {}];
    let arreglo = [];

    numeros.push(6);
    nombres.push("Luis");
    mixto.push(false);
    arreglo.push(1);

    console.log(numeros); // [1, 2, 3, 4, 5, 6]
    console.log(nombres); // ["Juan", "Pedro", "María", "Diana", "Luis"]
    console.log(mixto); // [1, "Pedro", true, null, undefined, {}, false]
    console.log(arreglo); // [1]
```

## Agregar un elemento al inicio de un array

Para agregar un elemento al inicio de un array, se usa el método unshift.

## Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];
    let nombres = ["Juan", "Pedro", "María", "Diana"];
    let mixto = [1, "Pedro", true, null, undefined, {}];
    let arreglo = [];

    numeros.unshift(0);
    nombres.unshift("Luis");
    mixto.unshift(false);
    arreglo.unshift(1);

    console.log(numeros); // [0, 1, 2, 3, 4, 5]
    console.log(nombres); // ["Luis", "Juan", "Pedro", "María", "Diana"]
    console.log(mixto); // [false, 1, "Pedro", true, null, undefined, {}]
    console.log(arreglo); // [1]
```

## Eliminar un elemento al final de un array

Para eliminar un elemento al final de un array, se usa el método pop.

## Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];
    let nombres = ["Juan", "Pedro", "María", "Diana"];
    let mixto = [1, "Pedro", true, null, undefined, {}];
    let arreglo = [1];

    numeros.pop();
    nombres.pop();
    mixto.pop();
    arreglo.pop();

    console.log(numeros); // [1, 2, 3, 4]
    console.log(nombres); // ["Juan", "Pedro", "María"]
    console.log(mixto); // [1, "Pedro", true, null, undefined]
    console.log(arreglo); // []
```

## Eliminar un elemento al inicio de un array

Para eliminar un elemento al inicio de un array, se usa el método shift.

## Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];
    let nombres = ["Juan", "Pedro", "María", "Diana"];
    let mixto = [1, "Pedro", true, null, undefined, {}];
    let arreglo = [1];

    numeros.shift();
    nombres.shift();
    mixto.shift();
    arreglo.shift();

    console.log(numeros); // [2, 3, 4, 5]
    console.log(nombres); // ["Pedro", "María", "Diana"]
    console.log(mixto); // ["Pedro", true, null, undefined, {}]
    console.log(arreglo); // []
```

## Eliminar un elemento de un array

Para eliminar un elemento de un array, se usa el método splice.

## Sintaxis

```javascript
    arreglo.splice(indice, cantidad);
```
- indice: Índice del elemento que queremos eliminar.
- cantidad: Cantidad de elementos que queremos eliminar.

## Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];
    let nombres = ["Juan", "Pedro", "María", "Diana"];
    let mixto = [1, "Pedro", true, null, undefined, {}];

    numeros.splice(0, 1);
    nombres.splice(1, 2);
    mixto.splice(2, 3);

    console.log(numeros); // [2, 3, 4, 5]
    console.log(nombres); // ["Juan", "Diana"]
    console.log(mixto); // [1, "Pedro", {}]
```





