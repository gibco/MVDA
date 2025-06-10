# Checklist de Accesibilidad para Documentos de Oficina

Esta lista de verificación proporciona criterios específicos para crear documentos accesibles en Microsoft Office, LibreOffice y Google Workspace, organizados por tipo de documento y nivel de complejidad.

## 📋 Checklist General (Todos los Documentos)

### Estructura y Organización

- [ ] **Título del documento**: Claro, descriptivo y único
- [ ] **Idioma definido**: Configurado como español (Colombia) o español (España)
- [ ] **Metadatos completos**: Autor, título, descripción en propiedades del archivo
- [ ] **Estructura lógica**: Información organizada de general a específico
- [ ] **Numeración consistente**: Páginas, secciones y subsecciones numeradas

### Estilos y Formato

- [ ] **Estilos predefinidos**: Usar únicamente estilos de la aplicación
- [ ] **Jerarquía de encabezados**: H1 → H2 → H3, sin saltar niveles
- [ ] **Formato consistente**: Mismo estilo para elementos similares
- [ ] **Evitar formato manual**: No usar espacios, tabulaciones o enters para espaciado
- [ ] **Fuentes legibles**: Sans-serif para pantalla, serif para impresión

### Contraste y Color

- [ ] **Contraste mínimo**: 4.5:1 para texto normal, 3:1 para texto grande (18pt+)
- [ ] **No solo color**: Información transmitida por color + otro elemento (forma, texto)
- [ ] **Colores institucionales**: Verificar cumplimiento en paleta corporativa
- [ ] **Simulación daltonismo**: Verificar con herramientas de simulación

### Verificación Automática

- [ ] **Accessibility Checker**: Ejecutado sin errores críticos
- [ ] **Revisión ortográfica**: Sin errores de escritura
- [ ] **Hipervínculos válidos**: Todos los enlaces funcionan correctamente

## 📄 Microsoft Word - Documentos de Texto

### Configuración Inicial

```
☑ Archivo > Opciones > Avanzadas > General
☑ "Confirmar conversión de formato de archivo al abrir"
☑ Archivo > Opciones > Idioma > Idioma de edición: Español
```

### Estructura del Documento

- [ ] **Portada estructurada**:
  - [ ] Título principal (Estilo "Título")
  - [ ] Subtítulo (Estilo "Subtítulo") 
  - [ ] Autor/Entidad (Estilo "Normal")
  - [ ] Fecha (Estilo "Normal")

- [ ] **Tabla de contenido automática**:
  - [ ] Referencias > Tabla de contenido > Automática
  - [ ] Basada en estilos de encabezado
  - [ ] Actualizable automáticamente

- [ ] **Encabezados estructurados**:
  - [ ] H1: Solo título principal del documento
  - [ ] H2: Secciones principales
  - [ ] H3: Subsecciones
  - [ ] H4-H6: Niveles adicionales si es necesario

### Contenido Textual

- [ ] **Párrafos**:
  - [ ] Estilo "Normal" para texto corriente
  - [ ] Justificación izquierda (evitar justificado completo)
  - [ ] Interlineado mínimo 1.15
  - [ ] Espaciado después: 6pt mínimo

- [ ] **Listas**:
  - [ ] Usar herramientas de lista automática
  - [ ] Estilo "Lista" o "Lista numerada"
  - [ ] Niveles de anidación apropiados
  - [ ] Puntuación consistente

- [ ] **Énfasis y resaltado**:
  - [ ] **Negrita** para énfasis fuerte
  - [ ] *Cursiva* para énfasis leve o términos extranjeros
  - [ ] Evitar subrayado (reservado para enlaces)
  - [ ] No usar solo mayúsculas para énfasis

### Elementos Visuales

- [ ] **Imágenes y gráficos**:
  - [ ] Texto alternativo descriptivo (no "imagen1.jpg")
  - [ ] Descripción del contenido, no de la apariencia
  - [ ] Marcar como decorativo si corresponde
  - [ ] Resolución apropiada (300 DPI para impresión, 96 DPI para web)

- [ ] **Tablas simples**:
  - [ ] Primera fila como encabezado
  - [ ] "Repetir filas de encabezado" activado
  - [ ] Celdas combinadas mínimas
  - [ ] Texto alternativo descriptivo para tabla completa

