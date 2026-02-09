---
sidebar_position: 2
---

# NativeScript

### 1. Introducción al framework

NativeScript es un framework de código abierto para crear aplicaciones móviles multiplataforma para iOS y Android, creado en el año 2015 y mantenido por la empresa búlgara Telerik. Se puede utilizar HTML, JavaScript y CSS y puede integrarse de forma nativa con frameworks como Angular, React y Vue.Js. A diferencia de otros frameworks híbridos, NativeScript proporciona acceso directo a las APIs nativas del sistema operativo sin necesidad de WebViews, por lo tanto, traduce el código de la aplicación directamente a los componentes de la interfaz de usuario nativos de cada plataforma.

### 2. Cómo funciona, núcleo y características principales

![image.png](attachment:b3654a27-d1e1-437d-a1cf-d18fc7bc9c88:image.png)

NativeScript está basado en tiempo de ejecución (runtime). Este runtime permite que el código JavaScript se comunique directamente con las APIs nativas de iOS y Android.

Los módulos principales de NativeScript (NativeScript Core Modules) son una colección de bibliotecas que se utiliza para crear una aplicación e indicar al entorno de ejecución de NativeScript qué debe hacer la aplicación en un dispositivo. Los módulos principales constan de diferentes bibliotecas, como los componentes de la interfaz de usuario (botones, vistas de lista, etiquetas), la navegación y la aplicación.

Utiliza motores de ejecución JavaScript (V8 para Android y JavaScriptCore para iOS) para ejecutar código JS/TS directamente en el dispositivo. A través de una capa de reflexión y binding, mapea el código JavaScript a las clases y métodos nativos.

**Características principales:**

**Acceso directo a las APIs nativas:** Se puede invocar cualquier API nativa de iOS o Android directamente desde un código JavaScript, sin necesidad de plugins o wrappers predefinidos. Esto es una ventaja significativa sobre otros frameworks.

**Rendimiento nativo:** Al usar componentes de UI nativos y acceder directamente a las APIs, las aplicaciones NativeScript ofrecen un rendimiento y una fluidez comparables a las aplicaciones nativas.

**Código reutilizable:** Permite compartir gran parte del código base entre iOS y Android, reduciendo el tiempo y el costo de desarrollo.

**Soporte para frameworks populares:** Integración con Angular, Vue.js y React para el desarrollo de la interfaz de usuario.

**Hot Reload y LiveSync:** Herramientas que aceleran el ciclo de desarrollo al permitir ver los cambios en tiempo real en los dispositivos o emuladores.

### 3. Conjunto de tecnologías y lenguajes que entran en juego

**JavaScript (ESNext):** El lenguaje principal.

**TypeScript:** Recomendado por su tipado estático, lo que mejora la mantenibilidad y escalabilidad del código.

**XML/CSS:** Se utilizan para definir la interfaz de usuario y estilizarla, de manera similar a HTML/CSS en la web, pero mapeando a componentes de UI nativos.

**Frameworks de Frontend integrados:** Angular, React, Svelte y [Vue.Js](http://vue.js/) entre otros frameworks pueden ser integrados al desarrollo de una aplicación de NativeScript.

### 4. Herramientas, IDEs de desarrollo, componentes para crear aplicaciones

- NativeScript CLI, herramienta principal para crear, ejecutar y compilar proyectos).
- IDE’s tales como Visual Studio Code, WebStorm, Sublime Text, StackBlitz entre otros.
- Componentes UI nativos de NativeScript
- Emuladores y dispositivos reales para pruebas

### 5. Posibilidad de integración con tecnologías de frontend

Una de las grandes ventajas de NativeScript es su flexibilidad para integrarse con frameworks de frontend populares. Por lo tanto, Angular, Vue.js o React pueden integrarse en el desarrollo de aplicaciones móviles nativas.

