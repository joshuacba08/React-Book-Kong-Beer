# Variales de Scope

En JavaScript, existen dos tipos de variables: las variables globales y las variables locales. Las variables globales se pueden acceder desde cualquier parte del código, mientras que las variables locales solo se pueden acceder desde el bloque de código donde se declararon.

A este tipo de entorno se le conoce como scope. El scope es el alcance que tiene una variable. En JavaScript, existen dos tipos de scope: el scope global y el scope local.

## Scope global

El scope global es el alcance que tienen las variables globales. Las variables globales se pueden acceder desde cualquier parte del código.

## Scope local

El scope local es el alcance que tienen las variables locales. Las variables locales solo se pueden acceder desde el bloque de código donde se declararon.

## Ejemplo

```javascript
    let a = 1; // Variable global

    function sumar() {
        let b = 2; // Variable local
        return a + b;
    }

    console.log(sumar()); // 3
    console.log(a); // 1
    console.log(b); // Error
```
Tal y como se muestra en el ejemplo anterior, la variable `a` es una variable global, por lo que se puede acceder a ella desde cualquier parte del código. Por otro lado, la variable `b` es una variable local, por lo que solo se puede acceder a ella desde el bloque de código donde se declaró.

En JavaScript, las variables globales se declaran usando la palabra clave `var`, mientras que las variables locales se declaran usando la palabra clave `let`.

Cabe destacar que las variables globales se pueden actualizar y redeclarar, mientras que las variables locales solo se pueden actualizar.

Hay que destacar además que las variables globales son más peligrosas que las variables locales, ya que pueden ser actualizadas desde cualquier parte del código, lo cual puede causar errores difíciles de detectar.

Por último vale mencionar a las constantes que son variables que no se pueden actualizar ni redeclarar. Las constantes se declaran usando la palabra clave `const` y estas son a su ves variables locales.

## Ejemplo

```javascript
    var a = 1; // Variable global
    let b = 2; // Variable local
    const c = 3; // Constante
```

## Recomendaciones

Se recomienda usar siempre `let` y `const` en lugar de `var`. Además, se recomienda usar `const` en lugar de `let` siempre que sea posible.

Es decir que si detectamos que una variable no se va a actualizar, debemos declararla como constante. De esta manera, evitamos que la variable sea actualizada por error.

## Ejemplo

```javascript
    const PI = 3.1416;
```

Existen grandes errores que se han cometido a lo largo de la historia en la ciencia. Uno de ellos es el valor de PI. En la antigüedad, se creía que el valor de PI era 3. Esto causó muchos errores en los cálculos de los científicos de la época. Por ejemplo, el valor de PI se usó para calcular el área de un círculo. Sin embargo, el valor de PI era incorrecto, por lo que el área de un círculo también era incorrecta.

## Ejemplo

```javascript
    let radio = 5;
    let area = PI * radio * radio;
    console.log(area); // 75.99
```

En el ejemplo anterior, el valor de PI es incorrecto, por lo que el área de un círculo también es incorrecta. Sin embargo, si usamos el valor correcto de PI, el área de un círculo será correcta.

## Ejemplo

```javascript
    const PI = 3.1416;
    let radio = 5;
    let area = PI * radio * radio;
    console.log(area); // 78.54
```

Imagina que alguien comete el error de querer actualizar el valor de PI. Si la variable PI fuera una variable global, se podría actualizar desde cualquier parte del código, lo cual causaría un error difícil de detectar.

```javascript
    const PI = 3.1416;
    PI = 3.14; // Error
```

Sin embargo, como se declaró la variable PI como constante, no se puede actualizar, lo cual evita que se cometa un error.