- [ ] **Tablas complejas**:
  - [ ] Dividir en tablas más simples si es posible
  - [ ] Resumen de tabla en texto alternativo
  - [ ] Explicación adicional en párrafo siguiente

### Enlaces e Referencias

- [ ] **Hipervínculos**:
  - [ ] Texto descriptivo ("Descargar formulario de solicitud")
  - [ ] Evitar "clic aquí", "ver más", URLs desnudas
  - [ ] Información de herramientas descriptiva
  - [ ] Enlaces externos claramente marcados

- [ ] **Referencias cruzadas**:
  - [ ] Usar herramienta automática de referencias
  - [ ] Texto significativo ("ver Tabla 3" vs "ver abajo")
  - [ ] Actualizables automáticamente

### Configuración de Exportación

```markdown
Para PDF:
☑ Archivo > Exportar > Crear PDF/XPS
☑ Optimizar para: Tamaño mínimo (publicación en línea)  
☑ Crear marcadores usando: Títulos
☑ Propiedades del documento
☑ Etiquetas de estructura del documento para accesibilidad
```

## 📊 Microsoft Excel - Hojas de Cálculo

### Estructura de Datos

- [ ] **Organización de hoja**:
  - [ ] Una tabla de datos por hoja
  - [ ] Encabezados en primera fila
  - [ ] Datos homogéneos en cada columna
  - [ ] Sin filas o columnas vacías en medio de datos

- [ ] **Nombres de hojas**:
  - [ ] Descriptivos y únicos
  - [ ] Sin caracteres especiales
  - [ ] Máximo 31 caracteres
  - [ ] Orden lógico de izquierda a derecha

### Formato de Datos

- [ ] **Encabezados de tabla**:
  - [ ] Formato > Como tabla > Seleccionar estilo
  - [ ] "La tabla tiene encabezados" marcado
  - [ ] Texto descriptivo en cada encabezado
  - [ ] Sin espacios en blanco innecesarios

- [ ] **Celdas de datos**:
  - [ ] Formato consistente por columna
  - [ ] Números como números (no texto)
  - [ ] Fechas en formato de fecha
  - [ ] Texto alineado a la izquierda
  - [ ] Números alineados a la derecha

### Accesibilidad Visual

- [ ] **Colores y formato**:
  - [ ] Contraste adecuado para texto
  - [ ] Información no dependiente solo del color
  - [ ] Borde de celdas para separación visual
  - [ ] Formato condicional accesible

- [ ] **Gráficos**:
  - [ ] Título descriptivo
  - [ ] Etiquetas de ejes claras
  - [ ] Leyenda incluida
  - [ ] Texto alternativo completo
  - [ ] Datos originales accesibles

### Fórmulas y Funciones

- [ ] **Documentación**:
  - [ ] Comentarios en celdas con fórmulas complejas
  - [ ] Hoja separada con explicaciones si es necesario
  - [ ] Referencias claras y comprensibles

- [ ] **Validación de datos**:
  - [ ] Listas desplegables con opciones claras
  - [ ] Mensajes de error informativos
  - [ ] Ayuda emergente cuando corresponde

## 📽️ Microsoft PowerPoint - Presentaciones

### Diseño de Diapositivas

- [ ] **Plantilla accesible**:
  - [ ] Diseño > Tamaño de diapositiva > 16:9 o 4:3 estándar
  - [ ] Colores con contraste adecuado
  - [ ] Fuentes legibles (mínimo 24pt para texto)
  - [ ] Espaciado suficiente entre elementos

- [ ] **Estructura de contenido**:
  - [ ] Una idea principal por diapositiva
  - [ ] Máximo 6-8 líneas de texto
  - [ ] Jerarquía visual clara (título > subtítulo > contenido)
  - [ ] Numeración de diapositivas

### Contenido Textual

- [ ] **Títulos de diapositiva**:
  - [ ] Único y descriptivo por diapositiva
  - [ ] Usar marcador de posición de título
  - [ ] Tamaño mínimo 32pt
  - [ ] Alto contraste con fondo

- [ ] **Texto de contenido**:
  - [ ] Marcadores de posición apropiados
  - [ ] Viñetas para listas
  - [ ] Numeración para procesos secuenciales
  - [ ] Texto suficientemente grande (24pt mínimo)

### Elementos Multimedia

