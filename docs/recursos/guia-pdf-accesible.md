# Guía para Crear PDFs Accesibles

Esta guía proporciona instrucciones detalladas para crear documentos PDF que cumplan con el estándar PDF/UA-1 (ISO 14289-1:2014) y sean accesibles para personas que utilizan tecnologías de apoyo.

## 🎯 Fundamentos del PDF Accesible

### ¿Qué es PDF/UA?

**PDF/UA (Universal Accessibility)** es un estándar ISO que define los requisitos técnicos para documentos PDF accesibles. Un PDF/UA garantiza que:

- El contenido sea perceptible por lectores de pantalla
- La navegación sea predecible y eficiente
- La estructura del documento sea comprensible
- Las interacciones sean operables con teclado

### Principios Básicos

1. **Estructura semántica**: El PDF debe tener etiquetas estructurales
2. **Orden de lectura lógico**: El contenido debe seguir una secuencia comprensible
3. **Texto alternativo**: Todas las imágenes deben tener descripciones
4. **Contraste adecuado**: Cumplir WCAG 2.1 nivel AA
5. **Navegación por teclado**: Todos los elementos interactivos deben ser accesibles

## 🛠️ Creación desde Documentos Fuente

### Desde Microsoft Word

#### Preparación del Documento Word

**1. Usar Estilos Predefinidos**
```
✓ Usar "Título 1", "Título 2", etc. para encabezados
✓ Aplicar "Normal" para texto corriente
✓ Usar "Lista" para elementos de lista
✗ NO formatear manualmente con negrita/tamaño
```

**2. Estructura de Encabezados**
```
Título 1: Título principal del documento
├── Título 2: Sección principal
│   ├── Título 3: Subsección
│   └── Título 3: Otra subsección
└── Título 2: Otra sección principal
```

**3. Texto Alternativo para Imágenes**
```
Clic derecho en imagen > Editar texto alternativo
- Descripción concisa pero informativa
- Evitar "imagen de..." o "foto de..."
- Si es decorativa, marcar como tal
```

**4. Tablas Accesibles**
```
✓ Definir fila de encabezados
✓ Usar "Repetir filas de encabezado"
✓ Evitar celdas combinadas complejas
✓ Proporcionar resumen si es compleja
```

**5. Enlaces Descriptivos**
```
✓ "Descargar formulario de solicitud"
✗ "Haga clic aquí"
✗ "Ver más"
```

#### Configuración de Exportación a PDF

**Archivo > Exportar > Crear PDF/XPS**

```
Configuración recomendada:
☑ Optimizar para: Tamaño mínimo (publicación en línea)
☑ Crear marcadores usando: Títulos
☑ Propiedades del documento
☑ Etiquetas de estructura del documento para accesibilidad
☑ Mapas de bits del texto cuando las fuentes no se pueden incrustar
```

### Desde Adobe InDesign

#### Configuración de Exportación

**Archivo > Exportar > Adobe PDF (Interactivo)**

```
Configuración de accesibilidad:
☑ Usar estructura para orden de tabulación
☑ PDF etiquetado
☑ Crear marcadores
☑ Incluir información de la estructura
☑ Exportar en orden de artículos del panel
```

**Panel Artículos**: Definir orden de lectura correcto antes de exportar

### Desde LibreOffice Writer

```
Archivo > Exportar en PDF
☑ PDF etiquetado (crear estructura PDF a partir de la estructura del documento)
☑ Exportar marcadores
☑ Crear formulario PDF
☑ Incrustar fuentes estándar
```

## 🔧 Optimización en Adobe Acrobat Pro

### Asistente "Hacer Accesible"

**Herramientas > Accesibilidad > Hacer accesible**

El asistente guía través de:
1. Reconocimiento de texto (si es necesario)
2. Detección de idioma del documento
3. Configuración de opciones de lectura
4. Estructura de etiquetas
5. Configuración de orden de tabulación

### Verificación de Estructura

#### Panel de Etiquetas (Tags)
```
Ver > Mostrar/Ocultar > Paneles de navegación > Etiquetas

Estructura típica:
Document
├── Part (opcional)
│   ├── H1 (Encabezado nivel 1)
│   ├── P (Párrafo)
│   ├── Figure (Imagen)
│   ├── Table
│   │   ├── TR (Fila de tabla)
│   │   │   ├── TH (Celda de encabezado)
│   │   │   └── TD (Celda de datos)
```

#### Corrección de Etiquetas Comunes

