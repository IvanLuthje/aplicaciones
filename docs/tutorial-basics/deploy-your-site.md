---
sidebar_position: 7
---

# Diseño Responsivo


Como los usuarios pueden acceder a un sitio web desde distintos tipos de dispositivos, se debe lograr que el contenido de una página web se adapte de la mejor forma posible a las dimensiones del dispositivo, para que la información mostrada sea más fácil de comprender.

Se trata crear una aplicación web que tenga la capacidad de redimensionar y colocar los elementos que forman parte del contenido para que se adapte al ancho de cada dispositivo, permitiendo una correcta visualización, navegación y una mejor experiencia de usuario. 
De esta forma, se puede proporcionar a los usuarios de una web los mismos contenidos (o acotados) en forma ordenada y optimizada sea cual sea el soporte.

## Ventajas del diseño responsivo

- Los layouts que estructuran el contenido e imágenes son fluidos y se pueden adaptar facilmente a la pantalla donde se renderiza.
- Permite reducir el tiempo de desarrollo de una app. Creando un solo diseño optimizado para todos los dispositivos en lugar de varios diseños independientes.
- Evitar contenidos duplicados.
- Baja el rebote de usuarios. Una buena parte de los usuarios que abandonan una página web es porque no quieren visualizar correctamente el contenido.
- Aumenta la viralidad de los contenidos, permitiendo que los usuarios compartan el contenido de manera natural y sin problemas.

## Herramientas de Diseño Responsivo

Existen distintas herramientas para adaptar el contenido de la aplicación web a la resolución del dispositivo donde se visualiza:

- Redimensionando
- Ocultando
- Agrandando
- Moviendo
- Encogiendo

Entre ellas encontramos:

- Viewport
- Grid View
- Media Queries

### Viewport

Viewport permite definir las dimensiones del dispositivo que se está utilizando. Si no se define el viewport la página se verá como si fuera de una PC de escritorio.

HTML5 introduce el tag meta viewport que se puede incluir en la sección del head del documento HTML, que nos permite definir el ancho y el alto del área usada por el navegador para renderizar el contenido, y la escala/zoom que debe mostrar inicialmente.

| Atributo | Valores | Descripción |
|---|---|---|
| width | Valor integral en px o constante device-width | Define el ancho del Viewport |
| height | Valor integral en px o constante device-height| Define la altura del Viewport |
| initial-scale | Cualquier número real de 0.1 en adelante. 1 representa no escalable | La escala / zoom inicial del sitio Web |
| user-scale | “yes” / “no” | Define los permisos para que el usuario pueda o no hacer zoom. |
| minimum-scale | Cualquier número real de 0.1 en adelante. 1 representa no escalable | La escala / zoom mínimo del sitio Web |
| maximum-scale | Cualquier número real de 0.1 en adelante. 1 representa no escalable | La escala / zoom máximo del sitio Web |


La configuración recomendada es:

```htm
<meta name="viewport" content="width=device-width", initial-scale=1.0>
```

De esta manera configuramos dos propiedades:

- width=device-width es equivalente al 100% del ancho de la pantalla del dispositivo. Colocar en esta propiedad un ancho en píxeles para definir un tamaño específico puede ser una mala práctica dado que va a mostrar resultados erróneos otros dispositivos o cuando el dispositivo cambia de orientación.

- Height no es necesario definirlo ya que se asignará automáticamente a través del scroll.

- initial-scale=1.0 configura el nivel de zoom inicial cuando el navegador carga la página por primera vez.


## Grid View

Consiste en dividir la estructura de la pagina web, sobre la cual se posicionarán los elementos, en columnas que sirven de soporte para la maquetación.
Este sistema frecuentemente cuenta con 12 columnas, que juntas tienen un ancho del 100% de la página (o contenedor), y se encogerá o expandirá de acuerdo a las dimensiones de la ventana del navegador. El motivo de usar exactamente 12 columnas y no 10, por ejemplo, es la versatilidad que ofrece el número 12, porque tiene muchos factores (es divisible entre 1, 2, 3, 4, 6 y 12).
La utilización de esta herramienta facilita la ubicación de los elementos sobre la página, dado que a cada elemento se le indica cuántas “columnas” ocupará dentro de su contenedor.

## Media Queries

