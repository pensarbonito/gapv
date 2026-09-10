# Workspace Dashboard

Un dashboard minimalist, ligero y autónomo para la gestión de tareas, seguimiento de proyectos y control de responsables en equipos de trabajo.

Diseñado para funcionar directamente en el navegador sin dependencias externas, bases de datos o servicios de backend.

---

## 🚀 Características Principales

* **Cero Configuración:** Basado 100% en tecnologías web nativas (HTML5, CSS3, JavaScript ES6+).
* **Persistencia Local:** Guarda todas las tareas automáticamente mediante `localStorage`. Los datos persisten al refrescar o cerrar la página.
* **Diseño Responsive:** Adaptado para una navegación fluida tanto en computadoras de escritorio como en dispositivos móviles.
* **Exportación / Importación CSV:** Permite realizar respaldos de seguridad locales e importar información desde archivos CSV.
* **Estructura Organizacional:**
  * **Categorías & Proyectos:** Filtro estructurado por áreas y proyectos predefinidos u opcionales.
  * **Gestión de Responsables:** Asignación visual por colores para miembros del equipo y la opción colectiva "Todo el equipo".
* **Filtros e Indicadores:** Estadísticas rápidas (Totales, Pendientes, Completadas) y vistas por categorías.

---

## 🛠️ Estructura del Repositorio

El repositorio mantiene una arquitectura ultra minimalista para facilitar su mantenimiento y despliegue:

```text
workspace-dashboard/
├── index.html       # Aplicación completa (Interfaz, estilos CSS y lógica JS)
├── LICENSE          # Licencia de código abierto (MIT)
└── README.md        # Documentación y guía de uso
```

---

## 💻 Instalación y Uso Local

No requiere la instalación de Node.js, servidores locales ni gestores de paquetes.

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/tu-usuario/workspace-dashboard.git
   ```
2. **Abrir la aplicación:**
   * Haz doble clic en el archivo `index.html` o ábrelo desde cualquier navegador web moderno (Chrome, Edge, Firefox, Safari).

---

## 🌐 Despliegue en GitHub Pages

Para publicar la aplicación en un enlace público accesible desde cualquier lugar:

1. Ve a tu repositorio en GitHub.
2. Ingresa a la sección **Settings** > **Pages** (en el menú lateral izquierdo).
3. En la sección **Build and deployment**:
   * **Source:** Selecciona `Deploy from a branch`.
   * **Branch:** Selecciona `main` (o `master`) y la carpeta `/ (root)`.
4. Haz clic en **Save**.
5. Espera un par de minutos y GitHub te proporcionará la URL de la aplicación pública (ejemplo: `https://tu-usuario.github.io/workspace-dashboard/`).

---

## 📊 Formato del Archivo CSV

El sistema permite exportar e importar datos para compartir información o restaurar copias de seguridad. El archivo CSV utiliza el siguiente formato:

| Campo | Descripción |
| :--- | :--- |
| **ID** | Identificador único secuencial (`TASK-001`, `TASK-002`) |
| **Tarea** | Nombre o descripción de la tarea |
| **Categoria** | Área o categoría a la que pertenece |
| **Proyecto** | Nombre del proyecto asignado |
| **Responsable** | Miembro del equipo o "Todo el equipo" |
| **Estado** | Estado de la tarea (`Pendiente` o `Completada`) |
| **Fecha Creacion** | Fecha en formato local (`DD/MM/YYYY`) |

---

## 🔒 Privacidad y Almacenamiento

* Los datos ingresados se guardan **únicamente en el navegador local** (`localStorage`) del dispositivo en uso.
* No se envían datos a servidores externos ni a GitHub.
* Si limpias la caché/historial del navegador, se borrarán los datos. Se recomienda usar la función **Exportar CSV** con frecuencia como método de respaldo.

---

## 📄 Licencia

Este proyecto se distribuye bajo la licencia **MIT**. Siéntete libre de modificarlo, adaptarlo y utilizarlo en tus propios proyectos.