- [ ] **Imágenes**:
  - [ ] Texto alternativo descriptivo
  - [ ] Calidad apropiada para proyección
  - [ ] No pixeladas ni distorsionadas
  - [ ] Complementan el contenido, no lo reemplazan

- [ ] **Videos y audio**:
  - [ ] Subtítulos disponibles
  - [ ] Controles de reproducción accesibles
  - [ ] Transcripciones disponibles
  - [ ] Volumen apropiado y claro

### Navegación y Orden

- [ ] **Orden de lectura**:
  - [ ] Panel de selección para verificar orden
  - [ ] Secuencia lógica de elementos
  - [ ] Títulos antes que contenido
  - [ ] Imágenes en contexto apropiado

- [ ] **Transiciones y animaciones**:
  - [ ] Transiciones simples y consistentes
  - [ ] Animaciones con propósito educativo
  - [ ] No causan convulsiones (< 3 parpadeos/segundo)
  - [ ] Pausables o evitables

### Exportación Accesible

```markdown
Para PDF:
☑ Archivo > Exportar > Crear PDF/XPS
☑ Publicar como: Diapositivas
☑ Incluir marcadores de estructura
☑ Orden de las diapositivas
☑ Propiedades del documento
```

## 🌐 Google Workspace - Documentos en Línea

### Google Docs

- [ ] **Configuración inicial**:
  - [ ] Herramientas > Configuración del idioma > Español
  - [ ] Archivo > Configuración de página > Márgenes estándar
  - [ ] Ver > Mostrar regla para alineación visual

- [ ] **Estilos y formato**:
  - [ ] Usar estilos predefinidos (Título, Título 1, 2, 3...)
  - [ ] Formato > Estilos de párrafo > aplicar consistentemente
  - [ ] Evitar formato manual directo

- [ ] **Colaboración accesible**:
  - [ ] Comentarios descriptivos y constructivos
  - [ ] Sugerencias claras y específicas
  - [ ] Historial de versiones documentado

### Google Sheets

- [ ] **Datos estructurados**:
  - [ ] Formato > Formato como tabla
  - [ ] Fijar filas de encabezado
  - [ ] Datos > Validación de datos para listas

- [ ] **Gráficos accesibles**:
  - [ ] Insertar > Gráfico
  - [ ] Título y etiquetas descriptivas
  - [ ] Colores diferenciables
  - [ ] Datos fuente disponibles

### Google Slides

- [ ] **Temas accesibles**:
  - [ ] Diapositiva > Cambiar tema > colores de alto contraste
  - [ ] Verificar legibilidad en todos los diseños
  - [ ] Personalizar si es necesario

- [ ] **Presentación inclusiva**:
  - [ ] Texto grande y legible
  - [ ] Descripciones verbales de elementos visuales
  - [ ] Ritmo pausado para asimilación

## 🔧 LibreOffice - Suite Gratuita

### Writer (Documentos)

- [ ] **Configuración de accesibilidad**:
  - [ ] Herramientas > Opciones > Accesibilidad
  - [ ] "Permitir herramientas de accesibilidad" activado
  - [ ] Soporte para tecnologías de apoyo

- [ ] **Estilos LibreOffice**:
  - [ ] F11 para panel de estilos
  - [ ] Usar estilos de párrafo predefinidos
  - [ ] Crear estilos personalizados si es necesario

### Calc (Hojas de cálculo)

- [ ] **Navegación mejorada**:
  - [ ] Hoja > Nombrar celdas y rangos
  - [ ] Nombres descriptivos para rangos importantes
  - [ ] Comentarios en celdas complejas

### Impress (Presentaciones)

- [ ] **Exportación universal**:
  - [ ] Archivo > Exportar como PDF
  - [ ] Etiquetas PDF marcadas
  - [ ] Marcadores para navegación

## ⚡ Checklist Rápido por Tiempo

### 5 Minutos (Verificación Básica)

- [ ] Ejecutar Accessibility Checker
- [ ] Verificar contraste de colores principales
- [ ] Revisar texto alternativo de imágenes
- [ ] Confirmar estructura de encabezados
- [ ] Probar navegación con Tab

### 15 Minutos (Revisión Intermedia)

- [ ] Todo lo anterior +
- [ ] Verificar orden de lectura lógico
- [ ] Revisar hipervínculos descriptivos
- [ ] Validar tablas simples
- [ ] Comprobar metadatos del documento

