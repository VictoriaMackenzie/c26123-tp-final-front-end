# Lumina - Domótica e Hogares Inteligentes 🏠💡

Lumina es una plataforma de comercio electrónico dinámica enfocada en la automatización del hogar y soluciones de domótica. Este proyecto fue desarrollado como el Trabajo Práctico Final para el curso de Frontend con JavaScript de Talento Tech.

La aplicación permite explorar un catálogo de dispositivos inteligentes interactivos, gestionar un carrito de compras interactivo con persistencia local de datos y enviar consultas mediante un formulario de contacto integrado.

---

## 🚀 Características Principales

* **Catálogo Dinámico:** Renderizado de productos automatizado mediante el consumo de un archivo JSON interno mediante `fetch`.
* **Gestión Integral del Carrito:** Permite agregar productos, eliminar elementos específicos por índice y vaciar la totalidad del carrito de compras.
* **Persistencia de Datos (Web Storage):** Implementación de `LocalStorage` para retener los artículos seleccionados por el usuario aun si la pestaña o el navegador se cierran.
* **Diseño Adaptativo (Responsive Design):** Interfaz estilizada de forma nativa mediante CSS con Mobile-First y Media Queries optimizadas para pantallas de hasta 600px.
* **Formulario de Contacto Funcional:** Validación y envío de mensajes enlazado directamente a través del servicio externo de Formspree.

---

## 🛠️ Tecnologías y Recursos Utilizados

* **HTML5** - Estructura semántica de las vistas (Inicio, Carrito y Contacto).
* **CSS** - Estilos personalizados, Flexbox para la distribución de layouts y Media Queries adaptativas.
* **JavaScript** - Programación modular (`import`/`export`), manipulación dinámica del DOM, manejo de eventos y asincronía.
* **FontAwesome (v4.7)** - Librería externa de iconos vectoriales para mejorar la experiencia visual del carrito de compras.
* **Formspree API** - Procesamiento asincrónico del formulario de mensajes.

---

## 📂 Estructura del Proyecto

El repositorio se encuentra organizado bajo la siguiente arquitectura de directorios:

├── .vscode/
│   └── settings.json           # Configuración del puerto fijo para Live Server (5502)
├── css/
│   └── estilos.css             # Hoja de estilos central y reglas responsive
├── data/
│   └── productos.json          # Base de datos de productos en formato JSON (Cerraduras, sensores, etc.)
├── img/
│   └── ...                     # Repositorio local de recursos gráficos e imágenes
├── js/
│   ├── carrito.js              # Controlador específico para la vista del carrito
│   ├── contacto.js             # Controlador específico para la vista de contacto
│   ├── funcionesCarrito.js     # Lógica central del negocio (añadir, remover y vaciar)
│   ├── index.js                # Controlador principal de la Home y carga de productos
│   ├── storage.js              # Abstracción y serialización JSON del LocalStorage
│   └── ui.js                   # Módulo de utilidades gráficas (contador de badges y alertas)
├── pages/
│   ├── carrito.html            # Vista detallada de la orden de compras
│   └── contacto.html           # Vista del formulario de consultas
└── index.html                  # Punto de acceso principal y landing page del sitio