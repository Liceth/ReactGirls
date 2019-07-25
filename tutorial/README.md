---
description: >-
  Hay muy pocas maneras de configurar React, por ello les mostrare dos opciones
  para tener una idea de como funciona.
---

# Instalación & Configuración

## **Archivo estático HTML**

Este primer método no es una forma muy común para configurar React y no sera como estaremos trabajando el resto de nuestro taller, pero sera muy fácil de entender y familiar si alguna vez haz usado librerías como jQuery, y es la forma menos aterradora de comenzar si no se esta familiarizado con Webpack, Babel y Node.js. 

Empezaremos creando un archivo básico que le colocaremos el nombre  `index.html` , Vamos a cargar dentro de la etiqueta head estos tres CDN  `React, React DOM y babel` 

 Luego crearemos un `div`  con **id**  llamado `root`   y finalmente crearemos un `script` tag donde nuestro código personalizado cobrara vida. 

{% code-tabs %}
{% code-tabs-item title="index.html" %}
```text
!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />

    <title>Hello React!</title>

    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6.26.0/babel.js"></script>
  </head>

  <body>
    <div id="root"></div>

    <script type="text/babel">
      // React code will go here
    </script>
  </body>
</html>

```
{% endcode-tabs-item %}
{% endcode-tabs %}

Este paso lo que hace es cargar al archivo HTML las ultimas versiones estables de las librerías hasta este momento.

* [**React** ](https://reactjs.org/docs/react-api.html)\*\*\*\*
  * Proporciona una detallada documentación de la  **API** para componentes en React
* [**ReactDOM** ](https://reactjs.org/docs/react-dom.html)\*\*\*\*
  * Proporciona métodos específicos de DOM que se pueden utilizar en el nivel superior de su aplicación.
* [**Babel**](https://babeljs.io/)\*\*\*\*
  * Es una herramienta mayormente usada para convertir código ECMAScript 2015+ en una versión compatible de JavaScript para actuales y antiguos navegadores o ambientes. 



