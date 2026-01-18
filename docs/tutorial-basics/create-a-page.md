---
sidebar_position: 2
---

# HTML

 Lenguaje en el cual se escriben las páginas web, que es interpretado por navegadores para dibujar y mostrar el contenido de la página web a los usuarios. Es un lenguaje de etiquetas, ya que todos los elementos que definen los componentes que forman parte de la página web se definen a partir de etiquetas.

Se crea el estandar CSS para separar el diseño del contenido.

Se definen estas etiquetas para definir los distintos elementos y secciones que componen un documento HTML como párrafos, enlaces, imágenes, listas, tablas, encabezados, cuerpo y pie de página, etc.

Las etiquetas se indican por pares y se indican de la siguiente forma:

Apertura etiqueta y Cierre /etiqueta

Un elemento **NO ES LO MISMO QUE UNA ETIQUETA, PERO UNA ETIQUETA DEFINE AL ELEMENTO,** está formado por etiquetas de apertura y cierre, atributos y contenido.

**p class='nombre_clase'Párrafo/p** 

donde **p** es la etiqueta de inicio, la clase es un atributo, el valor de la clase o atributo y la palabra Párrafo es el contenido.

Hay cuatro tipos de atributos:

- Básicos: Se pueden utilizar con todas las etiquetas: id, class, style, title
- Internalización: Se usan para mostrar el contenido en distintos idiomas: lang
- Eventos: Acciones dinámicas sobre los elementos onChange, onClick, onFocus
- Atributos en foco: Accesibilidad

**Doctype:** Permite mostrar la página correctamente ya que existen distintos tipos de documentos HTML, a partir de HTML5 se declara 

DOCTYPE html

**h1-6:** Son los títulos de sección y permite dividir las páginas en secciones jerárquicas, h1 es la sección de mayor importancia y h6 es la de menor importancia. Ayuda a los navegadores para indexar estructura y contenido de las páginas 

 **p:** Etiqueta que define párrafos, varios espacios seguidos se consideran como uno y varias lineas seguidas son consideradas como una. El navegador elimina espacios y lineas extras antes de mostrar contenido al usuario.

**a:** Etiqueta para definir enlaces (hipervínculos), el link es el elemento principal para el hipertexto. Mediante un click permite acceder a otros documentos y/o a otros recursos web. Existen distintos tipos de enlaces: locales, externos o internos al documento. Se puede definir sobre un texto, imagen y otro elemento HTML. href indica la URL del recurso que se va a enlazar.

**URL absolutas:** URL completa

**URL relativas:** Se construyen a partir de las absolutas y prescinde de algunas partes como protocolo y servidor.

**Links Locales:** Son enlaces a documentos del mismo sitio web

**Links Externos:** Se dirigen a otro documento perteneciente a otro sitio web (URL absoluta)

**Links Internos:** Son enlaces que permiten el desplazamiento sobre el mismo documento, para ir a una sección específica de la página

**Bookmarks:** Se utilizan para sitios web con páginas extensas, se define la etiqueta name, se crea el bookmark y luego se enlaza a la sección correspondiente. Cuando el link se clickea, la página automáticamente hace scroll hacia la ubicación de ese bookmark. Se utiliza href seguido de # con el nombre de la sección.

**img:** Se utiliza para definir imágenes, es una etiqueta vacía que no necesita cerrarse. Se define el atributo **src** para definir la URL de la imagen que se va a mostrar y el atributo **alt** para definir un texto alternativo para la descripción de la imagen.

**Listas:** ul lista desordenada, ol lista ordenada y dl lista de definiciones, donde es una lista de términos con descripción para c/u de ellos y las anidadas, que son listas dentro de otras.

li list item: Esta etiqueta se define para cada item de la lista.

**Tablas (deprecado):** Se definen con la etiqueta table. Las filas se crean utilizando tr, las columnas que contienen los datos td, el encabezado de la tabla con th, el tag caption para agregar titulo a la tabla inmediatamente despues del tag table y la celda vacía se define como **td&nbsp;/td. Se utilizaban antiguamente para definir la estructura de páginas web.**

**Elementos en bloque vs Elementos en linea:** Todos los elementos HTML tienen un modo de visualización de acuerdo al tipo de elemento que es.

Existen dos tipos de elementos, su diferencia radica en la forma que ocupan el espacio disponible en pantalla.

- **Elementos de bloque:** Comienzan en una nueva línea y ocupan todo el ancho disponible **div - p - form**
- **Elementos en línea:** No necesariamente comienzan en una nueva línea y sólo ocupan el ancho que necesitan **span - a - img**

