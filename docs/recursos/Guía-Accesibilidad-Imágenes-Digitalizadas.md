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