**Problema: Texto sin etiquetar**
```
Solución:
1. Seleccionar texto en el panel Contenido
2. Clic derecho > Crear etiqueta a partir de la selección
3. Elegir tipo de etiqueta apropiado (P, H1, etc.)
```

**Problema: Imágenes sin texto alternativo**
```
Solución:
1. Seleccionar etiqueta Figure
2. Propiedades > Etiqueta > Texto alternativo
3. Escribir descripción concisa
```

**Problema: Orden de lectura incorrecto**
```
Solución:
1. Herramientas > Accesibilidad > Orden de lectura
2. Reorganizar elementos arrastrando
3. Definir artefactos para elementos decorativos
```

### Panel de Comprobación de Accesibilidad

**Herramientas > Accesibilidad > Comprobación completa**

```
Configuración recomendada:
☑ Crear informe de accesibilidad
☑ Todas las reglas del estándar PDF/UA
☑ Comentarios en páginas donde se detecten problemas
☑ Crear informe de problemas en panel de navegación
```

### Configuración de Propiedades del Documento

**Archivo > Propiedades**

```
Descripción:
- Título: Título descriptivo del documento
- Autor: Nombre del autor o entidad
- Asunto: Breve descripción del contenido
- Palabras clave: Términos relevantes

Avanzadas:
☑ Idioma: Español (es-ES) o (es-CO)
☑ Enlace inicial: Primera página
☑ Diseño de página: Página única
```

## 📋 Lista de Verificación PDF/UA

### Estructura y Navegación

- [ ] Documento tiene estructura de etiquetas completa
- [ ] Orden de lectura es lógico y secuencial
- [ ] Encabezados están correctamente jerarquizados (H1-H6)
- [ ] Existe navegación por marcadores para documentos largos
- [ ] El idioma del documento está definido
- [ ] Los cambios de idioma están marcados

### Contenido Visual

- [ ] Todas las imágenes informativas tienen texto alternativo
- [ ] Imágenes decorativas están marcadas como artefactos
- [ ] Gráficos complejos tienen descripciones detalladas
- [ ] El contraste de colores cumple WCAG 2.1 AA (4.5:1 mínimo)
- [ ] La información no depende únicamente del color

### Tablas

- [ ] Tablas tienen encabezados definidos (TH)
- [ ] Estructura de tabla es simple y lógica
- [ ] Tablas complejas tienen resumen o descripción
- [ ] Celdas de datos están asociadas con encabezados correspondientes

### Formularios

- [ ] Todos los campos tienen etiquetas descriptivas
- [ ] Campos requeridos están claramente marcados
- [ ] Instrucciones de llenado son claras
- [ ] Mensajes de error son específicos y útiles
- [ ] Orden de tabulación es lógico

### Enlaces y Navegación

- [ ] Texto de enlaces es descriptivo
- [ ] Enlaces se pueden distinguir del texto normal
- [ ] URLs largas tienen texto descriptivo
- [ ] Enlaces externos se identifican claramente

### Configuración Técnica

- [ ] Fuentes están incrustadas
- [ ] No hay restricciones de accesibilidad en seguridad
- [ ] Metadatos del documento están completos
- [ ] Pasa verificación completa de PDF/UA

## 🔍 Herramientas de Verificación

### Adobe Acrobat Pro DC

**Comprobación Completa de Accesibilidad**
- Ubicación: Herramientas > Accesibilidad > Comprobación completa
- Resultado: Reporte detallado con problemas específicos
- Acción: Corregir cada elemento reportado

### PAC 4 (PDF Accessibility Checker)

**Descarga**: https://www.access-for-all.ch/en/pdf-lab/pdf-accessibility-checker-pac.html

```
Características:
✓ Verificación PDF/UA completa
✓ Vista previa de lector de pantalla
✓ Análisis de estructura lógica
✓ Gratuito y confiable
```

### CommonLook PDF Validator

**Tipo**: Herramienta comercial especializada
**Ventajas**: Verificación más exhaustiva, reparación guiada
**Uso**: Para documentos críticos o volúmenes grandes

## 🎭 Casos Especiales

### Documentos con Formularios

#### Campos de Formulario Accesibles

```xml
Estructura recomendada:
<Form>
  <P>
    <Label>Nombre completo:</Label>
    <Form role="textbox" />
  </P>
  <P>
    <Label>Correo electrónico:</Label>
    <Form role="textbox" />
  </P>
</Form>
```

**Configuración en Acrobat:**
1. Herramientas > Preparar formulario
2. Para cada campo: Propiedades > General > Información de herramientas
3. Configurar orden de tabulación: Ver > Mostrar/Ocultar > Reglas > Orden de tabulación

### Documentos con Gráficos Complejos

