# Herramientas de Evaluación de Accesibilidad

Esta guía proporciona un catálogo de herramientas para evaluar la accesibilidad de sitios web y documentos electrónicos, organizadas por tipo y nivel de expertise requerido.

## 🌐 Herramientas para Sitios Web

### Herramientas Oficiales Colombianas

#### Verificador de Accesibilidad de Colombia (MinTIC)
- **URL**: https://accesibilidad.mintic.gov.co/verificador/
- **Tipo**: Automático, gratuito
- **Descripción**: Herramienta oficial del MinTIC basada en WCAG 2.1
- **Ventajas**: 
  - Alineado con normativa colombiana
  - Reportes detallados en español
  - Seguimiento de múltiples URLs
- **Limitaciones**: Solo evaluación automática
- **Casos de uso**: Evaluación inicial, monitoreo continuo

### Herramientas Automáticas Internacionales

#### WAVE Web Accessibility Evaluator
- **URL**: https://wave.webaim.org/
- **Desarrollador**: WebAIM
- **Tipo**: Gratuito, extensión de navegador disponible
- **Características**:
  - Visualización in-situ de problemas
  - Iconografía intuitiva para errores
  - Análisis de contraste
  - Verificación de estructura semántica
- **Ideal para**: Desarrolladores y diseñadores

#### axe DevTools
- **URL**: https://www.deque.com/axe/devtools/
- **Desarrollador**: Deque Systems
- **Tipo**: Extensión de navegador, versión pro disponible
- **Características**:
  - Integración con herramientas de desarrollo
  - API para pruebas automatizadas
  - Guías de reparación específicas
  - Bajo índice de falsos positivos
- **Ideal para**: Desarrolladores, equipos de QA

#### Lighthouse Accessibility Audit
- **URL**: Integrado en Chrome DevTools
- **Desarrollador**: Google
- **Tipo**: Gratuito, integrado
- **Características**:
  - Puntuación de accesibilidad 0-100
  - Métricas de rendimiento relacionadas
  - Sugerencias de mejora priorizadas
  - Integración con CI/CD
- **Ideal para**: Auditorías rápidas, monitoreo continuo

### Herramientas Especializadas

#### ANDI (Accessible Name & Description Inspector)
- **URL**: https://www.ssa.gov/accessibility/andi/
- **Desarrollador**: Social Security Administration (USA)
- **Tipo**: Gratuito, bookmarklet
- **Características**:
  - Inspección detallada de nombres accesibles
  - Simulación de lectores de pantalla
  - Análisis de orden de tabulación
  - Verificación de estructura de encabezados
- **Ideal para**: Evaluación manual detallada

#### Colour Contrast Analyser
- **URL**: https://www.tpgi.com/color-contrast-checker/
- **Desarrollador**: TPGi
- **Tipo**: Gratuito, aplicación de escritorio
- **Características**:
  - Verificación precisa de contraste
  - Simulación de tipos de daltonismo
  - Herramienta de pipeta para selección de colores
  - Cumplimiento WCAG AA y AAA
- **Ideal para**: Diseñadores, verificación de paletas

#### Pa11y
- **URL**: https://pa11y.org/
- **Tipo**: Open source, línea de comandos
- **Características**:
  - Automatización en CI/CD
  - Pruebas masivas de sitios
  - Múltiples formatos de salida
  - Integración con Node.js
- **Ideal para**: Desarrolladores, DevOps

### Herramientas de Evaluación Manual

#### Tecnologías de Apoyo para Pruebas

**Lectores de Pantalla:**
- **NVDA** (Windows): https://www.nvaccess.org/ - Gratuito
- **JAWS** (Windows): https://www.freedomscientific.com/ - Comercial
- **VoiceOver** (macOS/iOS): Integrado en sistema
- **TalkBack** (Android): Integrado en sistema
- **Orca** (Linux): Pre-instalado en la mayoría de distribuciones

**Navegación por Teclado:**
- Pruebas manuales usando solo teclado
- Verificación de orden de tabulación lógico
- Comprobación de trampas de teclado
- Validación de atajos de teclado

**Software de Magnificación:**
- **ZoomText** (Windows): https://www.freedomscientific.com/
- **MAGic** (Windows): https://www.freedomscientific.com/
- **Zoom** (macOS): Integrado en sistema

## 📄 Herramientas para Documentos Electrónicos

### Microsoft Office

#### Microsoft Accessibility Checker
- **Ubicación**: Integrado en Word, Excel, PowerPoint
- **Acceso**: Archivo > Información > Revisar documento > Comprobar accesibilidad
- **Características**:
  - Detección automática de problemas comunes
  - Sugerencias de reparación paso a paso
  - Verificación en tiempo real (opcional)
  - Exportación de reportes
- **Limitaciones**: Solo problemas automáticamente detectables

#### Guía de uso para Office:
```
1. Crear documento con estilos predefinidos
2. Ejecutar Accessibility Checker regularmente
3. Agregar texto alternativo a imágenes
4. Verificar orden de lectura
5. Usar verificador de contraste
6. Probar con lector de pantalla
```

### Adobe PDF

