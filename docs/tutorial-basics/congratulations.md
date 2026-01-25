---
sidebar_position: 7
---

# LocalStorage

En las aplicaciones web, las peticiones entre un navegador y el servidor se realizan bajo el protocolo HTTP. Este protocolo es stateless, o sin estado, es decir que los servidores no persisten ninguna información sobre la petición realizada por el cliente, sólo se limitan a devolver el recurso solicitado. Para el servidor, una petición es indistinta de otra inmediata.

Para solucionar esta limitación surge el concepto del manejo de COOKIES

## Cookies
Las cookies son pequeños pedacitos de información que viajan en cada petición entre el cliente y el servidor.
El funcionamiento a grandes rasgos es el siguiente: 
- El servidor para identificar un usuario le asigna un ID único a cada cliente. 
- El cliente le enviará dicho identificador en cada una de las próximas peticiones al servidor.
- Posteriormente, cuando el servidor la recibe, comprueba que el ID sea válido (es decir, matchea en una base de datos local a qué usuario le asignó ese identificador) y lo reconoce. De esta forma se puede establecer finalmente una sesión entre el cliente y servidor.

Vale aclarar que queda a cargo del desarrollador de backend implementar la asignación y validación de cada ID generado y recibido de cada cliente.

Características de las cookies:

- Acceso a la información desde el servidor.
- Tienen caducidad, es decir expiran y se borran después de un determinado tiempo.
- Espacio limitado: Una cookie sólo puede ocupar 4kb de espacio. 
- Cada vez que se realiza una petición al servidor, toda la información guardada en las cookies (hasta 4Kb) deben viajar al servidor y volver. En el intercambio de información siempre viajan las cookies.
- Cada dominio almacena todas sus cookies en una sola cadena, lo que puede dificultar el análisis de los datos.
- Los datos no están encriptados.
- La inyección de SQL se puede realizar desde una cookie.

## Cookies Vs Storage
Las cookies resultaron la herramienta más útil durante mucho tiempo. Por la evolución de los navegadores y el avance hacia HTML5, se está dejando a un lado el concepto de utilizar Cookies, y se está migrando a LocalStorage y SessionStorage.

Ambas herramientas tienen similitudes, ya que consisten en almacenar información en el equipo del usuario que accede a la página web. Pero la diferencia es que las sólo los datos almacenados en las Cookies son y enviados y compartidos con el servidor.

Por lo tanto, la gran ventaja de las cookies es que podemos almacenar información accesible desde el servidor. Pero hay muchos otros casos en que sólo queremos persistir la información en el lado del cliente.



## Ejemplos de almacenamiento del lado del cliente:

- Llevar un control de usuarios

- Gustos y preferencias de usuarios. Guardar información sobre los hábitos del usuario.

- Manejo de historial: últimas búsquedas realizadas por el usuario.

- Guardar temporalmente resultados de una llamada a un webservice

- Mantener estado de la interfaz de usuario de manera sencilla.

- Compartir datos entre páginas del mismo sitio web. Ejemplo: implementación de un carrito de compras.

## Storage

El objeto Storage es una API de almacenamiento web, que nos permite almacenar datos de manera local en el navegador del usuario y sin necesidad de realizar alguna conexión a una base de datos. De una manera muy similar a como lo hacen las Cookies.

### LocalStorage Vs SessionStorage

HTML5 introduce las propiedades LocalStorage y SessionStorage, que tienen la capacidad de acceder al objeto Storage para almacenar datos de forma local. La diferencia entre ellas es que localStorage almacena los datos en forma indefinida o hasta que son eliminados explícitamente del navegador, mientras que sessionStorage almacena información mientras la ventana donde se esté utilizando siga abierta; una vez cerrada, la información se elimina.

Esta última es una solución ideal para los casos en los que solo necesitamos la información temporalmente (formularios encadenados o anidados, en distintas páginas de un asistente que recoge datos, etc.).

### API Storage

Validar storage en navegador: Valida que el navegaor sea compatible con el objeto storage

  ```javascript
  if (typeof(Storage) !== 'undefined'){
    // Codigo cuando storage es compatible
  } else {
    // Codigo cuando storage NO es compatible
  }
  ```
Guardar datos en storage

  ```javascript
  
  localStorage.setItem('Nombre','Ivan')
  localStorage.Apellido = 'Luthje'
  
  ```

  ```javascript
  
  let FirstName = sessionStorage.getItem('Nombre')
  LastName = sessionStorage.Apellido

  ```

Recuperar datos en storage

  ```javascript
  
  let FirstName = localStorage.getItem('Nombre')
  LastName = sessionStorage.Apellido
  
  ```

  ```javascript
  
  sessionStorage.setItem('Nombre','Ivan')
  localStorage.Apellido = 'Luthje'

  ```
Eliminar datos del storage

```javascript

  localStorage.removeItem(Apellido)
  
```
```javascript

  sessionStorage.removeItem(Apellido)
  
```
Limpiar todo el storage

```javascript

  localStorage.clear()
  
```
```javascript

  sessionStorage.clear()
  
```

### Ventajas de LocalStorage

- Si bien el espacio es limitado, los datos pueden ocupar hasta 5 o 10 MB dependiendo del navegador, incluyendo texto y multimedia.
- La información almacenada en la computadora del cliente no es enviada al servidor en cada petición.
- No existe caducidad para LocalStorage, sino que la información queda almacenada hasta que se la elimine expresamente.
- No afecta la performance del sitio
- La información es guardada y organizada por dominio web.
- Soporte por la mayoría de los navegadores modernos.

### Desventajas de LocalStorage

- Si el servidor necesita información almacenada del cliente, debe enviarla por otro medio.
- Solo se pueden almacenar cadenas de texto. No pueden almacenar otro tipo de objetos como booleanos, enteros, arreglos entre otros. Para solucionar esto, se utiliza JSON.

### Solución de JSON

Crear un objeto JS

```javascript
var persona = {
    nombre: "pepe",
    edad: 20,
    locura: true
}
```

Guardar y recuperar objeto en localStorage

```javascript
var personaAGuardar = JSON.stringify(persona);

localStorage.setItem("persona", personaAGuardar);
var personaGuardada = localStorage.getItem("persona");

console.log(typeof persona); //objeto
console.log(typeof personaGuardada); //string

var personaGuardada = JSON.parse(personaGuardada);
console.log(personaGuadada.locura); //true


```


<!-- You have just learned the **basics of Docusaurus** and made some changes to the **initial template**.

Docusaurus has **much more to offer**!

Have **5 more minutes**? Take a look at **[versioning](../tutorial-extras/manage-docs-versions.md)** and **[i18n](../tutorial-extras/translate-your-site.md)**.

Anything **unclear** or **buggy** in this tutorial? [Please report it!](https://github.com/facebook/docusaurus/discussions/4610)

## What's next?

- Read the [official documentation](https://docusaurus.io/)
- Modify your site configuration with [`docusaurus.config.js`](https://docusaurus.io/docs/api/docusaurus-config)
- Add navbar and footer items with [`themeConfig`](https://docusaurus.io/docs/api/themes/configuration)
- Add a custom [Design and Layout](https://docusaurus.io/docs/styling-layout)
- Add a [search bar](https://docusaurus.io/docs/search)
- Find inspirations in the [Docusaurus showcase](https://docusaurus.io/showcase)
- Get involved in the [Docusaurus Community](https://docusaurus.io/community/support) -->
