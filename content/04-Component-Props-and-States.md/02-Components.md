# Componentes

Los componentes son los elementos básicos de cualquier aplicación React. Ellos son como Funciones de JavaScript que aceptan entradas arbitrarias (Props) y devuelven Elementos React que describen lo que debe mostrarse en la pantalla.

Lo primero que hay que entender es que todo lo que aparece en pantalla en una aplicación React es parte de un componente. Esencialmente, una aplicación React son solo componentes dentro de otros componentes.

Los componentes te permiten dividir tu interfaz de usuario en piezas independientes y reutilizables. 

No está por demás citar esta dicho:

> **Los desarrolladores de React no crean páginas, construyen componentes.**

![1702303979649](image/02-Components/1702303979649.png)

En la imagen anterior podemos ver un ejemplo de cómo se vería una aplicación React en su forma más básica. En este caso, tenemos un componente `App` que contiene 3 componentes, <Navbar />, <Home /> y <Footer />. A su vez el componente <Home /> contiene 2 grupos de componentes, un <Banner /> y unos componentes <Card /> representado cards de productos.