### 30 Minutos (Auditoría Completa)

- [ ] Todo lo anterior +
- [ ] Probar con lector de pantalla
- [ ] Verificar en diferentes dispositivos
- [ ] Revisar formularios interactivos
- [ ] Documentar problemas encontrados
- [ ] Generar versión PDF accesible

## 📱 Consideraciones Móviles

### Diseño Responsive

- [ ] **Texto legible**:
  - [ ] Tamaño mínimo 16px en móviles
  - [ ] Contraste adecuado en pantallas pequeñas
  - [ ] Espaciado suficiente para touch

- [ ] **Navegación táctil**:
  - [ ] Elementos mínimo 44x44 pixeles
  - [ ] Espaciado entre elementos interactivos
  - [ ] Zoom permitido (no user-scalable=no)

### Compatibilidad Apps Móviles

- [ ] **Microsoft Office Mobile**:
  - [ ] Verificar apertura correcta
  - [ ] Funcionalidad básica mantenida
  - [ ] Sincronización con versión escritorio

- [ ] **Google Workspace Mobile**:
  - [ ] Edición colaborativa funcional
  - [ ] Comentarios y sugerencias accesibles
  - [ ] Compartir con permisos apropiados

## 🎯 Checklist por Audiencia

### Documentos para Ciudadanos

- [ ] **Lenguaje claro y sencillo**
- [ ] **Información de contacto visible**
- [ ] **Múltiples formatos disponibles** (PDF, HTML, texto)
- [ ] **Instrucciones paso a paso** para procesos
- [ ] **Glossario** para términos técnicos

### Documentos Internos/Técnicos

- [ ] **Estructura detallada** con numeración
- [ ] **Referencias cruzadas** automáticas
- [ ] **Índices y tablas** de contenido
- [ ] **Metadatos completos** para búsqueda
- [ ] **Control de versiones** documentado

### Materiales Educativos

- [ ] **Objetivos de aprendizaje** claros
- [ ] **Múltiples modalidades** (visual, auditivo, kinestésico)
- [ ] **Ejercicios y actividades** accesibles
- [ ] **Retroalimentación** clara y constructiva
- [ ] **Recursos adicionales** en formatos alternativos

### Documentos Legales/Normativos

- [ ] **Estructura jerárquica** clara (artículos, parágrafos, incisos)
- [ ] **Referencias normativas** precisas y verificables
- [ ] **Definiciones** de términos especializados
- [ ] **Tabla de contenido** detallada
- [ ] **Índice alfabético** para términos clave

## 🔄 Flujo de Trabajo Recomendado

### Fase 1: Planificación (Antes de crear)

```
□ Definir audiencia objetivo
□ Seleccionar plantilla accesible
□ Establecer estructura de contenido
□ Preparar recursos multimedia accesibles
□ Asignar responsabilidades de revisión
```

### Fase 2: Creación (Durante el desarrollo)

```
□ Usar estilos predefinidos desde el inicio
□ Agregar texto alternativo mientras se insertan imágenes
□ Configurar tablas con encabezados apropiados
□ Ejecutar Accessibility Checker periódicamente
□ Mantener estructura lógica consistente
```

### Fase 3: Revisión (Antes de publicar)

```
□ Auditoría completa de accesibilidad
□ Pruebas con tecnologías de apoyo
□ Revisión por segunda persona
□ Validación en diferentes dispositivos
□ Documentación de decisiones de accesibilidad
```

### Fase 4: Publicación (Al entregar)

```
□ Generar versiones en múltiples formatos
□ Incluir información de accesibilidad
□ Establecer canal de retroalimentación
□ Programar revisiones periódicas
□ Capacitar a usuarios si es necesario
```

## 🚨 Problemas Críticos a Evitar

### Errores que Rompen la Accesibilidad

**❌ NUNCA hacer:**

- [ ] ~~Usar imágenes de texto en lugar de texto real~~
- [ ] ~~Crear tablas con espacios y tabulaciones~~
- [ ] ~~Fusionar celdas innecesariamente en tablas~~
- [ ] ~~Usar solo color para transmitir información~~
- [ ] ~~Formatear manualmente con espacios/enters~~
- [ ] ~~Dejar imágenes sin texto alternativo~~
- [ ] ~~Usar "clic aquí" como texto de enlace~~
- [ ] ~~Crear encabezados con formato manual~~

