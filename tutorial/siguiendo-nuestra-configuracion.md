# Siguiendo nuestra configuración

El punto de entrada para nuestra aplicación sera el elemento div  con **id** `root` , el cual es llamado así por convención. También notaras que el script type `text/babel` el cual es obligatorio para el uso de Babel.

Ahora, vamos a escribir nuestro primer bloque de código en React. Es por ello que crearemos nuestra primer clase definida en el script `text/babel` 

Vamos a usar clases de ES6 para crear un en React llamado `App`  

```text
class App extends React.Component {
    //...
}
```

Ahora añadiremos el método `render`,  el cual es el único método obligatorio en un clase componente, el cual es usado para mostrar los nodos del DOM.

```text
class App extends React.Component {
  render() {
      return (
          //...
      );
  }
}
```

Vamos a colocar dentro del `return`, lo que parece como un simple bloque de HTML elemento. Note que NO vamos a retornar un string aquí, así que no usemos el símbolo `" "` alrededor del elemento. Esto es llamado `JSX`, y aprenderemos sobre esto mas adelante.

```text
class App extends React.Component {
    render() {
        return (
            <h1>Hello world!</h1>
        );
    }
}
```

Finalmente 