#### Descripción Detallada

**Para gráficos estadísticos:**
```
Método 1: Texto alternativo extendido
"Gráfico de barras que muestra ventas trimestrales 2023. 
Q1: $125,000; Q2: $150,000; Q3: $175,000; Q4: $200,000. 
Tendencia ascendente del 60% anual."

Método 2: Tabla de datos complementaria
Incluir tabla con datos exactos después del gráfico
```

#### Mapas e Infografías

```
Requerimientos:
- Descripción general del propósito
- Información clave en formato texto
- Tabla de datos si es aplicable
- Instrucciones alternativas para procesos
```

### Documentos Multiidioma

```xml
Estructura con cambios de idioma:
<Document lang="es-ES">
  <P>Texto en español</P>
  <P lang="en-US">Text in English</P>
  <P>Continúa en español</P>
</Document>
```

**Configuración en Acrobat:**
1. Seleccionar texto en idioma extranjero
2. Propiedades > Etiqueta > Idioma
3. Definir código de idioma apropiado

## ⚡ Automatización y Flujos de Trabajo

### Scripts de Acrobat

#### Script para Verificación Masiva

```javascript
// Ejemplo básico de script para verificar múltiples PDFs
function verificarAccesibilidad() {
    var reporte = this.accessibility.checkerReports;
    if (reporte.length > 0) {
        console.println("Problemas encontrados: " + reporte.length);
    }
}
```

### Plantillas Accesibles

#### Crear Plantilla Reutilizable

```
1. Crear documento Word con:
   - Estilos predefinidos
   - Estructura de encabezados
   - Página de portada estándar
   - Pie de página con información de accesibilidad

2. Guardar como plantilla (.dotx)

3. Configurar exportación PDF predeterminada

4. Documentar proceso para el equipo
```

### Control de Calidad

#### Checklist para Publicación

```
Antes de publicar:
□ Ejecutar comprobación completa en Acrobat Pro
□ Verificar con PAC 4
□ Probar navegación con teclado (Tab, flechas)
□ Revisar con lector de pantalla (NVDA/JAWS)
□ Validar en diferentes dispositivos
□ Confirmar cumplimiento de política institucional
□ Documentar fecha y responsable de verificación
```

#### Protocolo de Revisión por Pares

```
Revisor 1: Verificación técnica automática
Revisor 2: Evaluación manual de usabilidad  
Revisor 3: Pruebas con tecnologías de apoyo
Aprobación final: Responsable de accesibilidad
```

## 🚫 Errores Comunes y Cómo Evitarlos

### Errores en Creación del Documento Fuente

**❌ Error: Usar espacios para crear indentación**
```
Problema: "    Este texto tiene espacios al inicio"
✅ Solución: Usar estilos de párrafo con sangría definida
```

**❌ Error: Usar Enter múltiples para espacio vertical**
```
Problema: 
Título

[múltiples enters]

Contenido

✅ Solución: Configurar espaciado antes/después en estilos
```

**❌ Error: Crear tablas falsas con tabulaciones**
```
Problema: Columna 1    Columna 2    Columna 3
✅ Solución: Usar tabla real con encabezados definidos
```

### Errores en Exportación PDF

**❌ Error: No activar etiquetas estructurales**
```
Resultado: PDF sin estructura, inaccesible para lectores de pantalla
✅ Solución: Siempre activar "Etiquetas de estructura"
```

**❌ Error: Exportar como imagen**
```
Problema: Escanear documento o "Imprimir a PDF"
✅ Solución: Usar "Exportar como PDF" desde aplicación original
```

### Errores en Optimización

**❌ Error: Dejar imágenes sin texto alternativo**
```
Síntoma: "<Figure>" sin descripción en lector de pantalla
✅ Solución: Agregar texto alternativo a todas las imágenes informativas
```

**❌ Error: Orden de lectura incorrecto**
```
Problema: Lector lee columnas verticalmente en lugar de horizontalmente
✅ Solución: Usar herramienta "Orden de lectura" para reorganizar
```

## 📱 Consideraciones para Dispositivos Móviles

### Diseño Responsive en PDF

#### Configuración para Móviles

```
Configuración de página:
- Tamaño: A4 o Letter (evitar tamaños personalizados)
- Márgenes: Mínimo 2.5 cm para permitir zoom
- Fuente: Mínimo 12 puntos (14 puntos recomendado)
- Interlineado: 1.5 mínimo
```

#### Navegación Touch-Friendly

