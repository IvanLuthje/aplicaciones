---
sidebar_position: 1
---

# Aplicaciones hibridas

## Introducción

Reúne lo mejor de los las aplicaciones web y nativas.

Se desarrolla con lenguajes de programación de las web apps como HTML, CSS y JavaScript. Multiplataforma.

Brinda la posibilidad de acceder a las capacidades del dispositivo.

Aplicación web móvil que se comporta como una aplicación nativa.

Una vez que la aplicación está terminada, se compila generando un ejecutable.

La ejecución se realiza a través de una vista WebView, utilizada para visualizar el contenido en pantalla completa.

## Ventajas

- Uso de los recursos del dispositivo y sistema operativo.
- Costo menor que una app nativa.
- Multiplataforma.
- Ejecución offline.
- Distribución mediante distintas plataformas.
- La aparición de nuevos Frameworks y librerías facilita cada vez más el desarrollo

## Desventajas

- Performance es mayor que una web app pero menor que una aplicación nativa.
- Diseño visual puede estar afectado por el sistema operativo sobre el cual se ejecuta.
- No es la mejor opción si se requieren rendimientos gráficos elevados

## Tipo de Aplicaciones híbridas

1) Aplicaciones Shell nativas que contienen un sitio web externo

El desarrollo es igual que el de las aplicaciones web, los recursos web de la aplicación se encuentran en un servidor remoto. La diferencia es que la aplicación es compilada y ejecutada por el WebView y no por el navegador

2) Recursos Web preempaquetados

Es la forma más común de desarrollar. En este caso los recursos web no se obtienen de un servidor web externo, sino que se encuentran empaquetados dentro de la propia aplicación

3) Combinación de elementos web con nativos. Existen dos modelos:

- La aplicación se diseña como una aplicación web a la que se agregan componentes nativos para representar la interfaz de usuario
- La aplicación es principalmente nativa y se añaden pantallas HTML



## Utilización de Aplicaciones Hibridas

Son útiles cuando:
- Se necesita desarrollar en poco tiempo aplicaciones sencillas que se utilizan todas las plataformas.
- Cuando se requiere utilizar conocimientos existentes Vs. aprender los lenguajes nativos de cada plataforma
- Para aplicaciones que muestran pocos datos y que no requieren demasiadas animaciones



## Frameworks hibridos

- Funcionan como medio de comunicación entre la aplicación web móvil y los recursos del dispositivo
- Ofrecen librerías desarrolladas en JavaScript para acceder a las capacidades de los dispositivos móviles
- Compilan el código desarrollado en los lenguajes de programación web (HTML, CSS y JavaScript) para mejorar la performance de la aplicación
- El lenguaje predominante de todos los frameworks es JavaScript

- Facilitan la creación de aplicaciones híbridas:
    - Plugins para acceder a las funciones nativas
    - IDE y simuladores para pruebas de las aplicaciones en distintas resoluciones
    - Servicio de compilación de la nube, evitando tener que configurar ambientes de desarrollo para múltiples plataformas
    - Proveen servicios backend de uso común en aplicaciones móviles como notificaciones PUSH o administración de usuarios

- Proveen servicios backend de uso común en aplicaciones móviles como notificaciones PUSH o administración de usuarios
- Asistentes para publicación de las aplicaciones en las App Stores
- Desarrollo colaborativo de aplicaciones

**React Native**

Creado por Facebook, React Native se encuentra entre los mejores frameworks de aplicaciones híbridas en términos de eficiencia y rendimiento. Los desarrolladores pueden usar JavaScript y React para escribir aplicaciones móviles totalmente nativas tanto en iOS como en Android, contribuyendo prácticamente a la misma base de código. Esto se hace fácil, rápido y compartible en términos de código entre una aplicación web y una móvil, gracias a la evidente ayuda de la recarga en caliente y una gran comunidad de desarrollo .

La integración del módulo nativo probablemente sería un poco compleja para los novatos, pero en general, ese es el beneficio general de este paquete, lo que lo convierte en una de las principales soluciones para el desarrollo de aplicaciones híbridas .

Características principales