- **NativeScript + Angular:** Estas aplicaciones siguen dependiendo de los módulos principales de NativeScript y del entorno de ejecución de NativeScript, pero permiten reemplazar la estructura de la aplicación, la definición de páginas, la navegación y el enlace de datos de NativeScript con las funcionalidades propias de Angular.
- **NativeScript + Vue.js:** Aprovecha la reactividad y la simplicidad de Vue.js para el desarrollo. Ejecuta el código JavaScript/Vue en un entorno de ejecución JavaScript integrado (usando V8, el motor que impulsa Node.js, los navegadores basados en Chromium, los workers de Cloudflare, entre otros) que expone enlaces a todas las API nativas automáticamente.
- **NativeScript + React:** Aunque menos maduro que las integraciones con Angular y Vue, ofrece una opción para desarrolladores React. Las interfaces de usuario de React NativeScript se componen de vistas nativas, al igual que las de NativeScript.

### 6. Compilado y construcción de binario para Android y iOS. Servicios de compilación en la nube

NativeScript CLI permite compilar localmente apps en formato APK (Android) e IPA (iOS). También se puede integrar con servicios de CI/CD como GitHub Actions o servicios de compilación en la nube como Appflow.

### 7. Acceso a recursos del sistema operativo

El framework expone las APIs del sistema operativo de forma directa, permitiendo acceso a cámara, sensores, GPS, almacenamiento, etc. a través de plugins o invocaciones directas en JS.

### 8. Qué tipo de aplicaciones admite crear

NativeScript permite desarrollar aplicaciones empresariales, aplicaciones de consumo tales como redes sociales o aplicaciones de e-commerce y aplicaciones que requieren acceso intensivo al hardware.

Se pueden desarrollar aplicaciones web, iOS, Android y Vision Pro con un código base compartido, es decir, aplicaciones multiplataforma.

Además se pueden desarrollar aplicaciones para AndroidTV, Watch y watchOS.

Permite la documentación de API’s de plataforma probando API’s directamente desde un navegador web sin requerir configuración de máquina de desarrollo de plataforma.

### 9. **Cuándo conviene utilizar este framework**