### Señales de Alerta

**🚩 Revisar si encuentra:**

- Muchas advertencias en Accessibility Checker
- Texto que se ve como imagen al seleccionar
- Tablas que no se pueden navegar con teclado
- Elementos que desaparecen al quitar CSS/formato
- Contraste de colores que parece bajo
- Documentos que no se pueden leer linealmente

## 📊 Herramientas de Verificación por Plataforma

### Microsoft Office

**Accessibility Checker Integrado:**
```
Ubicación: Archivo > Información > Comprobar problemas > Comprobar accesibilidad
Ventajas: Integrado, tiempo real, específico por aplicación
Limitaciones: Solo detección automática
```

**Microsoft Accessibility Insights:**
- Herramienta externa para análisis profundo
- Disponible para Windows
- Integración con flujos de desarrollo

### Google Workspace

**Herramientas Nativas:**
```
Google Docs: Herramientas > Accesibilidad
Google Slides: Herramientas > Accesibilidad
Google Sheets: Verificación manual principalmente
```

**Extensiones Recomendadas:**
- WAVE Web Accessibility Evaluator
- axe DevTools (para documentos publicados en web)

### LibreOffice

**Verificación Manual:**
- Export a PDF y verificar con PAC 4
- Usar lector de pantalla (NVDA/Orca)
- Verificación visual de estructura

## 📚 Recursos de Capacitación

### Cursos en Línea

#### Microsoft Learn - Accessibility
- **URL**: https://docs.microsoft.com/learn/paths/accessibility-fundamentals/
- **Duración**: 2-4 horas
- **Nivel**: Principiante a intermedio
- **Certificación**: Gratuita

#### Google Applied Digital Skills
- **Enfoque**: Documentos accesibles en Google Workspace
- **Modalidad**: Videos interactivos
- **Idioma**: Disponible en español

### Documentación Oficial

#### Microsoft Accessibility Guide
- Guías específicas por aplicación
- Casos de uso detallados
- Actualizaciones regulares

#### Google Accessibility Documentation
- Mejores prácticas para G Suite
- Tutoriales paso a paso
- APIs de accesibilidad

### Webinars y Eventos

#### WebAIM Monthly Webinars
- Temas especializados en accesibilidad documental
- Casos de estudio reales
- Sesiones de Q&A

#### IAAP Local Chapters
- Eventos en español para Latinoamérica
- Networking con profesionales
- Certificaciones reconocidas

## 🏆 Certificación de Documentos Accesibles

### Proceso de Certificación Interna

**Nivel Básico (Documentos Simples):**
```
□ Accessibility Checker sin errores críticos
□ Verificación manual de estructura
□ Prueba básica con lector de pantalla
□ Aprobación de responsable de área
```

**Nivel Intermedio (Documentos Complejos):**
```
□ Todo lo anterior +
□ Auditoría con herramientas especializadas
□ Pruebas con múltiples tecnologías de apoyo
□ Revisión por experto en accesibilidad
□ Documentación de proceso de creación
```

**Nivel Avanzado (Documentos Críticos):**
```
□ Todo lo anterior +
□ Pruebas con usuarios reales con discapacidades
□ Certificación por terceros
□ Plan de mantenimiento y actualización
□ Capacitación específica para autores
```

### Sellos de Conformidad

**Información a incluir en documentos certificados:**
```
"Este documento cumple con las pautas de accesibilidad WCAG 2.1 AA 
y ha sido verificado el [fecha] por [responsable].
Para reportar problemas de accesibilidad: [contacto]"
```

## 🔮 Tendencias y Futuro

### Tecnologías Emergentes

**Inteligencia Artificial para Accesibilidad:**
- Generación automática de texto alternativo
- Detección inteligente de problemas de estructura
- Sugerencias de mejora en tiempo real
- Transcripción automática de contenido multimedia

**Realidad Aumentada/Virtual:**
- Documentos inmersivos accesibles
- Navegación espacial para personas ciegas
- Interpretación en lenguaje de señas integrada

### Evolución de Estándares

**WCAG 3.0 (EN desarrollo):**
- Nuevos criterios para documentos
- Métricas cuantitativas de accesibilidad
- Guías específicas para diferentes discapacidades

**PDF 2.0 y PDF/UA-2:**
- Mejor soporte para contenido multimedia
- Estructura semántica mejorada
- Integración con tecnologías web modernas

