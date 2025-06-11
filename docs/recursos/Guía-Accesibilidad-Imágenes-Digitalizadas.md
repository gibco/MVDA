# 📘 Guía para la Accesibilidad de Imágenes Digitalizadas

Esta guía proporciona recomendaciones básicas para asegurar que las imágenes digitalizadas sean accesibles para todas las personas, incluyendo personas con discapacidad visual o cognitiva. Aplica a documentos escaneados, fotografías, infografías, gráficos o cualquier recurso visual digital.

---

## ✅ 1. ¿Por qué es importante?

- **Cumplimiento normativo**: Ley 1618 de 2013, Ley 1341 de 2009, y Resolución 1519 de 2020 (Colombia).
- **Inclusión digital**: Permite el acceso equitativo a la información.
- **Mejora de la usabilidad**: Facilita la comprensión del contenido visual para todos los usuarios.

---

## 🧩 2. Tipos de imágenes digitalizadas

| Tipo de imagen       | Ejemplo                         | Recomendación de accesibilidad              |
|----------------------|----------------------------------|---------------------------------------------|
| Documento escaneado  | Actas, cartas, resoluciones      | OCR + Texto alternativo descriptivo         |
| Gráfico o infografía | Estadísticas, mapas, diagramas   | Descripción larga o tabla equivalente       |
| Fotografía            | Eventos, personas, objetos       | Texto alternativo con contexto funcional    |

---

## 📝 3. Texto alternativo (`alt`)

El texto alternativo describe el contenido y la función de la imagen.

```html
<img src="resolucion_2020.png" alt="Portada escaneada de la Resolución 1519 de 2020 del MinTIC, firmada digitalmente">
```

> 💡 *Debe ser claro, breve, y funcional. Evita frases como "imagen de..." o "foto que muestra..."*

---

## 🔍 4. OCR (Reconocimiento Óptico de Caracteres)

**¿Qué es?** Técnica para convertir imágenes escaneadas en texto legible por máquinas.

- ✅ Usa herramientas como Adobe Acrobat Pro, ABBYY FineReader o Tesseract.
- ✅ Verifica que el texto sea seleccionable, buscable y legible por lectores de pantalla.

```bash
# Ejemplo con Tesseract en terminal
tesseract imagen_escaneada.png salida_texto -l spa
```

---

## 📐 5. Contraste y calidad de imagen

- Usa imágenes con alto contraste y buena resolución.
- Evita imágenes borrosas, sobreexpuestas o con sombras.
- Si la imagen es de un documento, asegúrate de que esté bien alineada y sin dobleces visibles.

---

## 🧰 6. Recursos recomendados

- [WCAG 2.1 - Directrices de Accesibilidad](https://www.w3.org/WAI/WCAG21/es/)
- [Herramienta de validación Tingtun PDF/UA](https://pdf-accessibility.org/)
- [Resolución 1519 de 2020 - Gobierno Digital (Colombia)](https://www.funcionpublica.gov.co/documents/418537/0/Resoluci%C3%B3n+1519+de+2020.pdf)

---

## 🛠️ 7. Buenas prácticas

- ✅ Usa nombres de archivo descriptivos: `acta_asamblea_2024_ocr.pdf`
- ✅ Añade metadatos: título, autor, fecha de escaneo
- ✅ Informa si el documento ha sido validado por OCR y por quién
- ✅ Acompaña las imágenes con un resumen accesible en texto

---

## 📣 Licencia y reutilización

Este documento puede ser adaptado y reutilizado bajo la licencia [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

---

> 🧭 Elaborado para promover el acceso equitativo a la información pública digital en Colombia. Si encuentras barreras de accesibilidad, ¡repórtalas y sé parte del cambio!