Para utilizar este framework es conveniente en el caso de tener un acceso nativo sin escribir con los lenguajes Java y Swift para Android e iOS respectivamente, reutilizar conocimientos en JavaScript, Angular, [Vue.js](http://vue.js/) entre otros frameworks y crear una app con rendimiento nativo sin WebViews. 

### 10. Aceptación en el mercado

Aunque no es tan popular como React Native o Flutter, NativeScript tiene una comunidad pequeña, sólida y en crecimiento, con contribuciones constantes en GitHub y una base de usuarios activa en foros y Stack Overflow.

### 11. Análisis del esquema jerárquico completo de un proyecto


**App:** Permite mostrar todo el código fuente de la aplicación.

**app.css**: El archivo app.css contiene estilos globales de la interfaz de usuario, que carga el entorno de ejecución de NativeScript al iniciar la aplicación.

**app.js/app.ts**: Archivo de entrada principal (JavaScript/TypeScript). Es el primer código que se ejecuta cuando se inicia una aplicación.

**main-page.js/main.page.ts y main-page.xml**: El archivo main-page.xml describe la interfaz de usuario de una página dentro de la aplicación, y main-page.js/main-page.ts (JavaScript/TypeScript) contiene la lógica de negocio correspondiente a la página. Juntas, estas dos páginas forman una unidad cohesiva, que representa una única página, llamada main-page.

**main-view-model.js**: Modelo-vista del proyecto.

**package.json**: Se utiliza para describir la aplicación en general y las dependencias necesarias para compilar y ejecutar.

**webpack.config.js**: Archivo de configuración de WebPack para building y optimización. El Webpack es un empaquetador de módulos, lo que significa que puede tomar varios módulos de JavaScript distribuidos en múltiples archivos y agruparlos (o empaquetarlos) en un único formato comprimido y optimizado.

**nativescript.config.js**: Archivo de configuración principal para el CLI de NativeScript.

### 12. Creación de aplicación de ejemplo simple

Se debe instalar el conjunto de herramientas (CLI) de NativeScript con el gestor de [Node.js](http://node.js/) (npm) para poder crear y ejecutar aplicaciones de NativeScript con el comando:

`npm install -g nativescript`

Para crear un proyecto con el template en blanco se debe ejecutar el comando:

```console

`ns create nombre-app --template @nativescript/template-blank`

`cd nombre-app`

`ns run android`

```
Para crear un proyecto con el template Maestro/Detalle se debe ejecutar el comando:

```console

`ns create nombre-app --template @nativescript/template-master-detail`

`cd nombre-app`

`ns run android`

```

### 13. Configuración necesaria para poder crear una primera aplicación simple

- Node.js y npm instalados.
- NativeScript CLI (npm i -g @nativescript/cli).
- JDK y Android SDK (para Android).
- Xcode para iOS ejecutando en macOS.

### 14. Descripción de comandos utilizados

```console

**ns create <nombre-app> [--template <template-name>]:** Crea un nuevo proyecto NativeScript con el nombre especificado y, opcionalmente, un template.

**ns run <platform> [--device <deviceId>]:** Compila e instala la aplicación en un emulador/simulador o dispositivo conectado.

- **<platform>** puede ser android o ios.
- **-device** es opcional para especificar un dispositivo particular.

**ns build <platform>:** Compila la aplicación para la plataforma especificada sin ejecutarla. Genera el archivo .apk o .ipa.

**ns platform add <platform>:** Agrega una plataforma a un proyecto existente (generalmente ya viene con ns create).

**ns platform remove <platform>:** Elimina una plataforma del proyecto.

**ns plugin add <plugin-name>:** Agrega un plugin al proyecto.

**ns doctor:** Verifica que el entorno de desarrollo esté correctamente configurado.

```

### **15. Ventajas y desventajas de NativeScript**

**Ventajas:**

- Tiene acceso directo a las API Nativas, lo cual permite mejorar el rendimiento.
- Flexibilidad para integrar a otros frameworks de frontend, tales como Angular, React y Vue.js.
- Es de código abierto.
- Requiere poca experiencia.

**Desventajas:**

- Requiere Configuración del entorno nativo, ya que se necesita implementar el SDK de Android y Xcode de iOS instalados y configurados.
- Presenta una comunidad más pequeña pero en crecimiento.
- Carece de soporte y documentación.

**NativeScript frente a React Native**

|  | NativeScript | React Native |
| --- | --- | --- |
| Lenguaje | JavaScript, Typescript | JavaScript |
| Arquitectura | Un solo subproceso | Multiproceso |
| Reutilización de código | Alto | Alto |
| Performance | Velocidad de las startups | UI más fluida |
| Popularidad | Menos popular | Más popular |
| Ajustes de performance | Acceso directo a las API Nativas | Acceso limitado a las API Nativas |
| Comunidad | Comunidad más pequeña pero en crecimiento | Grande y extensa |
| Flexibilidad | Alta | Moderada |
| Usos | Aplicaciones complejas que requieren integración nativa o aplicaciones empresariales | Aplicaciones dedicadas a la interfaz de usuario, en proyectos grandes con experiencia en desarrollo web existente |
| Curva de aprendizaje | Rápida | Simple |

### 16. Conclusiones

NativeScript es una opción sólida para equipos que priorizan el acceso completo a APIs nativas y la flexibilidad de frameworks, especialmente cuando se necesita aprovechar funcionalidades específicas de iOS/Android en comparación a otros frameworks multiplataformas.

### Bibliografia

**Bronstein M., Bronstein N. (2018). The NativeScript Book. The Brosteins.**

**NativeScript vs React Native for Native App Development in 2025.** https://www.bacancytechnology.com/blog/nativescript-vs-react-native

**What is NativeScript?** https://docs.nativescript.org/

**Qué es NativeScript?** https://www.esic.edu/rethink/tecnologia/nativescript-que-es-y-caracteristicas-c

**NativeScript-Vue** https://nativescript-vue.org/

**React NativeScript:** https://react-nativescript.netlify.app/