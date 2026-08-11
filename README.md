# OpenSource / MateLogic

**Software abierto. Ideas compartidas.**

Directorio de proyectos open source creados por [MateLogic](https://github.com/Mate-Logic). Un espacio simple y elegante para descubrir las herramientas, librerías y utilidades que construimos en público.

## ✨ Características

- **Directorio de proyectos** con tarjetas para cada repo publicado.
- **Búsqueda instantánea** por nombre de proyecto (atajo con la tecla `/`).
- **Filtros por categoría**: Web, Herramientas, CLI y Librerías.
- **Tema oscuro** inspirado en la estética de OpenCode: superficies apagadas y grises cálidos.
- **Diseño responsive** y accesible, con etiquetas ARIA y navegación por teclado.

## 🚀 Empezando

### Requisitos

- [Node.js](https://nodejs.org/) `>= 22.12.0`
- `pnpm` ([instalación](https://pnpm.io/installation))

### Instalación

```sh
pnpm install
```

### Desarrollo

```sh
pnpm dev
```

El servidor de desarrollo se ejecuta en `http://localhost:4321`.

### Producción

```sh
pnpm build      # genera el sitio en ./dist/
pnpm preview    # previsualiza la build localmente
```

## 📦 Comandos

| Comando          | Acción                                            |
| :--------------- | :------------------------------------------------ |
| `pnpm install`   | Instala las dependencias                          |
| `pnpm dev`       | Inicia el servidor de desarrollo en `localhost:4321` |
| `pnpm build`     | Genera el sitio de producción en `./dist/`        |
| `pnpm preview`   | Previsualiza la build localmente                  |
| `pnpm astro ...` | Ejecuta comandos de la CLI de Astro               |

## 🗂️ Estructura del proyecto

```text
/
├── public/               # Assets estáticos (favicon, etc.)
└── src/
    └── pages/
        └── index.astro   # Página principal con el directorio
```

## ➕ Añadir un proyecto

Para publicar un nuevo proyecto, agrega un objeto al arreglo `projects` en [`src/pages/index.astro`](src/pages/index.astro):

```js
{
  name: 'Mi Proyecto',
  slug: 'mi-proyecto',
  description: 'Una breve descripción del proyecto.',
  category: 'Web',        // Web | Herramientas | CLI | Librerías
  language: 'Astro',
  status: 'En desarrollo',
  href: 'https://github.com/Mate-Logic/mi-proyecto',
  featured: true,
},
```

## 🧑‍🤝‍🧑 Contribuciones

¿Tienes una idea, encontraste un bug o quieres proponer un proyecto? Abre un *issue* o un *pull request*. Este es un espacio para construir en abierto: todas las contribuciones son bienvenidas.

## 📄 Licencia

Este proyecto está disponible como software de código abierto. Consulta la licencia de cada proyecto dentro del directorio para más detalles.

---

Hecho con curiosidad y código abierto.
