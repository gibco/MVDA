# 📁 Guía para la Construcción y Publicación Accesible de una Tabla de Retención Documental (TRD)

## 🎯 Objetivo

Orientar a entidades públicas en la creación, validación y publicación de una **Tabla de Retención Documental (TRD)** accesible, utilizando como base una hoja de cálculo Excel, con énfasis en el cumplimiento de las WCAG 2.1, la Resolución 1519 de 2020 y las buenas prácticas archivísticas en Colombia.

---

## 🧰 Requisitos Previos

- 🧩 **Normativa base**:
  - Ley 594 de 2000 (Ley General de Archivos)
  - Acuerdo AGN 001 de 2025
  - Resolución 1519 de 2020 (Gobierno Digital)
  - WCAG 2.1 nivel AA
- 🛠️ **Herramientas**:
  - Microsoft Excel o LibreOffice Calc
  - Exportador a HTML o PDF/A
  - Editor Markdown (Visual Studio Code, Typora, etc.)
  - Validador de accesibilidad (WAVE, axe, PDF Accessibility Checker)

---

## 🪜 Paso a Paso para la Construcción y Publicación Accesible

### 1. 📊 Diseña la hoja de cálculo base (Excel)

Crea una hoja con los siguientes encabezados, usando estilos de celda para facilitar la navegación por lector de pantalla:

| Código | Serie documental | Subserie | Tipo documental | Tiempo gestión | Tiempo central | Disposición final | Soporte |
|--------|------------------|----------|------------------|----------------|----------------|--------------------|---------|

> 💡 Usa encabezados claros y evita fusionar celdas.

---

### 2. ✅ Asegura accesibilidad en la hoja de cálculo

- Usa **texto plano** (sin imágenes incrustadas).
- Habilita etiquetas de encabezado en la **primera fila**.
- No uses **colores como único medio de diferenciación**.
- Añade una **hoja de metadatos** con información del documento:
  - Fecha de elaboración
  - Responsable
  - Estado de aprobación
  - Licencia de uso (p. ej. CC BY 4.0)

---

### 3. 🧾 Exporta la hoja de cálculo

Elige uno de estos formatos accesibles:

#### Opción A: HTML Accesible

1. Guarda como `.html`.
2. Abre el archivo y valida que:
   - La tabla tenga `<th scope="col">` y `<th scope="row">`.
   - El idioma esté declarado: `<html lang="es">`.

#### Opción B: PDF accesible

1. Guarda como PDF/A.
2. Usa herramienta como **Adobe Acrobat Pro** o **PAC 2021** para:
   - Verificar que los encabezados están etiquetados (`<TH>`).
   - Añadir etiquetas a la tabla si es necesario.
   - Establecer el idioma del documento a "es-CO".
   - Incluir texto alternativo si hay logotipos.

---

### 4. 📤 Publicación en la web

#### 🔹 Si usas sitio institucional

- Asegura que el PDF esté etiquetado correctamente.
- Usa un texto descriptivo para el enlace, por ejemplo:
  ```html
  <a href="ruta/TRD2025.pdf" aria-label="Descargar Tabla de Retención Documental 2025 en PDF accesible">
    Tabla de Retención Documental 2025 (PDF)
  </a>