Es la herramienta más importante para lograr aplicar distintos diseños en diferentes dispositivos.
Fue incorporada en la última versión de CSS (CSS3).
Este módulo sirve para detectar no solo el tipo de dispositivo por el que se está navegando, sino que permite aplicar diferentes estilos en base a las propiedades del dispositivo, como el ancho y alto de la ventana del navegador, el ancho y alto del dispositivo, el tipo de pantalla, la resolución del dispositivo y la orientación de la pantalla.
Antes de CSS3, debíamos utilizar JavaScript para obtener información sobre las dimensiones del navegador, y a partir de esa información ajustar las propiedades de los elementos del DOM. La llegada de media queries simplifica mucho esta tarea.

## Media Types

El concepto de media queries no es propio de CSS3, tiene su origen en los media types de CSS2.
Los media types definían como atributo media de los tags, y se lo utilizaban para determinar qué tipo de estilo se iba a aplicar a la página web de acuerdo al tipo de medio donde se estaba proyectando.
Los tipos de medio más comunes son:
- All: Se utiliza para todos los tipos de medios o dispositivos.
- Print: es la vista previa de impresión.
- Screen: para pantallas de ordenador, tablets y teléfonos móviles.
- Tv / Projection: para televisores o proyectores.
- Speech: Se utiliza para lectores de pantalla, generalmente utilizados por personas con discapacidad visual

## Diseño Bottom-up Vs. Top-bottom

**Responsive Web Design (Bottom Up)**: Adaptar y optimizar en contenido al ir reduciendo la ventana del navegador hasta terminar con la versión para moviles.

**Mobile First Web Design(Top-Bottom)**: Adaptar desde la resolución mas pequeña hasta terminar con la versión para escritorio. Simplificar la lectura de los dispositivos moviles, teniendo los recursos limitados

Lo mas recomendable es maquetar en versión mas pequeña optimizando el contenido que se utilice.

## Buenas prácticas del diseño responsivo

Antes de ponerlo en práctica, tener en cuenta:

- Evitar efectos y elementos que puedan hacer lenta la carga de la página. Usar librerías que no carguen recursos innecesarios.

- Tener en cuenta los hábitos de navegación de tus usuarios. Recuerda que necesitan soluciones rápidas y concretas, más si se conectan desde su móvil.

- Evitar la sobrecarga de información, usar textos cortos y botones para que el usuario sepa exactamente qué debe hacer en un momento determinado.

- Los tamaños de las fuentes, las imágenes. los menús y los elementos gráficos deben estar pensados para adaptarse a cualquier tamaño. De hecho algunos recomiendan hacer un desarrollo mobile first.

Los ejes principales del diseño responsivo son:

- Los contenidos del responsive design no se adaptan sino que se expanden.
- Es necesario usar unidades relativas (como el porcentaje de la pantalla), en lugar de unidades estáticas (como los píxeles).
- A menor tamaño de pantalla, el contenido deberá ocupar más espacio vertical.
- Si en el escritorio cuenta con tres columnas para distribuir los contenidos, en los dispositivos móviles sólo cuenta con una columna.
- Usar la anidación. Esta técnica hará que las pantallas se adapten a pantallas contraídas.
- Dependiendo de dispositivo, el contenido debe extenderse para ocupar todo el ancho de la pantalla.
- No hay grandes diferencias entre desarrollar un nuevo proyecto en pantalla grande o chica.
- Si el diseño contará con muchos efectos o detalles, lo más recomendable es utilizar vectores.


## Depuración

Los navegadores tienen incorporada herramientas para realizar depuraciones que permiten:

- Manipular el DOM.
- Editar y depurar JavaScript, css.
- Realizar auditorías del sitio para verificar el nivel de optimización alcanzada, evaluando la performance, analizando recursos consumidos.
- Permite emular pantallas de celular, diferentes tamaños de pantalla y resoluciones del dispositivo.
- Permite simular valores de distintos sensores (eventos táctiles, orientación del dispositivo, acelerómetro) y coordenadas de geolocalización.






Si en el escritorio cuenta con tres columnas para distribuir los contenidos, en los dispositivos móviles sólo cuenta con una columna.



<!-- Docusaurus is a **static-site-generator** (also called **[Jamstack](https://jamstack.org/)**).

It builds your site as simple **static HTML, JavaScript and CSS files**.

## Build your site

Build your site **for production**:

```bash
npm run build
```

The static files are generated in the `build` folder.

## Diseño Responsivo

Test your production build locally:

```bash
npm run serve
```

The `build` folder is now served at [http://localhost:3000/](http://localhost:3000/).

You can now deploy the `build` folder **almost anywhere** easily, **for free** or very small cost (read the **[Deployment Guide](https://docusaurus.io/docs/deployment)**). -->