Recarga en caliente : con esto, cualquier actualización en la aplicación es visible sin tener que crear la aplicación completa.
Módulos nativos : interactúa directamente con las API nativas a través de JavaScript.
Impulsado por la comunidad : gracias a que esta plataforma cuenta con un apoyo masivo de la comunidad, hay muchas bibliotecas y herramientas que dan como resultado una gran riqueza de funciones.
Ventajas

Rendimiento : Rendimiento casi nativo porque se accede directamente a los componentes nativos.
Reutilización : El código es reutilizable tanto en la plataforma web como en dispositivos móviles.
Popularidad : La gran comunidad y el respaldo corporativo han dado como resultado desarrollos continuos y recursos inmensos.
Desventajas

Complejidad : puede volverse complejo cuando se integra con módulos nativos.
Depuración: siempre es la parte más desafiante de todo, especialmente para aplicaciones complejas.

**Flutter**

Flutter es desarrollado por Google . Flutter es una de las potentes herramientas que han facilitado el desarrollo de aplicaciones móviles visualmente atractivas y muy funcionales. Se basa en el lenguaje de programación Dart y ofrece conjuntos de widgets prediseñados muy potentes que cumplen con los estándares de Material Design y Cupertino. Los desarrolladores que usan Flutter pueden ver los efectos de los cambios al instante gracias a la función de recarga en caliente.

Si bien el lenguaje Dart no es popular entre los desarrolladores, tener Flutter compilado en código nativo permitió un rendimiento fluido y una sensación bastante natural en varias plataformas.

Características principales

Recarga activa : obtenga una vista previa instantánea de los cambios que realice en el código.
Rich Widgets : una extensa lista de widgets prediseñados que cumplen con los estándares Material Design y Cupertino.
Lenguaje Dart : Adopte el lenguaje de programación Dart, fácil de aprender y muy productivo.
Ventajas

Rendimiento : Alto rendimiento debido a la compilación directa a código nativo.
Interfaz de usuario flexible : widgets personalizables que se pueden utilizar para crear interfaces de usuario expresivas y flexibles.
Escribe una vez e implementa en todas partes: una vez escrito, se puede implementar en cualquier lugar, ya sea en dispositivos móviles, la web o el escritorio.
Desventajas

Cuantificar : Se rumorea que el tamaño de las aplicaciones es mayor que el de otros marcos.
Curva de aprendizaje : El lenguaje Dart no está en manos de los programadores.

**Ionic**

Ionic es un framework de código abierto que utiliza tecnologías web como HTML , CSS y JavaScript para crear aplicaciones móviles, tanto para Android como para iOS . Es fácil de usar, muy flexible y cuenta con una amplia biblioteca de componentes de interfaz de usuario prediseñados que se integran fácilmente con Angular o React , plataformas utilizadas principalmente por desarrolladores front-end.

Puede que no esté al nivel de rendimiento de las aplicaciones totalmente nativas, pero esa es una de las razones por las que Ionic está a la vanguardia en el desarrollo de aplicaciones híbridas: puede integrarse con Capacitor y, por lo tanto, usar funcionalidad nativa.

Características principales

Multiplataforma : cree aplicaciones iOS , Android y web, todas desde el mismo código fuente.
Componentes de interfaz de usuario con estado : amplia biblioteca de componentes, ya prediseñados.
Integración con Capacitor: es el entorno de ejecución nativo más reciente y moderno que se utiliza para agrupar funcionalidades nativas.
Ventajas

Tecnologías web : utiliza tecnologías web comunes y, por lo tanto, es fácil de readoptar para los desarrolladores web.
Comunidad : Comunidad fuerte, gran apoyo y todo el camino hasta allí.
Fácil integración : se puede integrar fácilmente con otros marcos como Angular, React o Vue.
Desventajas

Rendimiento : No es exactamente igual que las aplicaciones totalmente nativas.
Funcionalidad nativa : puede haber algunas funcionalidades nativas que se vuelvan difíciles de implementar al implementarlas mediante complementos.

**Xamarin**

Xamarin , propiedad de Microsoft , es uno de esos potentes frameworks que permite el desarrollo de aplicaciones nativas multiplataforma mediante C# en .NET Framework . Admite hasta un 90% de compartición entre plataformas iOS , Android y Windows , ofreciendo un rendimiento casi nativo gracias a la compilación de código C# con código nativo . Por otro lado, la creación de aplicaciones con Xamarin , integrado con Visual Studio , cuenta con un sólido respaldo empresarial, aunque presenta una curva de aprendizaje más pronunciada y es posible que las aplicaciones no sean más pequeñas que las creadas con otros frameworks.

