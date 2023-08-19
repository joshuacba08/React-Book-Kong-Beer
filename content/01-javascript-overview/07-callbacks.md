# Callbacks

Un callback es una función que se pasa como argumento a otra función. Esta función se ejecuta dentro de la función que la recibe. Los callbacks se usan para ejecutar código de forma asíncrona. Es decir, el código se ejecuta en segundo plano, mientras que el resto del código se ejecuta de forma síncrona.

Además, los callbacks se usan para ejecutar código después de que se haya completado una tarea. Por ejemplo, si queremos ejecutar un código después de que se haya completado una petición a un servidor, podemos usar un callback para hacerlo.

Por último y no menos importante, los callbacks nos ayudan a separar el código en bloques más pequeños, lo cual hace que el código sea más fácil de leer y de mantener. Es decir que los callbacks nos ayudan a escribir código más limpio y organizado ya que nos permiten separar las responsabilidades del código.

## Ejemplo

```javascript
    function saludar(nombre) {
        console.log("Hola " + nombre);
    }

    function procesarEntradaUsuario(callback) {
        let nombre = prompt("Ingresa tu nombre");
        callback(nombre);
    }

    procesarEntradaUsuario(saludar);
```

Como se puede ver en el ejemplo anterior, la función `saludar` se pasa como argumento a la función `procesarEntradaUsuario`. Esta función se ejecuta dentro de la función `procesarEntradaUsuario`. Es decir, la función `saludar` se ejecuta dentro de la función `procesarEntradaUsuario`.


## Separación de responsabilidades

Vamos a ver la separación de responsabilidades mediante el ejemplo de una función Calculadora que recibirá por parámetros dos números y una función callback escritas como funcion flecha.

```javascript
    function calculadora(num1, num2, callback) {
        return callback(num1, num2);
    }

    calculadora(2, 3, (num1, num2) => num1 + num2);
    calculadora(2, 3, (num1, num2) => num1 - num2);
    calculadora(2, 3, (num1, num2) => num1 * num2);
    calculadora(2, 3, (num1, num2) => num1 / num2);
```

En el ejemplo anterior, la función `calculadora` recibe por parámetros dos números y una función callback. Esta función se ejecuta dentro de la función `calculadora`. Es decir, la función callback se ejecuta dentro de la función `calculadora`.

Veremos más callbacks cuando veamos los métodos iteradores de los arreglos. Estos reciben por parámetro una función callback que se ejecuta por cada elemento del arreglo.











