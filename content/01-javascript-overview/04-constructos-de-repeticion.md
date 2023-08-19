# Constructos de Repetición

En todos los lenguajes de programación existen los constructos de repetición. Estos nos permiten repetir un bloque de código varias veces.

La importancia de los constructos de repetición es que nos permiten repetir un bloque de código un número determinado de veces, o mientras una condición sea Verdadera. Esto nos permite reducir la cantidad de código que escribimos.

## for

El for es el constructor de repetición más básico. Se usa para repetir un bloque de código un número determinado de veces.

Sintaxis:

for (inicialización; condición; actualización) {
    // Bloque de código
}

```javascript
    for (let i = 0; i < 10; i++) {
        console.log(i);
    }
```

## while

El while es un constructor de repetición que se usa para repetir un bloque de código mientras la condición sea Verdadera.

Sintaxis:

while (condición) {
    // Bloque de código
}

```javascript
    let i = 0;

    while (i < 10) {
        console.log(i);
        i++;
    }
```

## do...while

El do...while es un constructor de repetición que se usa para repetir un bloque de código mientras la condición sea Verdadera. La diferencia con el while es que el bloque de código se ejecuta al menos una vez.

Sintaxis:

do {
    // Bloque de código
} while (condición);

```javascript
    let i = 0;

    do {
        console.log(i);
        i++;
    } while (i < 10);
```

## break

El break es una palabra clave que se usa para detener la ejecución de un bucle.

Sintaxis:

break;

```javascript
    for (let i = 0; i < 10; i++) {
        if (i === 5) {
            break;
        }

        console.log(i);
    }
```

## continue

El continue es una palabra clave que se usa para saltar una iteración de un bucle.

Sintaxis:

continue;

```javascript
    for (let i = 0; i < 10; i++) {
        if (i === 5) {
            continue;
        }

        console.log(i);
    }
```