Características principales

Base de código única: tiene hasta el 90% del código compartido en iOS, Android y Windows.
Rendimiento nativo : permite el rendimiento nativo al compilar desde código C# a código nativo.
Integración : Se integra con Visual Studio muy fácilmente.
Ventajas

Rendimiento : Se logra un rendimiento similar al nativo mediante la compilación nativa.
Reutilización : Alta reutilización de código dentro de las plataformas.
Copia de seguridad empresarial : buena copia de seguridad y soporte de Microsoft.
Desventajas

Curva de aprendizaje pronunciada : requiere familiaridad con C# y .NET Framework, lo que puede ser un desafío para algunos desarrolladores.
Tamaño de la aplicación : marcos que dan lugar a tamaños de aplicaciones más grandes que los de otros marcos.

**PhoneGap**

Conocido como Apache Cordova , PhoneGap permite a los desarrolladores crear aplicaciones móviles utilizando tecnologías web comunes como HTML , CSS y JavaScript . Cuenta con una gran cantidad de complementos para acceder a las funciones nativas de los dispositivos. Además, permite la creación de aplicaciones para múltiples plataformas utilizando una única base de código. Si bien esta es una solución práctica para desarrolladores web, es posible que no tenga el mismo rendimiento que las aplicaciones nativas . Otros posibles problemas podrían ser la compatibilidad deficiente con algunos complementos .

Características principales

Complementos : gran biblioteca de complementos disponibles para obtener muchas funciones nativas en el dispositivo.
Multiplataforma : desarrolle una variedad de aplicaciones para todas las plataformas de sistema operativo utilizando una base de código compartida.
Comunidad : Gran comunidad y gran ecosistema de complementos.
Ventajas

Tecnologías web : utiliza tecnologías web estándar para su desarrollo.
Complementos : hay muchos complementos que funcionan con este software.
Flexibilidad : admite todas las plataformas y dispositivos críticos.
Desventajas

Rendimiento : No es tan potente como las aplicaciones nativas.
Mantenimiento : Algunos complementos no tienen un buen mantenimiento.

**NativeScript**

NativeScript permite desarrollar aplicaciones móviles nativas reales escritas en JavaScript , TypeScript o Angular , proporcionando acceso directo a las API nativas . Algunos argumentan que su rendimiento es casi tan alto como el del desarrollo nativo . NativeScript también permite crear aplicaciones Ionic visualmente atractivas gracias a sus componentes de interfaz de usuario nativos prediseñados para iOS y Android. Como desventaja, los desarrolladores intransigentes afirman que NativeScript presenta una curva de aprendizaje más pronunciada y, en última instancia, resulta en un mayor tamaño de la aplicación gracias a las bibliotecas nativas integradas.

Características principales

API nativas : acceso directo a API nativas desde JavaScript o TypeScript.
Multiplataforma : desarrolle e implemente aplicaciones para iOS y Android con una única base de código.
Componentes de UI : Componentes de UI nativos prediseñados y creados para iOS y Android.
Ventajas

Acceso directo a API nativas : consiga un rendimiento casi nativo.
Flexibilidad : además de soportar muchos lenguajes de desarrollo, como JavaScript y TypeScript.
Comunidad : Es una comunidad activa con buena documentación.
Desventajas

Curva de aprendizaje : más pronunciada que la de otros frameworks.
Tamaño de la aplicación : mayor tamaño de la aplicación porque las bibliotecas nativas están empaquetadas con ellas.

**Framework7**

Framework7 es un framework frontend para crear aplicaciones web móviles y de escritorio que se integran de forma nativa con tecnologías web estándar, como HTML, CSS y JavaScript. Ofrece una completa biblioteca de componentes de interfaz de usuario compatible con React, Vue o Svelte. Es fácil de usar para desarrolladores web, pero su rendimiento no destaca en aplicaciones totalmente nativas. Además, presenta ciertas complejidades al integrarse con otros frameworks.

Características principales

Componentes de UI : abundante biblioteca de componentes de UI prediseñados.
Compatibilidad : funciona con otros marcos como React, Vue y Svelte.
Aspecto y funcionamiento nativos : proporciona un aspecto y funcionamiento nativos para las aplicaciones.
Ventajas