```
Enlaces y botones:
- Tamaño mínimo: 44x44 pixeles
- Espaciado entre elementos: 8 pixeles mínimo
- Texto de enlaces descriptivo y suficientemente largo
- Evitar enlaces muy cercanos entre sí
```

### Optimización para Lectores de Pantalla Móviles

**TalkBack (Android) y VoiceOver (iOS)**

```
Consideraciones especiales:
- Navegación por gestos específicos
- Lectura de metadatos más detallada
- Mejor soporte para tablas simples
- Integración con zoom del sistema
```

## 🎓 Recursos de Capacitación

### Cursos en Línea

#### WebAIM PDF Accessibility
- **URL**: https://webaim.org/training/pdf/
- **Nivel**: Intermedio
- **Duración**: 2-3 horas
- **Certificación**: Disponible

#### Adobe Accessibility Training
- **URL**: https://www.adobe.com/accessibility/training.html
- **Recursos**: Videos, tutoriales, documentación
- **Idioma**: Inglés (algunos recursos en español)

### Documentación Oficial

#### ISO 14289-1:2014
- **Descripción**: Estándar técnico completo PDF/UA-1
- **Acceso**: Compra a través de ISO
- **Alternativa**: Resumen gratuito en sitio web PDF Association

#### Matterhorn Protocol
- **URL**: https://www.pdfa.org/matterhorn-protocol/
- **Descripción**: Lista de verificación detallada PDF/UA
- **Formato**: PDF accesible (ironía intencional)
- **Idioma**: Inglés, con traducciones parciales

### Comunidades y Foros

#### PDF Association
- **URL**: https://www.pdfa.org/
- **Recursos**: Webinars, documentación técnica, foros
- **Enfoque**: Estándares PDF y accesibilidad

#### CommonLook Community
- **Foros**: Discusiones técnicas sobre PDF accesible
- **Recursos**: Casos de estudio, mejores prácticas
- **Soporte**: Gratuito para usuarios registrados

## 🔗 Integración con Sistemas Web

### Publicación en Sitios Web

#### Configuración de Servidor

```html
<!-- Headers HTTP recomendados -->
Content-Type: application/pdf
Content-Disposition: inline; filename="documento-accesible.pdf"
Cache-Control: public, max-age=3600

<!-- Meta información en HTML -->
<a href="documento.pdf" 
   type="application/pdf"
   title="Informe anual 2023 (PDF, 2.5 MB)">
   Descargar informe anual 2023
</a>
```

#### Alternativas y Complementos

```html
<!-- Página de descarga con información -->
<div class="documento-descarga">
  <h2>Informe Anual 2023</h2>
  <p>Documento en formato PDF accesible (PDF/UA)</p>
  
  <ul>
    <li><a href="informe-2023.pdf">Descargar PDF (2.5 MB)</a></li>
    <li><a href="informe-2023.html">Versión HTML</a></li>
    <li><a href="informe-2023.txt">Versión texto plano</a></li>
  </ul>
  
  <details>
    <summary>Información de accesibilidad</summary>
    <p>Este documento cumple con el estándar PDF/UA-1 y WCAG 2.1 AA.</p>
    <p>Si experimenta dificultades, contacte: accesibilidad@entidad.gov.co</p>
  </details>
</div>
```

### Metadatos para SEO y Accesibilidad

```xml
<!-- Metadatos XMP en PDF -->
<xmp:CreateDate>2024-03-15T10:30:00-05:00</xmp:CreateDate>
<xmp:ModifyDate>2024-03-15T10:30:00-05:00</xmp:ModifyDate>
<xmp:MetadataDate>2024-03-15T10:30:00-05:00</xmp:MetadataDate>
<dc:title>Informe Anual de Gestión 2023</dc:title>
<dc:description>Reporte completo de actividades y resultados</dc:description>
<dc:subject>gestión pública, transparencia, resultados</dc:subject>
<dc:language>es-ES</dc:language>
<pdf:PDFVersion>1.7</pdf:PDFVersion>
<pdfuaid:part>1</pdfuaid:part>
```

## 📊 Métricas y Monitoreo

### KPIs de Calidad

#### Métricas Técnicas

```
- Tiempo promedio de verificación por documento
- Porcentaje de documentos que pasan PDF/UA al primer intento
- Número de problemas promedio por documento
- Tiempo de corrección de problemas identificados
```

#### Métricas de Usuario

```
- Descargas de documentos PDF vs versiones alternativas
- Reportes de problemas de accesibilidad por usuarios
- Satisfacción de usuarios con tecnologías de apoyo
- Tiempo de localización de información en documentos
```

### Herramientas de Monitoreo

#### Automated PDF Testing