## 📞 Soporte y Comunidad

### Comunidades Hispanohablantes

**Accesibilidad Web Colombia:**
- Grupo de Facebook activo
- Eventos regulares y webinars
- Recursos en español

**Red Iberoamericana de Accesibilidad Web:**
- Colaboración entre países
- Compartir mejores prácticas
- Desarrollo de recursos regionles

### Listas de Correo Especializadas

**WebAIM Discussion List:**
- Discusiones técnicas avanzadas
- Respuestas de expertos reconocidos
- Archivo histórico de consultas

**IAAP Forums:**
- Subforos por especialidad
- Casos de estudio reales
- Networking profesional

## 📋 Plantillas de Documentación

### Reporte de Accesibilidad

```markdown
# Reporte de Accesibilidad - [Nombre del Documento]

**Fecha de evaluación:** [DD/MM/AAAA]
**Evaluador:** [Nombre y rol]
**Versión del documento:** [X.X]

## Resumen Ejecutivo
- Nivel de conformidad: [A/AA/AAA]
- Problemas críticos encontrados: [número]
- Tiempo estimado de corrección: [horas]

## Metodología
- [ ] Accessibility Checker automático
- [ ] Revisión manual con [herramienta]
- [ ] Pruebas con lector de pantalla [NVDA/JAWS/etc.]
- [ ] Verificación de contraste

## Problemas Encontrados
1. **[Categoría]:** [Descripción]
   - Ubicación: [página/sección]
   - Severidad: [Alta/Media/Baja]
   - Criterio WCAG: [X.X.X]
   - Solución recomendada: [pasos específicos]

## Recomendaciones
- Capacitación necesaria: [temas]
- Herramientas recomendadas: [lista]
- Revisión programada: [fecha]

## Aprobación
- [ ] Problemas críticos resueltos
- [ ] Verificación final completada
- [ ] Documento aprobado para publicación

**Firma del responsable:** ________________
**Fecha:** [DD/MM/AAAA]
```

### Log de Mejoras

```markdown
# Registro de Mejoras de Accesibilidad

| Fecha | Documento | Problema | Solución Aplicada | Responsable | Estado |
|-------|-----------|----------|-------------------|-------------|---------|
| DD/MM | Doc1.docx | Sin alt text | Agregado texto alternativo | Juan P. | ✅ |
| DD/MM | Report.pdf | Contraste bajo | Cambiado color de fondo | Ana G. | ✅ |
| DD/MM | Pres.pptx | Sin estructura | Aplicados estilos H1-H3 | Luis M. | 🔄 |
```

---

## 🎯 Resumen por Aplicación

### Microsoft Word - Puntos Clave
✅ **Esenciales:** Estilos, texto alternativo, estructura de encabezados, Accessibility Checker
⚠️ **Cuidado con:** Formato manual, tablas complejas, imágenes como texto
🎯 **Meta:** Documentos que se lean correctamente con tecnologías de apoyo

### Microsoft Excel - Puntos Clave  
✅ **Esenciales:** Encabezados de tabla, datos estructurados, gráficos con títulos
⚠️ **Cuidado con:** Celdas fusionadas, datos como texto, hojas sin nombres
🎯 **Meta:** Datos navegables y comprensibles para todos los usuarios

### Microsoft PowerPoint - Puntos Clave
✅ **Esenciales:** Títulos únicos, orden de lectura, texto alternativo, contraste
⚠️ **Cuidado con:** Animaciones excesivas, texto en imágenes, transiciones complejas
🎯 **Meta:** Presentaciones comprensibles sin apoyo visual

### Google Workspace - Puntos Clave
✅ **Esenciales:** Colaboración accesible, exportación correcta, estilos web-friendly
⚠️ **Cuidado con:** Dependencia de conexión, limitaciones de formato avanzado
🎯 **Meta:** Documentos accesibles en línea y offline

### LibreOffice - Puntos Clave
✅ **Esenciales:** Configuración de accesibilidad, exportación PDF etiquetado
⚠️ **Cuidado con:** Menos herramientas automáticas, verificación manual necesaria
🎯 **Meta:** Alternativa gratuita que mantenga estándares de accesibilidad

---

*¿Tienes preguntas específicas sobre alguna aplicación? ¡Consulta la documentación completa o contacta al equipo de accesibilidad!*