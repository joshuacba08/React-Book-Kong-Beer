# Objetos

Un objeto es una estructura de datos que nos permite almacenar varios valores en una misma variable. Estos valores pueden ser de cualquier tipo de dato, incluso otros objetos.

Los objetos son la estructura más compleja que existe. De hecho, los objetos son la base de todas las estructuras de datos que existen. Por ejemplo, las listas enlazadas, las pilas, las colas, los árboles, los grafos, etc. son estructuras de datos que se basan en los objetos.

Es debido a su complejidad que no podemos encontrarlos presentes en todos los lenguajes de programación.

En este capítulo veremos los objetos en JavaScript aplicando los conceptos que hemos aprendido hasta ahora. Una forma muy sencilla de crear objetos en JavaScript es usando la notación literal de objetos.

### Sintaxis

```javascript
    let objeto = {};
```

Los objetos se declaran usando llaves. Dentro de las llaves se colocan los valores que queremos almacenar en el objeto. Estos valores se separan por comas.

### Ejemplo

```javascript
    let persona = {
        nombre: "Juan",
        edad: 29,
        pais: "Colombia",
        hijos: ["Pedro", "María"],
        mascota: {
            nombre: "Firulais",
            edad: 5
        }
    };
```

Los objetos describen una relación entre propiedades y valores. Cada propiedad tiene un nombre y un valor. Por ejemplo, en el objeto anterior, la propiedad nombre tiene el valor "Juan", la propiedad edad tiene el valor 20, la propiedad pais tiene el valor "Colombia", etc.

## Acceder a una propiedad de un objeto

Para acceder a una propiedad de un objeto, se usa el nombre del objeto seguido de un punto y el nombre de la propiedad.

### Ejemplo

```javascript
    let persona = {
        nombre: "Juan",
        edad: 29,
        pais: "Colombia",
        hijos: ["Pedro", "María"],
        mascota: {
            nombre: "Firulais",
            edad: 5
        }
    };

    console.log(persona.nombre); // Juan
    console.log(persona.edad); // 29
    console.log(persona.pais); // Colombia
    console.log(persona.hijos); // ["Pedro", "María"]
    console.log(persona.mascota); // { nombre: "Firulais", edad: 5 }
```

## Actualizar una propiedad de un objeto

Para actualizar una propiedad de un objeto, se usa el nombre del objeto seguido de un punto, el nombre de la propiedad y se asigna el nuevo valor.

### Ejemplo

```javascript
    let persona = {
        nombre: "Juan",
        edad: 29,
        pais: "Colombia",
        hijos: ["Pedro", "María"],
        mascota: {
            nombre: "Firulais",
            edad: 5
        }
    };

    persona.nombre = "Pedro";
    persona.edad = 30;
    persona.pais = "España";
    persona.hijos = ["Diana"];
    persona.mascota = {
        nombre: "Firulais",
        edad: 6
    };
```

## Agregar una propiedad a un objeto

Para agregar una propiedad a un objeto, se usa el nombre del objeto seguido de un punto, el nombre de la nueva propiedad y se asigna el valor de la nueva propiedad.

### Ejemplo

```javascript
    let persona = {
        nombre: "Juan",
        edad: 29,
        pais: "Colombia",
        hijos: ["Pedro", "María"],
        mascota: {
            nombre: "Firulais",
            edad: 5
        }
    };

    persona.apellido = "Perez";
    persona.profesion = "Ingeniero";
    persona.hijos.push("Diana");
    persona.mascota.raza = "Labrador";
```
Si aplicamos un console.log a la variable persona, veremos que se ha agregado una nueva propiedad a la variable persona. El output en la consola será el siguiente para un `console.log(persona)`:

```javascript
    {
        nombre: "Juan",
        edad: 29,
        pais: "Colombia",
        hijos: ["Pedro", "María", "Diana"],
        mascota: {
            nombre: "Firulais",
            edad: 5,
            raza: "Labrador"
        },
        apellido: "Perez",
        profesion: "Ingeniero"
    }
```

## Eliminar una propiedad de un objeto

Para eliminar una propiedad de un objeto, se usa la palabra clave delete seguida del nombre del objeto y el nombre de la propiedad.

### Ejemplo

```javascript
    let persona = {
        nombre: "Juan",
        edad: 29,
        pais: "Colombia",
        hijos: ["Pedro", "María"],
        mascota: {
            nombre: "Firulais",
            edad: 5
        }
    };

    delete persona.nombre;
    delete persona.edad;
    delete persona.pais;
    delete persona.hijos;
    delete persona.mascota;
```

Si aplicamos un console.log a la variable persona, veremos que se ha eliminado una propiedad de la variable persona. El output en la consola será el siguiente para un `console.log(persona)`:

```javascript
    {}
```
Habremos vaciado el objeto por completo.





