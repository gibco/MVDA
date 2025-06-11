# 📁 Guía para la Construcción y Publicación Accesible de una Tabla de Retención Documental (TRD)

## 🎯 Objetivo

Orientar a entidades públicas en la creación, validación y publicación de una **Tabla de Retención Documental (TRD)** accesible, partiendo de una hoja de cálculo Excel, cumpliendo con los principios de:

- Accesibilidad digital (WCAG 2.1)
- Resolución 1519 de 2020
- Ley 594 de 2000 (Ley General de Archivos)
- Buenas prácticas archivísticas colombianas

---

## 🧰 Requisitos Previos

- Normativa base:
  - Acuerdo AGN 001 de 2025
  - WCAG 2.1 nivel AA
  - Resolución 1519 de 2020
- Herramientas:
  - Microsoft Excel o LibreOffice Calc
  - Validador de PDF accesibles (PAC 2021 o Adobe Acrobat Pro)
  - Editor de Markdown (VS Code, Typora)
  - Validador de HTML o PDF (WAVE, axe, PDF Checker)

---

## ✅ Lista de Chequeo: Accesibilidad en Excel

| Criterio | ¿Cumple? (✔/✘) | Observación / Solución |
|---------|------------------|-------------------------|
| **Evitar celdas combinadas** | ✘ | No usar `Combinar celdas`. En su lugar, replicar valores o ajustar el diseño. |
| **Encabezados claros en primera fila** | ✔ | Usar negrilla y estilo de encabezado; no dejar vacías las celdas. |
| **No usar colores como único medio de distinción** | ✔ | Usar texto o símbolos además del color. Ej: "Pendiente 🔴", "Aprobado ✅". |
| **Contraste de color suficiente** | ✔ | Validar con herramientas como Colour Contrast Analyser. |
| **Orden lógico de lectura (izquierda a derecha, arriba abajo)** | ✔ | Evitar columnas ocultas o saltos de celdas. |
| **Título del documento visible en primera hoja** | ✔ | Incluir en una celda superior, por ejemplo: "Tabla de Retención Documental 2025". |
| **Descripción en hoja separada (Metadatos)** | ✔ | Incluir autor, fecha, versión, contacto, licencia. |
| **Texto alternativo en imágenes (si aplica)** | ✔ | Insertar texto alternativo desde "Formato de imagen > Texto alternativo". |
| **Evitar uso de tablas anidadas** | ✔ | Una sola tabla por hoja, claramente delimitada. |
| **Validación de ortografía** | ✔ | Revisar ortografía y gramática para lectores de pantalla. |

---

## 🪜 Paso a Paso para la Construcción

### 1. 📊 Diseña tu hoja de Excel

| Código | Serie documental | Subserie | Tipo documental | Tiempo gestión | Tiempo central | Disposición final | Soporte |
|--------|------------------|----------|------------------|----------------|----------------|--------------------|---------|

> 💡 Consejo: Asigna nombres a las hojas con significado: "TRD", "Metadatos", "Referencias".

---

### 2. 🧾 Exporta el Excel

- A HTML accesible: exporta desde Excel como `.html`, y edita etiquetas `<th>` y el atributo `lang="es"`.
- A PDF accesible: exporta como PDF/A y etiqueta con Acrobat Pro. Usa PAC 2021 para validar etiquetas y orden de lectura.

---

## 📤 Publicación en Web o GitHub

### Sitio institucional

```html
<a href="docs/TRD_2025.pdf" aria-label="Descargar TRD 2025 en PDF accesible">
  Tabla de Retención Documental 2025 (PDF Accesible)
</a>
