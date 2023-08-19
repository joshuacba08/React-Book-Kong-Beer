# Laboratorio: Día y noche

## Objetivo

- Aplicar los conocimientos adquiridos sobre el DOM y eventos para crear una aplicación que cambie de tema.
- Utilizar el método `addEventListener` para escuchar eventos en el DOM.
- Utilizar el método `querySelector` para seleccionar elementos del DOM.
- Utilizar los constructos `if` y `else` para crear lógica condicional.

## Desarrollo

En este reto vamos a crear una aplicación que cambie de tema entre día y noche. Para esto, vamos a utilizar el método `addEventListener` para escuchar el evento `click` en un botón. Cuando el usuario haga click en el botón, vamos a cambiar el color de fondo de la página y el color del texto, además nuestro título debe cambiar de "Day" a "Night" y viceversa.

La estructura de nuestro directorio de trabajo debe ser la siguiente:

```bash
.
├── index.html
├── script.js
└── style.css
```

Para este reto, vamos a utilizar el siguiente código HTML y CSS:

###### index.html

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width" />
    <title>Javascript Overview</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>

  <body>
    <div class="container" id="fondo">
      <h1 id="title">Day</h1>
    </div>

    <script src="script.js"></script>
  </body>
</html>
```

###### style.css

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: 0;
}

.container {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100vw;
  height: 100vh;
  background-color: #f6f4eb;
  transition: all 500ms ease-in-out;
}
```

Ahora que tenemos nuestro HTML y CSS listos, vamos a crear la lógica de nuestro programa en el archivo `script.js`.

Como recomendación, podemos dividir nuestra logica en 3 o 4 partes:

1. Declarar las variables que vamos a utilizar para seleccionar los elementos del DOM.
2. Definir las funciones que vamos a utilizar para cambiar el tema.
3. Implementar los eventos que van a escuchar los clicks en los botones.
4. Dejar la última parte de nuestro código para las ejecuciones inmediatas.

###### script.js

```js
// 1. Declarar las variables que vamos a utilizar para seleccionar los elementos del DOM.
const fondo = document.getElementById("fondo");
const title = document.getElementById("title");

// 2. Definir las funciones que vamos a utilizar para cambiar el tema.

const changeTime = () => {
  if (title.textContent === "Day") {
    fondo.style.backgroundColor = "#000000";
    title.style.color = "#ffffff";
    title.innerText = "Night";
  } else if (title.textContent === "Night") {
    fondo.style.backgroundColor = "#F6F4EB";
    title.style.color = "#000000";
    title.innerText = "Day";
  }
};

// 3. Implementar los eventos que van a escuchar los clicks en los botones.
fondo.addEventListener("click", changeTime);

// 4. Dejar la última parte de nuestro código para las ejecuciones inmediatas.

// En este caso no tenemos ejecuciones inmediatas, pero vale la pena mencionar que este es el lugar donde se deben colocar.
```

### Función changeTime a detalle

```js
const changeTime = () => {
  if (title.textContent === "Day") {
    fondo.style.backgroundColor = "#000000";
    title.style.color = "#ffffff";
    title.innerText = "Night";
  } else if (title.textContent === "Night") {
    fondo.style.backgroundColor = "#F6F4EB";
    title.style.color = "#000000";
    title.innerText = "Day";
  }
};
```

Vamos a analizar el core de nuestra función `changeTime`:

- Primero, vamos a utilizar un condicional `if` para verificar si el texto del elemento `title` es igual a `Day`.
- De ser así, vamos a manipular los estilos del elemento capturado en la variable `fondo` y del elemento capturado en la variable `title`.
- Por último, vamos a cambiar el texto del elemento `title` a `Night`.
- Si el texto del elemento `title` no es igual a `Day`, vamos a utilizar un condicional `else if` para verificar si el texto del elemento `title` es igual a `Night`.
- De ser así, vamos a manipular los estilos del elemento capturado en la variable `fondo` y del elemento capturado en la variable `title`.
- Por último, vamos a cambiar el texto del elemento `title` a `Day`.
- Si ninguna de las condiciones anteriores se cumple, no vamos a hacer nada.

### Métodos del DOM utilizados en este reto

- `document.getElementById()` : Este método nos permite seleccionar un elemento del DOM a través de su atributo `id`.
- `document.addEventListener()` : Este método nos permite escuchar eventos en el DOM.
- `element.addEventListener()` : Este método nos permite escuchar eventos en un elemento del DOM.
- `element.style` : Este método nos permite manipular los estilos de un elemento del DOM.
- `element.textContent` : Este método nos permite obtener el texto de un elemento del DOM.
- `element.innerText` : Este método nos permite obtener el texto de un elemento del DOM y además nos permite modificarlo.

### Eventos del DOM utilizados en este reto

- `click` : Este evento se dispara cuando el usuario hace click en un elemento del DOM. En este caso, el evento se escucha en toda la pantalla ya el elemento `fondo` ocupa toda la pantalla.

```html
<div class="container" id="fondo">
  <h1 id="title">Day</h1>
</div>
```

Ya que esta es una sección de repaso, no ondaremos en los detalles de los eventos, pero si quieres saber más sobre ellos, puedes consultar la [documentación de MDN](https://developer.mozilla.org/es/docs/Web/Events).

### Código completo en el siguiente link:

[Javascript-overview](https://replit.com/@joshuacba08/Javascript-overview-Ibec?v=1#script.js)

## Conclusiones

En este reto, aprendimos a utilizar los métodos `addEventListener` y `querySelector` para escuchar eventos en el DOM y seleccionar elementos del DOM respectivamente. Además, aprendimos a utilizar los constructos `if` y `else` para crear lógica condicional.

## Reto extra

- Modifica el código para que el tema cambie entre día, tarde y noche 😉 Para esto, puedes utilizar el método `Date.getHours()` para obtener la hora actual del sistema y crear una lógica condicional que cambie el tema dependiendo de la hora del día. 