Tecnologías web : utiliza HTML, CSS y JavaScript; por lo tanto, es amigable para los desarrolladores web.
Personalización : Componentes de interfaz de usuario muy personalizables.
Comunidad : Buen soporte comunitario, documentación detallada.
Desventajas

Rendimiento : Puede que no sea lo suficientemente potente como el de las aplicaciones nativas completas.
Curva de aprendizaje : La curva de aprendizaje puede volverse bastante rígida en los casos de integración entre marcos.

**Onsen UI**

Onsen UI es un paquete de componentes listos para implementar en tu aplicación móvil que usa HTML , CSS y JavaScript . Es totalmente compatible con Angular , React y Vue , optimiza el rendimiento con funciones como la carga diferida y es muy práctico para desarrolladores web . Sin embargo, sus desventajas incluyen la escasa documentación sobre su uso y que su comunidad no es tan grande como la de frameworks más grandes como React Native .

Características principales

Elementos de interfaz de usuario : gran colección prediseñada de elementos de interfaz de usuario.
Compatibilidad : funciona perfectamente con Angular, React y Vue.
Rendimiento : desarrollado para un rendimiento máximo con carga diferida y renderizado eficiente.
Ventajas

Tecnologías web : Las tecnologías web familiares hacen que el desarrollo web sea más sencillo.
Facilidad de integración : es fácil de integrar con marcos populares.
Personalización : Los elementos de la interfaz de usuario son altamente personalizables.
Desventajas

Documentación : Algunas partes de la documentación pueden ser insuficientes.
Comunidad : Comunidad pequeña en comparación con marcos más grandes, como React Native.

**Sencha Touch**

Sencha Touch es una plataforma JavaScript diseñada específicamente para la web móvil . Permite a los desarrolladores crear aplicaciones con HTML5 y JavaScript, de forma que se vean y se sientan nativas . Se basa en la arquitectura MVC y cuenta con numerosos componentes de interfaz de usuario para la entrada táctil. Esta aplicación tiene una curva de aprendizaje bastante pronunciada debido a sus funciones muy completas, pero requiere una licencia de alto costo.

Características principales

Componentes de UI : Amplio conjunto de componentes de UI optimizados para el tacto.
Alto rendimiento : utilización de aceleración de hardware y optimización de renderizado.
Arquitectura MVC : Arquitectura Modelo-Vista-Controlador incorporada para estructurar aplicaciones.
Ventajas

Rendimiento : Excelente rendimiento para aplicaciones móviles.
Aspecto y funcionamiento nativos : proporciona el aspecto y funcionamiento nativos para múltiples plataformas.
Funciones empresariales : contiene funciones para aplicaciones orientadas a la empresa.
Desventajas

Costo : La licencia puede ser costosa para equipos pequeños.
Curva de aprendizaje pronunciada : la aplicación alberga una gran cantidad de funciones, lo que la hace compleja.

**Appcelerator Titanium**

Appcelerator Titanium es una plataforma de desarrollo de código abierto que permite crear aplicaciones móviles con JavaScript , con la ayuda de API nativas como las proporcionadas por JavaScript. Admite desarrollo multiplataforma y ofrece un rendimiento prácticamente nativo para iOS , Android y Windows . Los desarrolladores pueden crear la interfaz de usuario utilizando una herramienta de diseño visual dentro de Titanium . Sin embargo, dado que Titanium requiere conocimientos de API nativas y funciones específicas de la plataforma, resulta muy difícil para los nuevos usuarios.

Características principales

Multiplataforma : cree para iOS, Android y Windows desde una única fuente.
API nativas : esto permite el acceso directo a las API nativas, lo que significa que los resultados de rendimiento son mejores.
Diseñador de aplicaciones : diseñadores de interfaces gráficas de usuario.
Ventajas

Rendimiento : Rendimiento casi nativo.
Integración : Se integra fácilmente con otras herramientas y servicios de desarrollo.
Comunidad : Cuenta con un fuerte respaldo comunitario y abundante documentación.
Desventajas

Curva de aprendizaje pronunciada : requiere comprensión de las API nativas y las características específicas de la plataforma.
Complejidad : Las funcionalidades avanzadas pueden volverse complejas.
