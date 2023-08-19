# Array de objetos

## Introducción

En este documento se explica cómo crear un array de objetos. El objetivo es que el estudiante aprenda a crear un array de objetos usando lo visto hasta ahora sobre objetos. Para ello, se explica cómo crear un array de objetos usando un ejemplo.

Los arrays de objetos son muy utilizados en el desarrollo de software. Por ejemplo, en una aplicación web de una tienda online, se puede usar un array de objetos para almacenar los productos de la tienda. 

## Ejemplo práctico

Supongamos que es nuestro primer día de trabajo en una empresa de desarrollo de software. Nuestro jefe nos pide que desarrollemos un sistema para administrar los productos de la empresa. Para ello, nos pide que creemos un array de objetos que almacene los productos de la empresa.

Previamente hemos modelado la entidad Producto a través de un objeto. Ahora, debemos crear un array de objetos que almacene los productos de la empresa. A continuación se muestra un ejemplo de cómo crear un array de objetos:

```javascript
    let productos = [
        {
            nombre: "Televisor",
            precio: 1000,
            descripcion: "Televisor Samsung 50 pulgadas"
        },
        {
            nombre: "Celular",
            precio: 500,
            descripcion: "Celular Samsung Galaxy S10"
        },
        {
            nombre: "Laptop",
            precio: 1500,
            descripcion: "Laptop Lenovo Thinkpad T480"
        }
    ];
```

Perfecto, hemos creado un array de objetos. Un ejercicio muy práctico sería intentar crear un array de objetos que represente a una persona, a un auto, a una mascota, etc.


## Aplicaciones prácticas

ES muy probable que si tenemos un array de objetos, queramos mostrar los objetos en una página web. Para ello, podemos usar el método `forEach` de los arreglos. Este método recibe por parámetro una función callback que se ejecuta por cada elemento del arreglo. A continuación se muestra un ejemplo de cómo mostrar los productos de la empresa en una página web aunque para este caso solo lo mostraremos por consola:

```javascript
    productos.forEach(producto => {
        console.log(producto.nombre);
        console.log(producto.precio);
        console.log(producto.descripcion);
    });
```

## Conclusiones

- Un array de objetos es un arreglo que almacena objetos.
- Esta estructura de datos combinada es muy utilizada en el desarrollo de software.
- Dominar los métodos de los arreglos es fundamental para trabajar con arrays de objetos.
  