```javascript
// Ejemplo con Pa11y para verificación masiva
const pa11y = require('pa11y');

async function verificarPDFs(urls) {
  for (const url of urls) {
    try {
      const results = await pa11y(url, {
        standard: 'WCAG2AA',
        timeout: 30000
      });
      console.log(`${url}: ${results.issues.length} problemas`);
    } catch (error) {
      console.error(`Error verificando ${url}:`, error.message);
    }
  }
}
```

## 🆘 Resolución de Problemas Comunes

### Problemas de Estructura

**Síntoma**: Lector de pantalla no reconoce encabezados
```
Diagnóstico: 
1. Abrir panel de Etiquetas en Acrobat
2. Verificar presencia de H1, H2, etc.
3. Comprobar jerarquía correcta

Solución:
1. Herramientas > Accesibilidad > Agregar etiquetas al documento
2. Reetiquetado manual si es necesario
3. Verificar orden de lectura
```

**Síntoma**: Orden de lectura incorrecto en columnas
```
Diagnóstico:
1. Herramientas > Accesibilidad > Orden de lectura
2. Verificar secuencia visual

Solución:
1. Reorganizar elementos arrastrando
2. Crear regiones de lectura apropiadas
3. Verificar con lector de pantalla
```

### Problemas de Contenido

**Síntoma**: Imágenes leídas como "imagen sin descripción"
```
Diagnóstico:
1. Verificar presencia de texto alternativo
2. Comprobar etiquetas Figure en panel de Etiquetas

Solución:
1. Seleccionar etiqueta Figure
2. Propiedades > Etiqueta > Texto alternativo
3. Escribir descripción apropiada
```

**Síntoma**: Tabla leída incorrectamente
```
Diagnóstico:
1. Verificar estructura TH/TD en etiquetas
2. Comprobar asociación de encabezados

Solución:
1. Herramientas > Accesibilidad > Configurar asistencia tabla
2. Definir encabezados de fila y columna
3. Simplificar estructura si es muy compleja
```

### Problemas de Formularios

**Síntoma**: Campos de formulario no accesibles
```
Diagnóstico:
1. Verificar etiquetas de campos
2. Comprobar orden de tabulación

Solución:
1. Propiedades de campo > General > Información de herramientas
2. Configurar orden de tabulación lógico
3. Agrupar campos relacionados
```

## 📞 Soporte y Recursos Adicionales

### Contactos de Soporte Técnico

#### Adobe Support
- **Accesibilidad**: Casos específicos de Acrobat Pro
- **Documentación**: Guías oficiales actualizadas
- **Foros**: Comunidad de usuarios y expertos

#### Organizaciones Especializadas

**IAAP (International Association of Accessibility Professionals)**
- Certificaciones en accesibilidad
- Red de profesionales
- Recursos de formación continua

**Fundación ONCE (España)**
- Investigación en accesibilidad
- Herramientas y metodologías
- Asesoría especializada

### Servicios de Consultoría

#### Cuándo Solicitar Ayuda Externa

```
Considerar consultoría cuando:
- Volumen de documentos muy alto (>1000 PDFs)
- Documentos técnicos complejos (manuales científicos)
- Documentos legacy sin fuente original
- Implementación de flujos automatizados
- Capacitación intensiva del equipo
- Auditorías de cumplimiento formal
```

---

## 🏁 Resumen Ejecutivo

### Proceso Recomendado (30 minutos por documento)

```
1. [5 min] Preparar documento fuente con estilos correctos
2. [2 min] Exportar con configuración de accesibilidad
3. [10 min] Optimizar en Acrobat Pro (estructura, alt text)
4. [5 min] Ejecutar verificación automática completa
5. [5 min] Probar con lector de pantalla
6. [3 min] Documentar y publicar
```

### ROI de Accesibilidad PDF

```
Beneficios:
+ Cumplimiento normativo (evitar sanciones)
+ Mejor posicionamiento SEO
+ Mayor alcance de audiencia (15% población)
+ Reducción de consultas de soporte
+ Mejora de imagen institucional

Costos:
- Tiempo inicial de implementación
- Capacitación del personal
- Herramientas especializadas (Acrobat Pro)
- Posible consultoría externa
```

### Próximos Pasos

1. **Evaluar documentos actuales** con PAC 4
2. **Capacitar al equipo** en creación accesible
3. **Establecer flujo de trabajo** estándar
4. **Implementar verificación** en proceso de publicación
5. **Monitorear y mejorar** continuamente

---

*¿Tienes preguntas específicas sobre PDF accesible? ¡Abre un issue en el repositorio y te ayudaremos!*