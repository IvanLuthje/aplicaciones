---
sidebar_position: 3
---

# CSS

**CSS:** Lenguaje de hojas de estilos creado para controlar la presentación y aspecto de los documentos HTML. Es la mejor forma de separar el contenido de la página web de su presentación. Definido como un estándar por la W3C. En el CSS se puede definir como se muestran los elementos del documento HTML, como por ejemplo color, tamaño, tipo de letra, separación horizontal y vertical entre elementos, posición de cada elemento en la pantalla, etc.

El CSS obliga a crear documentos HTML semánticos, mejoran la accesibilidad del documento, reduce la complejidad de su mantenimiento, visualizar el mismo documento en dispositivos diferentes y se puede controlar el estilo y formato de múltiples páginas simultáneamente.

Esta forma de definir el aspecto de los elemento no es la más adecuada, ya que si tuviéramos una página con 50 elementos, habría que insertar 50 etiquetas Font, del mismo modo si un sitio web se compone de 10.000 etiquetas, habrá que definir 10.000 atributos

Con CSS se pueden establecer los mismos estilos con menor esfuerzo y sin ensuciar el código HTML de los contenidos.

Flexibilidad y diferentes opciones para hacer una misma tarea. Existen al menos 3 opciones para incluir CSS en un documento HTML:

- **Incluir directamente CSS en los elementos HTML:** Es el peor y menos utilizado ya que tienen el inconveniente que la utilización de etiquetas font, se utiliza en situaciones en las que se debe incluir un estilo muy específico para un solo elemento concreto, se define con el atributo style de los elementos definidos en HTML.
- **Incluir CSS dentro del documento HTML:** Se define dentro del head con la etiqueta style y se utiliza cuando un número pequeño de estilos se definen sobre un único documento. Soluciona el problema anterior pero se aplica solamente en un solo documento.
- **Definir CSS en un archivo externo (Recomendado):** Se definen en un archivo de extensión .css y el nombre del archivo se define dentro del head por medio de la etiqueta link. El mantenimiento se simplifica al máximo y se puede utilizar en todos los documentos indicando ese archivo .css.

La regla de CSS está conformada por Selectores (Nombre del elemento, pueden ser varios) y Declaraciones (propiedades del elemento con sus respectivos valores)

Los selectores disponibles son:

- Universales (*): Se utiliza para seleccionar a todos los elementos de la página
- Tipo o Etiqueta: Se utiliza para seleccionar todos los elementos de la página cuya etiqueta HTML coincide con el nombre del selector (h1,h2,p,etc.)
- Descendente: Selecciona subelementos dentro de otros elementos (p span, h1 a, etc.)
- Selector de ID (#): Selecciona un único elemento HTML a partir de un atributo ID
- Clase (.): Selecciona los elementos HTML con el atributo class.
- Comentarios: Describir de manera breve y estructurar de manera clara los archivos CSS complejos.

Para resolver colisiones de estilos se siguen estas reglas:

- Determinar todas las declaraciones que se aplican al elemento seleccionado
- Ordenar las declaraciones según su origen y prioridad:
    - Por defecto del navegador
    - Hoja de estilos Externa
    - Hoja de estilos Interna
    - Estilo Inline

- Ordenar las declaraciones según lo especíico que sea el selector (mas especifico - menor importancia)
- A igual especificidad la propiedad queda determinada por el orden que se procesan, se tomará la última regla.

**Modelo de Cajas:** Una de las características más importantes del lenguaje, es un comportamiento CSS que hace que todos los elementos de la página se representen mediante cajas rectangulares, estas cajas se crean automáticamente cada vez que se define una etiqueta HTML. Los navegadores son los que crean y colocan las cajas automáticamente y con CSS se pueden modificar todas o algunas de sus características.

- Margin: Area transparente alrededor del borde que permite separar las cajas con el resto de las cajas subyacentes.
- Border: Linea que encierra completamente el contenido y el padding. Afectado por el background-color de la caja.
- Padding: Area vacía alrededor del contenido. Afectado por el background-color
- Contenido: Espacio que contiene elementos HTML.

**Dimensiones de los elementos:** Unidades para representar la altura, ancho y márgenes de los elementos y para el tamaño de las letras de un texto, son relativas.

**Em:** Tamaño de letra de un elemento.

**Px:** Tamaño de resolución de pantalla del dispositivo.

**%:** Referencia a otra medida. Se utiliza para establecer el ancho de un elemento, la referencia será en proporción del elemento padre.

Las dimensiones se pueden definir de acuerdo a las siguientes reglas:

- Para definir las dimensiones de elementos que forman parte del layout, es decir, que estructuran a la página, se recomienda uasr porcentajes, dado que permiten crear diseños dinámicos que se adapten a las dimensiones del dispositivo.
- Para la altura de los elementos se pueden usar píxeles (px).
- Para definir el tamaño de la letra de los textos se pueden usar la unidad “em”.

Importancia de CSS3

- Es la última versión del estándar.
- Una de sus diferencias es la separación de módulos, donde cada uno cuanta con distintas características. Los módulos más destacados son:
    - Media Queries: permite adaptar el contenido a las dimensiones del dispositivo: Dimension del Viewport – Orientación – Resolución de pantalla.
    - Múltiples imágenes de fondo y bordes con imágenes.
    - Efectos en el texto.
    - Animaciones de elementos HTML sin el uso de Flash y JS.
    - Transiciones.

Buenas prácticas de CSS

- Minimizar requerimientos HTTP puede reducir el tiempo de respuesta
- Los navegadores tienen sus propios estilos, es recomendable tener estilos que se normalicen o reseteen lo estilos de los navegadores.
- **Normalizadores**: El CSS del diseñador no es el único CSS que se está ejecutando, sino que los navegadores tienen sus propios estilos, y los aplica automáticamente al renderizar
el sitio.
Pero no todos los navegadores tienen los mismos estilos CSS entre ellos.
Esto crea conflictos, dado que una página puede llegar a verse de una forma en un navegador y de otra forma en otro, aunque tengan el mismo CSS y el mismo HTML.
Los normalizadores regulan las características que pueden verse afectadas por las diferencias entre navegadores. Es recomendable tener estilos que normalicen o reseteen los estilos de los navegadores.
Un normalizador posible es:
**Normalize** - https://necolas.github.io/normalize.css/