**div**: Elemento de bloque para definir zonas o divisiones de una página web, utilizado también como un elemento contenedor de otros elementos HTML. No tiene atributos obligatorios.

**span**: Elemento en línea, funciona como un contenedor de textos. No tiene atributos obligatorios.

**Atributos globales:** Pueden ser configurados en todos los elementos HTML mencionados, los más importantes son:

- Id: Permite identificar a un elemento específico del documento, por lo que deben ser únicos.
- Class: Se utilizan para agrupar elementos con características y propiedades comunes.
- Style: Agregar propiedades CSS a un elemento. Se utiliza en la etapa de diseño para realizar pruebas. No es recomendable pasarlo a producción, para ello se define un archivo CSS.

**Layout:** Representa estructura básica del sitio, define la disposición general de los elementos comunes a todas o a la mayoría de las páginas que conformar el sitio web. Se dividen en bloques o secciones.

Modos de armar el layout:

- **Mediante tablas:** Las filas y columnas se utilizaban para representar las distintas secciones. Se definían al menos tres filas: una para la cabecera, otra para el menú y los contenidos, y la última para el pie de página. Este modelo quedó obsoleto.
- **Mediante contenedores Div y Span:** Estos elementos son fácilmente manipulables desde CSS. Por lo que principalmente son aptos para el diseño responsivo. Se lograron las siguientes mejoras: Mantenimiento, Velocidad de carga y Diseño.

**Tags semánticos**: Se utilizan para reemplazar los contenedores div y span para separar los contenidos del sitio. Son elementos con un significado propio que describen claramente su contenido. Un tag semántico no fue diseñado para estructurar el layout sino para ayudar al programador a identificar las distintas secciones del documento HTML.

**Header:** Encabezados, pueden haber varios en un mismo documento, en el cual contiene elementos de identidad, logos y nombre de la organización y eslóganes y elementos de navegación el sitio.

**Nav:** Define el menú principal de navegación del sitio, por lo tanto, define un conjunto de links para navegar hacia otras secciones o páginas del sitio. Se utiliza para bloques de navegación dentro de un documento.

**Main:** Contenido principal de la página y es el contenedor del elemento section, es único y agrupa justo el contenido deseado y no se permite agrupar elementos como anuncios y barras laterales.

**Section:** Permite agrupar contenido relacionado, representa una sección del documento con elementos del mismo tema.

**Article:** Similar a la sección que por sí solo tiene razón de ser y significado. Por ejemplo: post de "blogs", artículos de una revista digital, noticias de un periódico digital y opiniones de un foro.

**Aside:** Contenido menos importante del sitio, se define como barra lateral de una página web. Utilizado para calendarios, publicidad, notas, redes sociales relacionadas, info de contacto, etc.

**Footer:** Pie de página, en la cual se define información como contacto, derechos de autor y avisos legales. Al igual que el header pueden haber varios en el mismo documento.

**Form:** Etiqueta que define un formulario, son usados para recolectar datos que ingresa el usuario para que posteriormente sean procesados, permiten enviar requerimientos con estos datos al servidor. 

**Input:** Define los distintos tipos de datos que puede ingresar el usuario, es el más importante y utilizado, se debe indicar el tipo de dato que se espera recibir en el campo mediante el atributo **type**

**Action:** Posee la URL que indica a dónde se van a enviar los datos del formulario

**Method:** Define el método HTTP usado para enviar los datos ingresados por los usuarios:

- **GET:** No permite enviar archivos adjuntos y los datos enviados se ven en la barra de direcciones
- **POST:** Los datos enviados no se pueden ver tan fácilmente y permite enviar muchos más datos.

**Name:** Establece el nombre del formulario

**Target:** Indica donde se mostrará la respuesta que reciba del servidor (_blank, _self, _parent, _top).

**Textarea:** Elemento que permite crear una lista desplegable y se define con la etiqueta textarea. Los atributos son:

- name (texto): Define el nombre
- cols (numero): Define el ancho visible
- rows (número): Define la cantidad visible de lineas
- disabled: Input deshabilitado
- readonly: Indica que el texto es de sólo lectura

**Select**: Elemento que permite el acceso de texto multilinea, cada ítem de la lista se define con la etiqueta option. Los atributos son:

- name
- size (número): Cantidad de opciones visibles en la lista desplegable
- disabled
- multiple: Indica que se pueden seleccionar más de una opción

**optgroup:** Elemento que permite agrupar opciones relacionadas dentro de la lista desplegable. Los atributos son:

