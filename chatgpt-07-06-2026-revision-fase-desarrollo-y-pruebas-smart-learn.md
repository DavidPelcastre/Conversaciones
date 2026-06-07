# Resumen de conversación

## Objetivo
Revisar y fortalecer los apartados de **Fase de Desarrollo** y **Fase de Pruebas** de la tesina de Smart Learn, validando tecnologías, arquitectura, casos de prueba y casos de aceptación para asegurar consistencia entre la documentación y la implementación real del proyecto.

## Contexto
Smart Learn es una plataforma educativa accesible compuesta por:
- Aplicación móvil Android (Java).
- Plataforma web (Vue.js).
- Backend con Spring Boot y Spring Security.
- Base de datos MySQL.
- Almacenamiento local SQLite para funcionamiento offline.

Durante la revisión se buscó evitar inconsistencias entre la tesina y el sistema real, especialmente en temas de arquitectura, seguridad, accesibilidad y pruebas.

## Ideas clave
- La fase de desarrollo debe centrarse en la implementación del sistema, no en repetir análisis o diseño.
- Se identificó una corrección importante: el almacenamiento local utiliza SQLite y no Room.
- La documentación debe reflejar únicamente funcionalidades realmente implementadas.
- Los apartados de pruebas deben incluir evidencias y resultados verificables.
- Los casos de aceptación deben cubrir los flujos completos más importantes del sistema sin exceder una cantidad razonable.

## Decisiones
- Mantener la arquitectura de tres capas:
  - Cliente (Android y Web).
  - API REST (Spring Boot).
  - Base de datos (MySQL).
- Mantener el uso de:
  - Spring Security.
  - JWT.
  - HTTPS.
  - BCrypt.
  - Vue.js.
  - SQLite.
  - TextToSpeech.
  - SpeechRecognizer.
  - Autenticación biométrica.
- El sistema de recomendaciones no se manejará como motor inteligente; la recomendación se limitará a sugerir la revisión de teoría cuando existan errores.
- Mantener el funcionamiento offline mediante SQLite.
- Reducir los casos de aceptación a seis escenarios principales.

## Trabajo realizado
### Revisión de la fase de desarrollo
- Análisis de la estructura propuesta.
- Identificación de fortalezas y posibles mejoras.
- Validación conceptual de módulos web, móvil y backend.
- Elaboración de una lista de tecnologías, herramientas, patrones y mecanismos para verificar su implementación real.

### Revisión de la fase de pruebas
- Revisión de:
  - Pruebas unitarias.
  - Pruebas de integración.
  - Pruebas funcionales.
  - Pruebas de accesibilidad.
  - Pruebas de seguridad.
  - Pruebas de rendimiento.
- Identificación de errores de redacción y ortografía.
- Recomendaciones sobre métricas, evidencias y resultados.

### Casos de aceptación propuestos
1. Autenticación y acceso.
2. Gestión de contenido.
3. Consulta de contenido accesible.
4. Ejercicios y progreso.
5. Integración y modo offline.
6. Seguridad y auditoría.

## Problemas/dudas
- Falta definir con precisión cómo se medirán algunos indicadores:
  - Cobertura de pruebas.
  - Rendimiento.
  - Vulnerabilidades de seguridad.
- Pendiente validar la implementación final de todos los mecanismos descritos en la tesina mediante revisión directa del código.
- Pendiente completar la sección formal de resultados de aceptación.

## Conclusiones
- La estructura general de la tesina es sólida y adecuada para un proyecto de nivel técnico.
- Existe buena alineación entre accesibilidad, seguridad y objetivos educativos del proyecto.
- Conviene respaldar afirmaciones cuantitativas (cobertura, rendimiento, seguridad) con evidencia objetiva.
- La corrección de Room a SQLite evita una inconsistencia técnica importante.
- Los seis casos de aceptación definidos cubren los requerimientos funcionales y no funcionales más relevantes sin sobrecargar la documentación.

## Pendientes
- Revisar el código fuente de backend, móvil y web para validar la implementación real de las tecnologías documentadas.
- Completar la sección de casos de aceptación con resultados obtenidos y evidencias.
- Verificar métricas reales de pruebas antes de la redacción final.
- Revisar diagramas UML y consistencia con la implementación.
- Continuar la revisión integral de la tesina conforme avance el desarrollo.
