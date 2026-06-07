# chatgpt-07-06-2026-sprints-smartlearn-fase-final.md

## Objetivo
Definir y completar la planeación de los sprints finales del proyecto Smart Learn para su documentación en Jira y posterior incorporación a la tesina.

## Contexto
Se revisó la estructura de la tesina y la relación entre los sprints de documentación y los sprints de desarrollo del software. Se concluyó que el cronograma de la tesina debe reflejar principalmente el desarrollo del proyecto Smart Learn y no la redacción de capítulos.

También se analizaron las limitaciones actuales del proyecto:
- El proyecto se considera funcionalmente terminado.
- La IA de recomendaciones personalizadas no fue implementada y deberá eliminarse de la tesina o trasladarse a trabajo futuro.
- La accesibilidad auditiva sí fue implementada mediante secuencias de imágenes en Lengua de Señas Mexicana.
- No existen pruebas formales con usuarios externos.
- El límite aproximado de la tesina es de 80 páginas.

## Ideas clave
- Priorizar consistencia sobre perfección académica.
- Eliminar funcionalidades no implementadas de la documentación.
- Utilizar un cronograma basado en sprints reales del desarrollo.
- Mantener los casos de uso y evidencias al mínimo necesario para respetar el límite de páginas.
- Utilizar los sprints finales para justificar pruebas, validaciones y documentación.

## Decisiones

### Cronograma general
Se acordó utilizar el cronograma del desarrollo del sistema y no el cronograma de elaboración de la tesina.

Propuesta:
- S1: Análisis y definición de mejoras.
- S2: Corrección y validación de requerimientos.
- S3: Mejora de interfaces y validaciones.
- S4: Desarrollo de funcionalidades móviles.
- S5: Desarrollo de funcionalidades web.
- S6: Implementación de seguridad y autenticación avanzada.
- S7: Consolidación de plataforma web y recopilación de datos.
- S8: Infraestructura y despliegue en la nube.
- S9: Integración general y optimización.
- S10: Pruebas técnicas.
- S11: Validación de calidad.
- S12 (opcional): Cierre y entrega del proyecto.

### Sprint 6 – Implementación de seguridad y autenticación avanzada
Tareas definidas:
1. Implementar generación y validación de tokens JWT (5 SP).
2. Configurar Spring Security para autenticación y autorización (5 SP).
3. Proteger endpoints de la API mediante roles y permisos (3 SP).
4. Implementar filtro de autenticación JWT (3 SP).
5. Desarrollar módulo de verificación OTP por correo electrónico (8 SP).
6. Optimizar validación de credenciales en servidor (3 SP).
7. Implementar control de acceso basado en roles (3 SP).
8. Realizar pruebas funcionales de autenticación y autorización (5 SP).

Incremento:
- Autenticación JWT.
- OTP.
- Control de acceso por roles.
- Protección de endpoints.

### Sprint 7 – Consolidación de plataforma web y recopilación de datos
Tareas definidas:
1. Implementar gestión de materias en plataforma web (5 SP).
2. Implementar gestión de temas y subtemas (5 SP).
3. Implementar gestión de contenido teórico (5 SP).
4. Implementar gestión de ejercicios y evaluaciones (5 SP).
5. Implementar recopilación de métricas de uso y progreso académico (8 SP).
6. Integrar módulos web y móvil para sincronización de contenidos (8 SP).
7. Optimizar navegación y experiencia de usuario en plataforma web (3 SP).
8. Realizar pruebas funcionales de gestión académica y sincronización (5 SP).

Incremento:
- Gestión académica consolidada.
- Recopilación de métricas.
- Sincronización entre móvil y web.

