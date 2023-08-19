# Operadores Aritméticos y la librería Math

## Operadores Aritméticos

Los operadores aritméticos son los siguientes:

|   Operación   | Símbolo |
| :-------------: | :------: |
|      Suma      |    +    |
|      Resta      |    -    |
| Multiplicación |    *    |
|    División    |    /    |
|     Módulo     |    %    |
|    Incremento     |    ++    |
|    Decremento     |    --    |


## Ejemplos

```javascript
    let a = 1;
    let b = 2;

    let c = a + b; // 3
    let d = a - b; // -1
    let e = a * b; // 2
    let f = a / b; // 0.5
    let g = a % b; // 1
    let h = a++; // 2
    let i = b--; // 1
```

## Operadores de asignación

Los operadores de asignación son los siguientes:

|   Operación   | Símbolo |
| :-------------: | :------: |
|      Asignación      |    =    |
|      Suma y asignación      |    +=    |
| Resta y asignación |    -=    |
|    Multiplicación y asignación    |    *=    |
|     División y asignación     |    /=    |
|    Módulo y asignación     |    %=    |
|    Incremento y asignación     |    ++    |
|    Decremento y asignación     |    --    |

## Ejemplos

```javascript
    let a = 1;
    let b = 2;

    a += b; // 3
    a -= b; // -1
    a *= b; // 2
    a /= b; // 0.5
    a %= b; // 1
    a++; // 2
    b--; // 1
```

## Operadores de concatenación

La concatenación es la unión de dos o más cadenas de texto. Además, podemos concatenar cadenas de texto con números. Los operadores de concatenación son los siguientes:

|   Operación   | Símbolo |
| :-------------: | :------: |
|      Concatenación      |    +    |
|      Concatenación y asignación      |    +=    |

## Ejemplos

```javascript
    let a = "Hola";
    let b = "Mundo";

    let c = a + b; // HolaMundo
    let d = a += b; // HolaMundo
```

## typeof y isNaN

El operador typeof nos permite saber el tipo de dato de una variable. Los tipos de datos que nos devuelve son los siguientes:

|   Tipo de dato   | Resultado |
| :-------------: | :------: |
|      Number      |    number    |
|      String      |    string    |
| Boolean |    boolean    |
|    Function    |    function    |
|     Object     |    object    |
|    Array     |    object    |
|    Undefined     |    undefined    |
|    Null     |    object    |

El método isNaN nos permite saber si un valor es NaN (Not a Number). Este método devuelve true si el valor es NaN, y false si no lo es.

## Ejemplos

```javascript
    let a = 1;
    let b = "Hola";
    let c = true;
    let d = function() {};
    let e = {};
    let f = [];
    let g = undefined;
    let h = null;

    typeof a; // number
    typeof b; // string
    typeof c; // boolean
    typeof d; // function
    typeof e; // object
    typeof f; // object
    typeof g; // undefined
    typeof h; // object

    isNaN(a); // false
    isNaN(b); // true
    isNaN(c); // false
    isNaN(d); // true
    isNaN(e); // true
    isNaN(f); // true
    isNaN(g); // true
    isNaN(h); // true
```

## La librería Math

La librería Math nos permite realizar operaciones matemáticas más complejas. Algunos de los métodos que nos ofrece son:

|   Método   | Descripción |
| :-------------: | :------: |
|      Math.abs()      |    Devuelve el valor absoluto de un número.    |
|      Math.ceil()      |    Devuelve el entero más grande mayor o igual que un número.    |
| Math.floor() |    Devuelve el entero más pequeño menor o igual que un número.    |
|    Math.pow()    |    Devuelve la potencia de un número.    |
|     Math.sqrt()     |    Devuelve la raíz cuadrada de un número.    |
|     Math.random()     |    Devuelve un número aleatorio entre 0 y 1.    |


## Ejemplos

```javascript
    let a = Math.abs(-1); // 1
    let b = Math.ceil(1.5); // 2
    let c = Math.floor(1.5); // 1
    let d = Math.pow(2, 3); // 8
    let e = Math.sqrt(4); // 2
    let f = Math.random(); // 0.123456789
```
