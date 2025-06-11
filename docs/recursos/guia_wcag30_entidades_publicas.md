# 🛡️ Guía Técnica para la Implementación de Accesibilidad Web (WCAG 3.0) en Entidades Públicas

> 📌 Esta guía no es una opción. Es una hoja de ruta obligatoria para asegurar el acceso igualitario a los servicios digitales del Estado colombiano.

---

## 🎯 Propósito

Garantizar que **todos los ciudadanos**, sin importar su condición, puedan acceder a la información y servicios digitales. Incumplir no solo implica sanciones normativas, sino una grave afectación a los principios de equidad, inclusión y transparencia pública.

---

## 1. 📚 Fundamentos Normativos

- **Internacionales**: WCAG 3.0 (Working Draft - W3C)
- **Nacionales**:
  - Ley 1618 de 2013
  - Resolución 1519 de 2020 (Gobierno Digital)
  - Ley 1341 de 2009 (TIC)
  - CONPES 3975 de 2019

---

## 2. 🧩 Componentes Críticos a Intervenir

| Componente Digital           | Fallos comunes detectados                                   | Correcciones obligatorias |
|-----------------------------|-------------------------------------------------------------|----------------------------|
| Sitios web institucionales  | Sin etiquetas `alt`, navegación rota, sin contraste         | WCAG: A y AA obligatorio   |
| Documentos digitales (.PDF) | Imágenes escaneadas sin OCR, sin estructura, sin etiquetas  | PDF/UA mínimo              |
| Formularios y trámites      | Campos sin `label`, sin validación accesible                | ARIA roles, foco visible   |
| Multimedia                  | Videos sin subtítulos, sin audio descripción                | Subtítulos, transcripciones|

---

## 3. 🧪 Auditoría Técnica Obligatoria

Realizar pruebas automatizadas y manuales con herramientas como:

- [axe-core](https://www.deque.com/axe/)
- [Lighthouse](https://developer.chrome.com/docs/lighthouse/)
- [Pa11y](https://pa11y.org/)
- [AChecker](https://achecker.achecks.ca/)

📌 *Resultado mínimo esperado*: ≥ 90% de cumplimiento con nivel A y AA.

---

## 4. 🛠️ Implementación Técnica por Principio

| Principio WCAG 3.0 | Requisito técnico mínimo                                |
|--------------------|----------------------------------------------------------|
| Perceptible         | `alt`, contrastes WCAG (≥ 4.5:1), encabezados semánticos |
| Operable            | Navegación por teclado, foco visible, tiempo suficiente |
| Comprensible        | Lenguaje claro (`lang="es"`), formularios etiquetados  |
| Robusto             | Código válido, roles ARIA apropiados, compatible con AT |

---

## 5. 👥 Pruebas con usuarios con discapacidad

**No es accesibilidad si no se prueba con usuarios reales.**  
Pruebas funcionales con tecnologías de asistencia:

- NVDA / JAWS (lectores de pantalla)
- VoiceOver (iOS/macOS)
- Navegación con solo teclado

---

## 6. 📄 Declaración Técnica de Accesibilidad

Requiere:
- Versión del estándar usado (WCAG 3.0)
- Herramientas de auditoría utilizadas
- Áreas conformes y pendientes
- Mecanismo de reporte ciudadano (correo, formulario accesible)

📌 *Modelo sugerido:* VPAT adaptado al contexto colombiano.

---

## 7. 📈 Indicadores de Accesibilidad (mínimo semestrales)

- % de cumplimiento (por tipo de contenido)
- Nº de barreras corregidas
- Nº de contenidos accesibles (PDF, sitios, trámites)
- Nº de incidentes reportados / atendidos

---

## 8. 🧠 Capacitación Técnica Continua

Todo equipo TIC y de comunicaciones debe tener formación básica en:

- Principios WCAG 3.0
- Accesibilidad en diseño UI/UX
- PDF accesible y documentos ofimáticos accesibles

Recomendado: mínimo 1 servidor certificado IAAP por entidad.

---

## 🔐 Riesgos de no cumplimiento

- Sanciones disciplinarias (Ley 734)
- Reclamaciones ante la Procuraduría
- Incumplimiento en evaluación FURAG
- Vulneración del derecho de acceso a la información pública

---

## ✅ Licencia

Esta guía puede ser utilizada y adaptada libremente bajo licencia [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/), citando la fuente.

> ⚠️ *No hay transformación digital sin accesibilidad digital. La inclusión no es un anexo: es el principio rector de todo gobierno digital.*
