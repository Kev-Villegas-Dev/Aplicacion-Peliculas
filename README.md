# Aplicación-Peliculas - Kevin Villegas Rendón -
## Descripción General de la Aplicación

**peliculasApp** es una aplicación móvil multiplataforma desarrollada con **Ionic Framework** y **Angular** que permite a los usuarios explorar información detallada sobre películas.

La aplicación consume la **API de The Movie Database (TMDb)** para ofrecer las siguientes funcionalidades principales:

* **Cartelera Actual:** Muestra un listado de películas que están actualmente en estreno (`getFeature`).
* **Películas Populares:** Navegación por un listado infinito de las películas más populares (`getPopulares`).
* **Detalle de Película:** Vista detallada de cualquier película, incluyendo sinopsis, géneros y el elenco de actores (`getActoresPelicula`).
* **Búsqueda:** Permite buscar películas por título (`buscarPeliculas`).
* **Favoritos:** Utiliza el almacenamiento local para guardar y gestionar una lista de películas favoritas (Deducido por la dependencia `@ionic/storage-angular`).

---

## Tecnologías y Dependencias Utilizadas

El proyecto fue inicializado como una aplicación **Angular** con el tipo de proyecto **Ionic**.

### Stack Principal
* **Framework Móvil:** [Ionic Framework](https://ionicframework.com/)
* **Framework Frontend:** [Angular](https://angular.io/) (Versión `^16.2.9`)
* **Lenguaje:** TypeScript (Versión `~4.8.4`)
* **API de Datos:** The Movie Database (TMDb)
* **Contenedor Nativo:** Capacitor (Versión `7.2.0`)

### Dependencias Destacadas
| Dependencia | Versión | Propósito |
| :--- | :--- | :--- |
| `@ionic/angular` | `^6.2.4` | Componentes y utilidades de Ionic. |
| `@angular/core` | `^16.2.9` | Núcleo de Angular. |
| `@angular/common` | `^16.2.9` | Módulos comunes, incluyendo el cliente HTTP para consumir la API. |
| `@ionic/storage-angular` | `^4.0.0` | Gestión de almacenamiento de datos local (para favoritos). |
| `rxjs` | `~7.5.7` | Programación reactiva. |

---

## Instrucciones para la Instalación y Ejecución Local

Para ejecutar este proyecto en tu entorno local, sigue los siguientes pasos.

### 1. Prerrequisitos

Asegúrate de tener instalado:
* **Node.js** y **npm** (o yarn).
* La Interfaz de Línea de Comandos de Ionic (**Ionic CLI**):
    ```bash
    npm install -g @ionic/cli
    ```

### 2. Configuración del Proyecto

1.  **Clonar el repositorio Aplicacion-Peliculas - Kev-Villegas-Dev :**
    ```bash
    # Ingresa el comando en tu CMD o consola de git
    git clone [URL_DEL_REPOSITORIO-APLICACION-PELICULLAS/KEV-VILLEGAS-DEV]
    cd aplicacion-peliculas
    ```
2.  **Instalar las dependencias de Node:**
    ```bash
    npm install
    ```
3.  **Verificar la configuración de la API Key:**
    La aplicación utiliza la API de TMDb. El proyecto ya incluye la configuración en el archivo de entorno:
    * `src/environments/environment.ts`
    
    ```typescript
    export const environment = {
      production: false,
      url: '[https://api.themoviedb.org/3](https://api.themoviedb.org/3)',
      apiKey: 'MI API KEY', // AQUI SALDRA LA TUYA o LA QUE ESTA USANDO EL DOCUMENTO ¡Recuerda que no compartas tu API Key personal!
      imgPath: '[https://image.tmdb.org/t/p](https://image.tmdb.org/t/p)'
    };
    ```

### 3. Ejecución en Navegador

Para ejecutar la aplicación en el navegador web en modo de desarrollo:
```bash
ionic serve
```

### Créditos y Agradecimientos
Este proyecto fue posible gracias a las siguientes fuentes de documentación y material educativo:

Documentación de Angular (v16): Por la referencia oficial del framework.

https://angular.dev/overview

Ionic Documentation: Por la base del framework y su documentación oficial.

https://ionicframework.com/docs/

Fernando Herrera: Agradecimiento por el curso y el material educativo sobre Ionic y Angular que sirvió como guía para el desarrollo de esta aplicación.
