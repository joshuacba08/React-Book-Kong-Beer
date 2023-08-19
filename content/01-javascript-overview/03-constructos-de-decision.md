# Constructos de decisión

En todos los lenguajes de programación existen los constructos de decisión. Estos nos permiten tomar decisiones en base a una condición.

Estas condiciones pueden ser Verdaderas o Falsas.

## Truthy y Falsy

En JavaScript, existen valores que son considerados como Verdaderos y otros que son considerados como Falsos.

La siguiente tabla puede ayudarte a entender como funciona esto:

|    Valor    | ¿Es Verdadero? |
| :----------: | :-------------: |
|  undefined  |      Falso      |
|     null     |      Falso      |
|      0      |      Falso      |
|     NaN     |      Falso      |
|      ""      |      Falso      |
|     ' '     |    Verdadero    |
|      1      |    Verdadero    |
|    "Hola"    |    Verdadero    |
|      []      |    Verdadero    |
|      {}      |    Verdadero    |
| function(){} |    Verdadero    |

## Aplicación de los constructos de decisión

Los constructos de decisión se usan para tomar decisiones en base a una condición. Esto permite que el código se ejecute de forma diferente en base a la condición. Es decir, si la condición es Verdadera, se ejecuta un bloque de código, y si la condición es Falsa, se ejecuta otro bloque de código. De esta manera podemos controlar el flujo de nuestro programa.

## if

El if es el constructor de decisión más básico. Se usa para ejecutar un bloque de código si la condición es Verdadera.

### Ejemplo

```javascript
    let a = 1;
    let b = 2;

    if (a < b) {
        console.log("a es menor que b");
    }
```

## if...else

El if...else es un constructor de decisión que se usa para ejecutar un bloque de código si la condición es Verdadera, y otro bloque de código si la condición es Falsa.

### Ejemplo

```javascript
    let a = 1;
    let b = 2;

    if (a < b) {
        console.log("a es menor que b");
    } else {
        console.log("a es mayor que b");
    }
```

## if...else if...else

El if...else if...else es un constructor de decisión que se usa para ejecutar un bloque de código si la condición es Verdadera, otro bloque de código si la condición es Falsa, y otro bloque de código si la condición es Verdadera.

### Ejemplo

```javascript
    let a = 1;
    let b = 2;

    if (a < b) {
        console.log("a es menor que b");
    } else if (a > b) {
        console.log("a es mayor que b");
    } else {
        console.log("a es igual a b");
    }
```

## switch

El switch es un constructor de decisión que se usa para ejecutar un bloque de código si la condición es Verdadera, otro bloque de código si la condición es Falsa, y otro bloque de código si la condición es Verdadera.

### Ejemplo

```javascript
    let a = 1;
    let b = 2;

    switch (a) {
        case 1:
            console.log("a es igual a 1");
            break;
        case 2:
            console.log("a es igual a 2");
            break;
        default:
            console.log("a no es igual a 1 ni a 2");
            break;
    }
```

## Operadores de comparación

Los operadores de comparación se usan para comparar dos valores. Los operadores de comparación son los siguientes:

|       Operación       | Símbolo |
| :--------------------: | :------: |
|         Igual         |    ==    |
|        No igual        |    !=    |
|  Estrictamente igual  |   ===   |
| Estrictamente no igual |   !==   |
|       Mayor que       |    >    |
|   Mayor o igual que   |    >=    |
|       Menor que       |    <    |
|   Menor o igual que   |    <=    |

## Operadores lógicos

Los operadores lógicos se usan para combinar dos o más condiciones. Los operadores lógicos son los siguientes:

| Operación | Símbolo |
| :--------: | :------: |
|     Y     |    &&    |
|     O     |   \|\|   |
| Negación |    !    |

## Operadores ternarios

Los operadores ternarios se usan para asignar un valor a una variable en base a una condición. Los operadores ternarios son los siguientes:

| Operación | Símbolo |
| :--------: | :------: |
|  Ternario  |    ?    |
|  Ternario  |    :    |

### Ejemplo

```javascript
    let a = 1;
    let b = 2;

    let c = a < b ? "a es menor que b" : "a es mayor que b";
```
