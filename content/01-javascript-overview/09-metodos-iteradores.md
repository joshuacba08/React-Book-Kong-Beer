# Métodos iteradores de los arrays

Los métodos iteradores de los arrays son métodos que nos permiten recorrer los elementos de un array. Estos métodos reciben por parámetro una función callback que se ejecuta por cada elemento del array.

Puedes conocer más sobre los métodos iteradores de los arrays en el siguiente enlace: [Métodos iteradores de los arrays](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Global_Objects/Array/prototype)

Probablemente hayas aprendido a recorrer un array usando un ciclo for. Sin embargo, los métodos iteradores de los arrays son más fáciles de usar y más potentes que los ciclos for.

Vamos a ver los métodos iteradores de los arrays más importantes.

## forEach

El método forEach nos permite recorrer los elementos de un array. Este método recibe por parámetro una función callback que se ejecuta por cada elemento del array.

La función callback recibe por parámetro cada elemento del array. Además, recibe por parámetro el índice del elemento y el array completo.

### Sintaxis

```javascript
    array.forEach((elemento, indice, array) =>{
        // Código a ejecutar por cada elemento
    });
```

### Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];

    numeros.forEach((numero)=> {
        console.log(numero);
    });
```

*output:*

```javascript
    1
    2
    3
    4
    5
```

### Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];

    numeros.forEach((numero, indice)=> {
        console.log(indice + ": " + numero);
    });
```

*output:*

```javascript
    0: 1
    1: 2
    2: 3
    3: 4
    4: 5
```

## find

El método find nos permite encontrar un elemento en un array. Este método recibe por parámetro una función callback que se ejecuta por cada elemento del array.

La función callback recibe por parámetro cada elemento del array. Además, recibe por parámetro el índice del elemento y el array completo.

La función callback debe retornar un valor booleano. Si la función retorna true, significa que se encontró el elemento. Si la función retorna false, significa que no se encontró el elemento.

El método find retorna el elemento encontrado. Si no se encuentra el elemento, retorna undefined.

### Sintaxis

```javascript
    array.find((elemento, indice, array)=> {
        // Código a ejecutar por cada elemento
    });
```

### Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];

    let numero = numeros.find((numero) =>{
        return numero === 3;
    });

    console.log(numero); // 3
```

### Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];

    let numero = numeros.find((numero) =>{
        return numero === 6;
    });

    console.log(numero); // undefined
```

## findIndex

El método findIndex nos permite encontrar el índice de un elemento en un array. Este método recibe por parámetro una función callback que se ejecuta por cada elemento del array.

La función callback recibe por parámetro cada elemento del array. Además, recibe por parámetro el índice del elemento y el array completo.

La función callback debe retornar un valor booleano. Si la función retorna true, significa que se encontró el elemento. Si la función retorna false, significa que no se encontró el elemento.

El método findIndex retorna el índice del elemento encontrado. Si no se encuentra el elemento, retorna -1.

### Sintaxis

```javascript
    array.findIndex((elemento, indice, array)=> {
        // Código a ejecutar por cada elemento
    });
```

### Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];

    let indice = numeros.findIndex((numero) =>{
        return numero === 3;
    });

    console.log(indice); // 2
```

### Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];

    let indice = numeros.findIndex((numero) =>{
        return numero === 6;
    });

    console.log(indice); // -1
```

## filter

El método filter nos permite filtrar los elementos de un array. Este método recibe por parámetro una función callback que se ejecuta por cada elemento del array.

La función callback recibe por parámetro cada elemento del array. Además, recibe por parámetro el índice del elemento y el array completo.

La función callback debe retornar un valor booleano. Si la función retorna true, significa que el elemento se debe incluir en el nuevo array. Si la función retorna false, significa que el elemento no se debe incluir en el nuevo array.

El método filter retorna un nuevo array con los elementos filtrados.

### Sintaxis

```javascript
    array.filter((elemento, indice, array) =>{
        // Código a ejecutar por cada elemento
    });
```
- elemento: El elemento actual del array.
- indice: El índice del elemento actual del array.
- array: El array original.

### Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];

    let numerosFiltrados = numeros.filter((numero) =>{
        return numero > 3;
    });

    console.log(numerosFiltrados); // [4, 5]
```

En el ejemplo anterior, se filtran los números mayores que 3. El resultado es un nuevo array con los números filtrados.


## map

El método map nos permite transformar los elementos de un array. Este método recibe por parámetro una función callback que se ejecuta por cada elemento del array.

La función callback recibe por parámetro cada elemento del array. Además, recibe por parámetro el índice del elemento y el array completo.

La función callback debe retornar el elemento transformado.

El método map retorna un nuevo array con los elementos transformados.

### Sintaxis

```javascript
    array.map((elemento, indice, array) =>{
        // Código a ejecutar por cada elemento
    });