#### Adobe Acrobat Pro DC
- **Características de accesibilidad**:
  - Accessibility Checker completo
  - Herramienta de etiquetado automático
  - Panel de orden de lectura
  - Verificación de PDF/UA
  - Reparación de estructura de etiquetas

#### Procesos recomendados:
```
1. Crear PDF desde fuente accesible (Word, InDesign)
2. Ejecutar Make Accessible Action Wizard
3. Revisar estructura de etiquetas
4. Verificar orden de lectura
5. Validar con lector de pantalla
6. Confirmar cumplimiento PDF/UA
```

#### PAC 4 (PDF Accessibility Checker)
- **URL**: https://www.access-for-all.ch/en/pdf-lab/pdf-accessibility-checker-pac.html
- **Desarrollador**: Access for All Foundation
- **Tipo**: Gratuito
- **Características**:
  - Verificación PDF/UA completa
  - Vista previa de lector de pantalla
  - Análisis de estructura lógica
  - Reporte detallado de conformidad
- **Ideal para**: Verificación final de PDFs

### Documentos Web (HTML)

#### ACE by DAISY
- **URL**: https://inclusivepublishing.org/ace/
- **Tipo**: Herramienta de línea de comandos, gratuita
- **Uso**: Principalmente para EPUB, también HTML
- **Características**:
  - Verificación de estándares EPUB Accessibility
  - Reportes detallados en HTML
  - Integración con flujos de publicación
  - Validación de metadatos de accesibilidad

## 🛠️ Herramientas de Desarrollo y Integración

### Automatización y CI/CD

#### axe-core
- **URL**: https://github.com/dequelabs/axe-core
- **Tipo**: Librería JavaScript open source
- **Integraciones**: Jest, Selenium, Cypress, Playwright
- **Uso**: Pruebas automatizadas de accesibilidad en desarrollo

#### Pa11y CI
- **Características**:
  - Integración con sistemas de build
  - Configuración de umbrales de error
  - Reportes automatizados
  - Notificaciones de regresiones

### Extensiones de Navegador

#### Web Developer Toolbar
- **Funcionalidades para accesibilidad**:
  - Desactivar CSS para revisar estructura
  - Resaltar elementos semánticos
  - Validar marcado HTML
  - Revisar enlaces y navegación

#### HeadingsMap
- **URL**: Extensión para Chrome/Firefox
- **Función**: Visualizar estructura jerárquica de encabezados
- **Beneficio**: Identificar problemas en estructura semántica

## 📊 Estrategia de Evaluación Recomendada

### Fase 1: Evaluación Automática Inicial
1. **Verificador MinTIC** - Conformidad básica colombiana
2. **WAVE** - Problemas visuales evidentes
3. **axe DevTools** - Análisis técnico detallado
4. **Lighthouse** - Puntuación general y tendencias

### Fase 2: Evaluación Manual Especializada
1. **ANDI** - Inspección de nombres accesibles
2. **Navegación por teclado** - Pruebas de usabilidad
3. **Lector de pantalla** - NVDA o VoiceOver
4. **Contraste de colores** - Colour Contrast Analyser

### Fase 3: Validación con Usuarios
1. **Pruebas con usuarios reales** con discapacidades
2. **Feedback cualitativo** sobre experiencia de uso
3. **Validación de casos de uso** específicos
4. **Documentación de hallazgos** y mejoras

## 📈 Interpretación de Resultados

### Criterios de Priorización

**Nivel Alto (Bloqueo completo):**
- Contenido no accesible para lectores de pantalla
- Trampas de teclado
- Contraste insuficiente severo
- Formularios sin etiquetas

**Nivel Medio (Dificultad significativa):**
- Estructura de encabezados incorrecta
- Enlaces sin contexto claro
- Falta de texto alternativo en imágenes informativas
- Problemas de orden de tabulación

**Nivel Bajo (Mejoras menores):**
- Optimizaciones de rendimiento
- Mejoras en texto alternativo descriptivo
- Refinamiento de nombres accesibles
- Optimizaciones de CSS

### Métricas de Seguimiento

- **Errores automáticos**: Cantidad y tendencia en el tiempo
- **Puntuación Lighthouse**: Objetivo mínimo 90/100
- **Conformidad WCAG**: Porcentaje de criterios cumplidos
- **Tiempo de resolución**: Velocidad de corrección de problemas

## 🎯 Recomendaciones por Perfil

### Para Desarrolladores
1. Integrar axe-core en pruebas unitarias
2. Usar WAVE durante desarrollo
3. Configurar Lighthouse en CI/CD
4. Practicar navegación por teclado regularmente

### Para Diseñadores
1. Usar Colour Contrast Analyser en paletas
2. Validar prototipos con WAVE
3. Considerar simuladores de daltonismo
4. Documentar decisiones de accesibilidad

### Para Editores de Contenido
1. Usar Accessibility Checker de Office
2. Verificar PDFs con PAC 4
3. Probar contenido con lectores de pantalla
4. Mantener checklist de accesibilidad

### Para Gestores de Proyecto
1. Establecer criterios de aceptación accesibles
2. Incluir evaluaciones en sprints
3. Monitorear métricas de accesibilidad
4. Capacitar al equipo en herramientas básicas

---

*¿Conoces alguna herramienta adicional que debería incluirse? ¡Contribuye al repositorio!*