### Sprint 8 – Infraestructura y despliegue en la nube
Tareas definidas:
1. Configurar entorno de alojamiento en Azure for Students (5 SP).
2. Implementar despliegue del servidor Spring Boot en entorno remoto (8 SP).
3. Configurar comunicación HTTP entre clientes y servidor (3 SP).
4. Configurar conexión remota entre aplicación móvil y backend (5 SP).
5. Configurar conexión remota entre plataforma web y backend (5 SP).
6. Configurar servicios y recursos para pruebas remotas (3 SP).
7. Validar integración completa de la arquitectura distribuida (5 SP).
8. Realizar pruebas funcionales de despliegue y conectividad (5 SP).

Incremento:
- Infraestructura en Azure.
- Backend desplegado.
- Arquitectura distribuida funcional.

### Sprint 9 – Integración general y optimización
Tareas definidas:
1. Corregir incidencias detectadas durante pruebas preliminares (5 SP).
2. Optimizar rendimiento general del sistema (5 SP).
3. Aplicar mejoras de seguridad y control de acceso (3 SP).
4. Optimizar funcionalidades de accesibilidad (3 SP).
5. Integrar módulos desarrollados en sprints anteriores (8 SP).
6. Validar flujo completo de operación del sistema (5 SP).
7. Organizar evidencias técnicas del desarrollo (3 SP).
8. Realizar validación general de funcionalidades implementadas (5 SP).

Incremento:
- Sistema completamente integrado.
- Evidencias organizadas.
- Versión candidata para pruebas finales.

### Sprint 10 – Pruebas técnicas
Tareas definidas:
1. Ejecutar pruebas unitarias del backend (5 SP).
2. Ejecutar pruebas unitarias de aplicación Android (5 SP).
3. Ejecutar pruebas de integración entre módulos (8 SP).
4. Ejecutar pruebas funcionales de plataforma web (5 SP).
5. Ejecutar pruebas funcionales de aplicación móvil (5 SP).
6. Registrar incidencias y resultados de pruebas (3 SP).
7. Corregir incidencias críticas detectadas (5 SP).

Incremento:
- Pruebas técnicas completadas.
- Correcciones críticas implementadas.

### Sprint 11 – Validación de calidad
Tareas definidas:
1. Ejecutar pruebas de accesibilidad (5 SP).
2. Ejecutar pruebas de seguridad (5 SP).
3. Ejecutar pruebas de rendimiento (5 SP).
4. Ejecutar pruebas de aceptación del sistema (8 SP).
5. Corregir observaciones derivadas de las pruebas finales (5 SP).
6. Actualizar documentación técnica del proyecto (3 SP).
7. Generar informe final de validación (3 SP).

Incremento:
- Validación integral completada.
- Informe final generado.

### Sprint 12 – Cierre y entrega (opcional)
Tareas definidas:
1. Realizar correcciones menores posteriores a validación (3 SP).
2. Preparar documentación final de la tesina (5 SP).
3. Organizar evidencias para presentación y defensa (3 SP).
4. Preparar materiales de exposición del proyecto (3 SP).
5. Generar versión final para entrega (2 SP).

Incremento:
- Proyecto listo para entrega y defensa.
- Documentación finalizada.

## Trabajo realizado
- Revisión de la coherencia de la tesina respecto al estado real del proyecto.
- Definición del enfoque del cronograma.
- Diseño de los sprints 6 al 12.
- Asignación de tareas y Story Points utilizando escala Fibonacci.
- Definición de incrementos por sprint.

## Problemas/dudas
- Confirmar el funcionamiento exacto de la IA utilizada para reconocimiento de comandos.
- Verificar si el Sprint 12 será necesario o si se integrará dentro del Sprint 11.
- Completar evidencias y resultados para los apartados de pruebas de la tesina.
- Verificar que las referencias bibliográficas estén completas.

## Conclusiones
- La estructura de 12 sprints es consistente con el desarrollo del proyecto.
- El Sprint 12 puede eliminarse sin afectar significativamente la narrativa del proyecto.
- Es prioritario eliminar de la tesina cualquier funcionalidad no implementada.
- Los apartados de pruebas, resultados y mejora continua serán los principales focos de trabajo para concluir la tesina.
