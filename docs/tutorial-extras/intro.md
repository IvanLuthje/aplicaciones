---
sidebar_position: 4
---

# Introducción a Aplicaciones Nativas

- Desarrolladas en un lenguaje y entorno de desarrollo específico
- Ejecutadas en un dispositivo y sistema operativo determinado.
- El código fuente de estas aplicaciones se escribe en función del dispositivo.
- Este código fuente se compila a un ejecutable. Es un proceso similar al de las tradicionales aplicaciones de escritorio. 
- Cuando la aplicación está lista para ser distribuida, es subida a las App stores (tiendas de aplicaciones) específicas de cada dispositivo. 
-	App Stores llevan a cabo un proceso de auditoría para evaluar si se adecúa a los requerimientos y a las políticas del market

## Ventajas

- Aplicación integrada al dispositivo pudiendo interactuar con otras apps del dispositivo
- Acceso total a las utilidades del dispositivo
- Capacidad de utilizar toda la pantalla del dispositivo y proporcionar una mejor UI
- Puede ejecutarse offline
- La aplicación puede correr en segundo plano y notificar cuando la info esté disponible
- Aplicaciones más rápidas que un sitio web movil
- Notificaciones

## Desventajas

- Desarrollo más costoso que un sitio web movil
- Las apps no están disponibles para ser instaladas en todos los dispositivos móviles
- La actualización de la app es mucho más compleja
- Cada plataforma tiene su propio entorno de desarrollo y lenguaje de programación
- Fragmentación del mercado: Desarrollar para una plataforma puede significar quedar afuera de un alto % del mercado
- Fragmentación interna. Por ejemplo: Android tiene un gran % del mercado pero actualmente existen varias versiones en uso
- Para que los usuarios puedan utilizar una aplicación primero debe descargarla e instalarla, lo que requiere un mayor conocimiento y lealtad a la marca

## Plataformas

- Android
- iOS
- Windows Phone (obsoleto)
- Blackberry OS (obsoleto)
- Symbian (obsoleto)

## Fragmentación interna y externa

**Fragmentación Externa** se desarrollan aplicaciones nativas para diferentes plataformas o sistemas operativos, tales como iOS y Android.
Cuando una marca (ej. Samsung o Xiaomi) tiene tantos modelos que no puede actualizar todos a la misma velocidad.

**Fragmentación Interna** la aplicación se comporta o se presenta en diferentes versiones o en distintos dispositivos dentro de esa misma plataforma.
La brecha entre los usuarios que tienen Android 14 y los que siguen estancados en Android 10, lo que complica el trabajo a los desarrolladores de apps.

Desarrollar una app para la última versión lanzada de una plataforma es la solución más adecuada, debido a que mejora cuestiones de seguridad y compatibilidad en el futuro.



<!-- # Manage Docs Versions

Docusaurus can manage multiple versions of your docs.

## Create a docs version

Release a version 1.0 of your project:

```bash
npm run docusaurus docs:version 1.0
```

The `docs` folder is copied into `versioned_docs/version-1.0` and `versions.json` is created.

Your docs now have 2 versions:

- `1.0` at `http://localhost:3000/docs/` for the version 1.0 docs
- `current` at `http://localhost:3000/docs/next/` for the **upcoming, unreleased docs**

## Add a Version Dropdown

To navigate seamlessly across versions, add a version dropdown.

Modify the `docusaurus.config.js` file:

```js title="docusaurus.config.js"
export default {
  themeConfig: {
    navbar: {
      items: [
        // highlight-start
        {
          type: 'docsVersionDropdown',
        },
        // highlight-end
      ],
    },
  },
};
```

The docs version dropdown appears in your navbar:

![Docs Version Dropdown](./img/docsVersionDropdown.png)

## Update an existing version

It is possible to edit versioned docs in their respective folder:

- `versioned_docs/version-1.0/hello.md` updates `http://localhost:3000/docs/hello`
- `docs/hello.md` updates `http://localhost:3000/docs/next/hello`
 -->