```

### Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];

    let numerosTransformados = numeros.map((numero) =>{
        return numero * 2;
    });

    console.log(numerosTransformados); // [2, 4, 6, 8, 10]
```

En el ejemplo anterior, se multiplican por 2 todos los números del array. El resultado es un nuevo array con los números transformados.

Usar un map es una buena práctica cuando queremos transformar los elementos de un array o cuando queremos una copia del array original.

## reduce

El método reduce nos permite reducir los elementos de un array a un único valor. Este método recibe por parámetro una función callback que se ejecuta por cada elemento del array.

La función callback recibe por parámetro un acumulador y cada elemento del array. Además, recibe por parámetro el índice del elemento y el array completo.

La función callback debe retornar el valor del acumulador. Este valor se pasa como acumulador en la siguiente iteración.

El método reduce retorna el valor del acumulador.

### Sintaxis

```javascript
    array.reduce((acumulador, elemento, indice, array) =>{
        // Código a ejecutar por cada elemento
    });
```

### Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];

    let suma = numeros.reduce((acumulador, numero) =>{
        return acumulador + numero;
    }, 0);

    console.log(suma); // 15
```

En el ejemplo anterior, se suman todos los números del array. El resultado es un número que es la suma de todos los números del array.


## some

El método some nos permite saber si algún elemento de un array cumple con una condición. Este método recibe por parámetro una función callback que se ejecuta por cada elemento del array.

La función callback recibe por parámetro cada elemento del array. Además, recibe por parámetro el índice del elemento y el array completo.

La función callback debe retornar un valor booleano. Si la función retorna true, significa que algún elemento cumple con la condición. Si la función retorna false, significa que ningún elemento cumple con la condición.

El método some retorna un valor booleano. Si algún elemento cumple con la condición, retorna true. Si ningún elemento cumple con la condición, retorna false.

### Sintaxis

```javascript
    array.some((elemento, indice, array) =>{
        // Código a ejecutar por cada elemento
    });
```

### Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];

    let resultado = numeros.some((numero) =>{
        return numero > 3;
    });

    console.log(resultado); // true
```

En el ejemplo anterior, se verifica si algún número del array es mayor que 3. El resultado es true porque el número 4 es mayor que 3.

## includes

El método includes nos permite saber si un elemento se encuentra en un array. Este método recibe por parámetro el elemento que queremos buscar.

El método includes retorna un valor booleano. Si el elemento se encuentra en el array, retorna true. Si el elemento no se encuentra en el array, retorna false.

### Sintaxis

```javascript
    array.includes(elemento);
```

### Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];

    let resultado = numeros.includes(3);

    console.log(resultado); // true
```

En el ejemplo anterior, se verifica si el número 3 se encuentra en el array. El resultado es true porque el número 3 se encuentra en el array.

## Sort

El método sort nos permite ordenar los elementos de un array. Este método recibe por parámetro una función callback que se ejecuta por cada elemento del array.

La función callback recibe por parámetro cada elemento del array. Además, recibe por parámetro el índice del elemento y el array completo.

La función callback debe retornar un valor numérico. Si el valor es negativo, significa que el primer elemento es menor que el segundo. Si el valor es positivo, significa que el primer elemento es mayor que el segundo. Si el valor es cero, significa que el primer elemento es igual que el segundo.

El método sort retorna un nuevo array con los elementos ordenados.

### Sintaxis

```javascript
    array.sort((elemento1, elemento2) =>{
        // Código a ejecutar por cada elemento
    });
```

### Ejemplo

```javascript
    let numeros = [5, 3, 4, 2, 1];

    let numerosOrdenados = numeros.sort((a, b) =>{
        return a - b;
    });

    console.log(numerosOrdenados); // [1, 2, 3, 4, 5]
```

En el ejemplo anterior, se ordenan los números del array de menor a mayor. El resultado es un nuevo array con los números ordenados.

## reverse

El método reverse nos permite invertir los elementos de un array. Este método no recibe parámetros.

El método reverse retorna un nuevo array con los elementos invertidos.

### Sintaxis

```javascript
    array.reverse();
```

### Ejemplo

```javascript
    let numeros = [1, 2, 3, 4, 5];

    let numerosInvertidos = numeros.reverse();

    console.log(numerosInvertidos); // [5, 4, 3, 2, 1]
```

En el ejemplo anterior, se invierten los números del array. El resultado es un nuevo array con los números invertidos.







