---
description: >-
  Casi todo en React consiste en componentes, de los cuales puede ser class
  components o simple components.
---

# Componentes

Muchas aplicaciones React poseen componentes pequeños y todo es cargado dentro del componente principal `App.js` . Los componentes muy a menudo tiene su propio archivo. así que cambiemos un poco nuestro proyecto para ello.

Eliminemos la clases App de nuestro `index.js` , lucirá algo como esto.

{% code-tabs %}
{% code-tabs-item title="src/index.js" %}
```text
import React from 'react'
import ReactDOM from 'react-dom'
import App from './App'
import './index.css'

ReactDOM.render(<App />, document.getElementById('root'))
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Ahora crearemos un nuevo archivo llamado  `App.js`  y allí colocaremos el componente.

{% code-tabs %}
{% code-tabs-item title="src/App.js" %}
```text
import React, { Component } from 'react'

class App extends Component {
  render() {
    return (
      <div className="App">
        <h1>Hello, React!</h1>
      </div>
    )
  }
}

export default App
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Aquí lo que se realizo fue exportar el componente como `App` y cargarlo en el`index.js` No es obligatorio separar los componentes en archivos pero una aplicación comenzara a volverse difícil de manejar si no se hace.

