# 🚀 UIS Asignaturas — Ingeniería de Sistemas

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Online-2563eb?logo=github)](https://hecfrantuis.github.io/UIS_Asignaturas/)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/es/docs/Web/HTML)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/es/docs/Web/JavaScript)
[![License](https://img.shields.io/badge/license-MIT-green)](#-licencia)

Panel web dinámico que organiza y expone los contenidos, talleres, plantillas y herramientas interactivas de las asignaturas de **Ingeniería de Sistemas de la Universidad Industrial de Santander (UIS)**.

Todo se genera automáticamente desde la estructura de carpetas del repositorio usando la **API de GitHub**, por lo que **no hay que tocar el HTML cada vez que se agrega un nuevo recurso**. Basta con subir el archivo a la carpeta correcta y aparecerá en el panel.

🔗 **Sitio en vivo:** <https://hecfrantuis.github.io/UIS_Asignaturas/>

---

## 📖 Tabla de contenidos

- [Características](#-características)
- [Estructura del repositorio](#-estructura-del-repositorio)
- [Cómo agregar contenido](#-cómo-agregar-contenido)
- [Cómo funciona el panel](#-cómo-funciona-el-panel)
- [Ejecución local](#-ejecución-local)
- [Despliegue en GitHub Pages](#-despliegue-en-github-pages)
- [Contribuir](#-contribuir)
- [Tecnologías](#-tecnologías)
- [Licencia](#-licencia)
- [Autor](#-autor)

---

## ✨ Características

- 📂 **Navegación por materias**: primero se listan las carpetas (materias), y al entrar se muestran los recursos `.html` de cada una.
- 🔁 **Generación automática**: el índice se construye dinámicamente desde la API de GitHub. No hay que editar HTML.
- 🌐 **Routing con hash**: URLs compartibles tipo `#/Asignaturas/Simulacion_Digital`. El botón "atrás" del navegador funciona.
- 📱 **100% responsive**: se adapta a móvil, tablet y escritorio.
- ⚡ **Caché en `sessionStorage`**: reduce el consumo de la API de GitHub (60 peticiones/hora sin token).
- 🧭 **Breadcrumb y botón "Volver"** para navegar jerárquicamente.
- ♿ **Accesibilidad**: navegación por teclado en las tarjetas (Enter / Espacio).
- 🎨 **Diseño limpio** con variables CSS, fácil de personalizar.

---

## 📁 Estructura del repositorio

```text
UIS_Asignaturas/
├── index.html                  # Panel principal (entrada de GitHub Pages)
├── README.md
└── Asignaturas/                # Cada subcarpeta = una materia
    └── Simulacion_Digital/
        ├── Metodo_Congruencial_Mixto.html
        ├── Metodo_Congruencial_ShumShumBlum.html
        ├── Metodo_Productos_Medios.html
        ├── metodo_congruencial_aditivo.html
        ├── metodo_congruencial_multiplicativo.html
        ├── metodo_cuadrados_medios.html
        └── metodo_producto_constante.html