value (texto): Definir el valor a ser enviado por el servidor

selected: Indica que la opción es preseleccionada

disabled: Opción deshabilitada

label (texto): Define un rótulo breve para una opción

fieldset: Elemento que permite agrupar elementos relacionados dentro de un mismo formulario.

**Head:** Se encuentran relacionados con el propio documento HTML y no con su contenido, permiten definir:

- Titulo del documento
- Estilos
- Scripts
- Links
- Metadatos

**Title:** Establece el título de la página, los navegadores muestran este atributo como el título de ventana del navegador. Es utilizado por los motores de búsqueda y colocado como el título de resultados de búsqueda realizadas por los usuarios. Elemento obligatorio en cualquier documento HTML.

**Link:** Elemento que permite definir relaciones entre documentos HTML y otros documentos y recursos.

**Metadatos**: Se define con la etiqueta **meta**.

- Permite especificar información importante sobre la página como la descripción de la página, palabras claves, autor, etc.
- Se pueden incluir varios metadatos especificando propiedad y valor.
- Es usada por los browsers, por motores de búsqueda y por otros servicios web.
- Generalmente se utilizan sólo los atributos “name” y “content”.
- **http-equiv**: define el intervalo de tiempo en segundos para que el documento se actualice o refresque
- **Charset**: establece el estándar de codificación de caracteres utilizado

**Viewport**: Metadata para definir el ancho, alto y escala del dispositivo que se está utilizando. Si no se define el viewport la página se verá como si fuera de una PC de escritorio.

**Apple-mobile-web-capable**

- Es de Apple, pero es compatible con Android.
- Define que una aplicación se ejecute en modo Fullscreen.
- Sólo tiene efecto si la aplicación ha sido agregada previamente en marcadores.
- Se puede realizan otras configuraciones para que se vea en pantalla completa como una aplicación nativa, y hasta crear un acceso directo en el menú de aplicaciones.

**Format-detection**

- Existe una opción para que cualquier número que parezca un teléfono se transforme automáticamente en un enlace que el usuario puede clickear para llamar a ese número
- Mediante este meta tag se puede habilitar o deshabilitar esta detección automática
- Se pueden detectar direcciones postales y de correo con la misma técnica
- Sirve con Android y iOS

**Cambios de HTML5**

- La declaración del documento es muy simple: DOCTYPE html
- Se incorporan los elementos semánticos: header - main - section - article - aside - footer
- Se crean nuevos atributos de control de formularios: “number” – “date” – “time” – “calendar”
- Se puede complementar con otras apis: Geolocation y LocalStorage
- Se agregan archivos multimedia de audio y video

**XHTML**

- Es una remodelación HTML, una versión más robusta.
- Es una adaptación de HTML al lenguaje XML.
- Surgió ante los problemas de compatibilidad que existían cuando se abría un documento HTML en distintos navegadores.
- La sintaxis del lenguaje HTML es muy permisivo.
- XHTML es mucho más estricto para evitar errores a la hora de ser interpretados por los navegadores.
- Documentos donde se especifican qué elementos forman el contenido y no cómo tiene que verse cada cosa.
- Por esta razón, se eliminan todas las etiquetas y atributos que sirven para definir el aspecto.
- Establece las siguientes normas:
    - Las etiquetas se tienen que cerrar de acuerdo a cómo se abren, es decir manteniendo el orden.
    - Los nombres de las etiquetas y atributos siempre se escriben en minúscula.
    - El valor de los atributos se encierra siempre entre comillas.
    - Todas las etiquetas deben cerrarse siempre, incluso las etiquetas no tienen cierre.



- `src/pages/index.js` → `localhost:3000/`
- `src/pages/foo.md` → `localhost:3000/foo`
- `src/pages/foo/bar.js` → `localhost:3000/foo/bar`

## Create your first React Page

Create a file at `src/pages/my-react-page.js`:

```jsx title="src/pages/my-react-page.js"
import React from 'react';
import Layout from '@theme/Layout';

export default function MyReactPage() {
  return (
    Layout
      h1My React page/h1
      pThis is a React page/p
    /Layout
  );
}
```

A new page is now available at [http://localhost:3000/my-react-page](http://localhost:3000/my-react-page).

## Create your first Markdown Page

Create a file at `src/pages/my-markdown-page.md`:

```mdx title="src/pages/my-markdown-page.md"
# My Markdown page

This is a Markdown page
```

A new page is now available at [http://localhost:3000/my-markdown-page](http://localhost:3000/my-markdown-page).
