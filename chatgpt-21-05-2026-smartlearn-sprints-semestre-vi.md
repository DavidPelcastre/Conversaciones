# Smart Learn — Evidencia de Desarrollo mediante Metodología SCRUM

**Empresa:** CyberPath S.A.S.  
**Proyecto:** Smart Learn  
**Materia:** Proyecto Integrador  
**Metodología utilizada:** SCRUM adaptado al entorno académico  
**Periodo:** Semestre VI  

---

# Introducción

Durante el semestre VI, el desarrollo del proyecto Smart Learn se organizó mediante una metodología SCRUM adaptada al entorno académico, utilizando ciclos de trabajo semanales (sprints) enfocados en el análisis, desarrollo, pruebas e incremento del sistema.

El proyecto tuvo como objetivo continuar el desarrollo de una plataforma educativa accesible, incorporando mejoras relacionadas con accesibilidad, seguridad, infraestructura, aplicación móvil, plataforma web y futuras integraciones con Inteligencia Artificial y análisis de datos.

Cada sprint permitió generar avances iterativos y funcionales dentro de los distintos módulos del sistema, manteniendo una arquitectura escalable y preparada para futuras expansiones.

---

# Tecnologías Utilizadas

## Backend
- Java
- Spring Boot
- Spring Security
- JWT
- Maven
- MySQL

## Aplicación móvil
- Android Studio
- Java
- Retrofit
- SQLite/Room
- APIs REST

## Plataforma web
- HTML
- CSS
- JavaScript
- Vue.js
- Vite

## Infraestructura
- Microsoft Azure for Students
- Máquinas virtuales
- Servicios HTTP

## Tecnologías investigadas para futuras integraciones
- OpenAI Whisper
- Cloud Text-to-Speech
- Teachable Machine
- APIs de Inteligencia Artificial

---

# Desarrollo del Proyecto mediante SCRUM

## Sprint 1 — Análisis y definición de mejoras

### Objetivo
Identificar oportunidades de mejora en Smart Learn y definir nuevas funcionalidades relacionadas con accesibilidad, ciberseguridad, análisis de datos e integración de Inteligencia Artificial.

### Historias de usuario
- Como desarrollador, necesito identificar errores y áreas de mejora para optimizar el funcionamiento de la plataforma.
- Como administrador, necesito nuevas funcionalidades para gestionar mejor el contenido educativo.
- Como usuario, necesito una plataforma más accesible e intuitiva.

### Actividades realizadas
- Identificación de errores y oportunidades de mejora.
- Definición de nuevas funcionalidades para la plataforma.
- Análisis de integración de:
  - Inteligencia Artificial,
  - análisis de datos,
  - ciberseguridad.
- Elaboración de documentación de requerimientos:
  - generales,
  - IA,
  - análisis de datos,
  - ciberseguridad.
- Organización inicial del backlog del proyecto.

### Pruebas realizadas
- Validación de viabilidad técnica de requerimientos.
- Revisión inicial de compatibilidad entre módulos.

### Incremento
- Base de requerimientos funcionales y técnicos del semestre.

---

## Sprint 2 — Corrección y validación de requerimientos

### Objetivo
Refinar y validar la documentación funcional y técnica del sistema para iniciar el desarrollo de nuevas características.

### Historias de usuario
- Como equipo de desarrollo, necesitamos validar los requerimientos para asegurar una implementación correcta.
- Como administrador, necesito que las funcionalidades estén correctamente definidas antes de su implementación.

### Actividades realizadas
- Corrección de documentación de requerimientos.
- Presentación de requerimientos del sistema.
- Ajustes derivados de observaciones técnicas y funcionales.
- Refinamiento del backlog y priorización de tareas.

### Pruebas realizadas
- Revisión funcional de requerimientos.
- Validación de coherencia entre funcionalidades planeadas y arquitectura del sistema.

### Incremento
- Documentación refinada y validada para desarrollo.

---

## Sprint 3 — Mejora de interfaces y validaciones

### Objetivo
Mejorar la experiencia de usuario en la aplicación móvil y fortalecer las validaciones de autenticación.

### Historias de usuario
- Como usuario, necesito interfaces más accesibles y organizadas para mejorar la navegación.
- Como usuario, necesito validaciones seguras al iniciar sesión y registrarme.

### Actividades realizadas
- Mejora de interfaces gráficas en la aplicación móvil.
- Integración de elementos de accesibilidad.
- Implementación de validaciones en login y sign up.
- Desarrollo de lógica de validación de entradas.
- Investigación sobre:
  - Text To Speech (TTS),
  - análisis de datos mediante IA.
- Investigación sobre cifrado de datos móviles.

### Pruebas realizadas
- Validación de formularios de autenticación.
- Pruebas de navegación e interacción entre pantallas.
- Verificación de validaciones de datos de entrada.

### Incremento
- Interfaces más accesibles y validaciones funcionales de autenticación.

---

## Sprint 4 — Accesibilidad mediante lenguaje de señas

### Objetivo
Desarrollar un sistema inicial de accesibilidad auditiva basado en reproducción visual de lenguaje de señas.

### Historias de usuario
- Como usuario con discapacidad auditiva, necesito apoyo visual mediante lenguaje de señas para comprender mejor el contenido.
- Como usuario, necesito herramientas de accesibilidad integradas en la plataforma.

### Actividades realizadas
- Investigación sobre lenguaje de señas.
- Recopilación y organización de imágenes de:
  - abecedario,
  - palabras básicas.
- Diseño del sistema visual de reproducción de señas.
- Desarrollo inicial del módulo de accesibilidad auditiva.
- Planeación de integración mediante panel visual interactivo en pantalla.

### Pruebas realizadas
- Validación de reproducción visual de imágenes.
- Pruebas iniciales de integración en la interfaz móvil.

### Incremento
- Prototipo funcional parcial del sistema visual de lenguaje de señas.

---

## Sprint 5 — Investigación de IA y planeación de analítica

### Objetivo
Investigar tecnologías relacionadas con Inteligencia Artificial y preparar la arquitectura del módulo de análisis de datos.

### Historias de usuario
- Como administrador, necesito recopilar información de uso para generar futuras recomendaciones académicas.
- Como desarrollador, necesito evaluar tecnologías de IA compatibles con la plataforma.

### Actividades realizadas
- Investigación sobre modelos de IA mediante APIs externas.
- Investigación de herramientas y tecnologías como:
  - Teachable Machine,
  - Cloud Text-to-Speech,
  - Whisper de OpenAI.
- Planeación del módulo de análisis de datos:
  - aplicación móvil,
  - plataforma web.
- Investigación sobre tipos de cifrado para aplicación móvil.
- Mejora de interfaz gráfica web.
- Planeación de recopilación de datos académicos y de uso.

### Pruebas realizadas
- Evaluación de compatibilidad entre APIs y arquitectura existente.
- Validaciones preliminares de integración.

### Incremento
- Arquitectura inicial para futuras integraciones de IA y analítica.

---

## Sprint 6 — Implementación de seguridad y autenticación avanzada

### Objetivo
Fortalecer la seguridad del sistema mediante autenticación JWT y verificación en dos pasos.

### Historias de usuario
- Como usuario, necesito mecanismos de autenticación seguros para proteger mi cuenta.
- Como administrador, necesito proteger los endpoints y accesos del sistema.

### Actividades realizadas
- Implementación de autenticación mediante JWT.
- Protección de endpoints en el servidor Spring Boot.
- Configuración de seguridad mediante Spring Security.
- Implementación de verificación en dos pasos mediante OTP enviado por correo electrónico.
- Optimización de validación de credenciales en servidor.
- Implementación de filtros de autenticación y control de acceso.

### Pruebas realizadas
- Pruebas de autenticación y autorización.
- Validación de endpoints protegidos.
- Verificación de funcionamiento del sistema OTP.

### Incremento
- Sistema de autenticación y seguridad funcional en backend y plataforma web.

---

## Sprint 7 — Consolidación de plataforma web y recopilación de datos

### Objetivo
Consolidar el funcionamiento de la plataforma web administrativa y preparar la recopilación de datos académicos y de uso.

### Historias de usuario
- Como administrador, necesito gestionar materias, ejercicios y contenido desde una plataforma web.
- Como sistema, necesito recopilar datos de progreso y uso para futuras recomendaciones académicas.

### Actividades realizadas
- Consolidación de funcionalidades de la plataforma web administrativa.
- Implementación de gestión de:
  - materias,
  - temas,
  - subtemas,
  - teorías,
  - ejercicios.
- Preparación de recopilación de datos:
  - tiempo de uso,
  - progreso académico,
  - acceso a teoría,
  - realización de ejercicios,
  - aciertos.
- Integración parcial entre módulos móviles y web.
- Ajustes de interfaz y navegación.
- Mantenimiento de compatibilidad entre páginas HTML tradicionales y frontend basado en Vue.js.

### Pruebas realizadas
- Validación de navegación y operaciones CRUD.
- Pruebas funcionales de interacción entre frontend y backend.
- Verificación de almacenamiento de información.

### Incremento
- Plataforma web administrativa funcional y preparada para futuras integraciones analíticas.

---

## Sprint 8 — Infraestructura y despliegue en la nube

### Objetivo
Implementar infraestructura remota para el funcionamiento del servidor y comunicación cliente-servidor.

### Historias de usuario
- Como usuario, necesito acceso estable a la plataforma desde distintos dispositivos.
- Como desarrollador, necesito un entorno remoto para pruebas e integración del sistema.

### Actividades realizadas
- Configuración de máquinas virtuales mediante Azure for Students.
- Despliegue del servidor Spring Boot en entorno remoto.
- Configuración de comunicación mediante peticiones HTTP.
- Integración de conexión entre aplicación móvil, backend y plataforma web.
- Configuración de servicios para pruebas remotas.

### Pruebas realizadas
- Pruebas de conectividad cliente-servidor.
- Validación de peticiones y respuestas HTTP.
- Pruebas de estabilidad básica del servidor remoto.

### Incremento
- Servidor funcional desplegado en máquina virtual remota.

---

## Sprint 9 — Integración general y optimización

### Objetivo
Integrar los módulos desarrollados durante el semestre y optimizar el funcionamiento general del sistema.

### Historias de usuario
- Como usuario, necesito una plataforma estable e integrada.
- Como equipo de desarrollo, necesitamos consolidar los avances realizados durante el semestre.

### Actividades realizadas
- Corrección de errores detectados durante pruebas.
- Optimización general del sistema.
- Ajustes de seguridad y accesibilidad.
- Integración de módulos desarrollados en sprints anteriores.
- Organización y preparación de evidencias de desarrollo.
- Validación general de funcionalidades implementadas.

### Pruebas realizadas
- Pruebas generales de funcionamiento.
- Validación de integración entre módulos.
- Verificación de estabilidad básica del sistema.

### Incremento
- Versión integrada y funcional de Smart Learn con mejoras en accesibilidad, seguridad e infraestructura.

---

# Arquitectura General del Proyecto

El proyecto Smart Learn se encuentra dividido en múltiples módulos especializados:

## Backend
El backend fue desarrollado utilizando Spring Boot, implementando:
- autenticación JWT,
- protección de endpoints,
- verificación OTP,
- controladores REST,
- repositorios,
- servicios,
- DTOs,
- lógica de negocio,
- y conexión con base de datos MySQL.

## Aplicación móvil
La aplicación móvil fue desarrollada en Android Studio e incluye:
- autenticación,
- consumo de APIs REST,
- sincronización de contenido,
- accesibilidad visual y auditiva,
- gestión de materias,
- teoría,
- ejercicios,
- progreso académico,
- y validaciones de usuario.

## Plataforma web
La plataforma web administrativa permite:
- administración de materias,
- gestión de ejercicios,
- administración de usuarios,
- carga de contenido educativo,
- y mantenimiento de información académica.

La plataforma incluye tanto páginas HTML tradicionales como una migración parcial hacia Vue.js y Vite.

## Infraestructura
La infraestructura del sistema utiliza máquinas virtuales en Microsoft Azure for Students para:
- despliegue del backend,
- pruebas remotas,
- comunicación cliente-servidor,
- y validación de conectividad.

---

# Conclusiones

Durante el semestre VI se logró consolidar una arquitectura funcional y escalable para Smart Learn, permitiendo avances importantes en:
- seguridad,
- accesibilidad,
- despliegue remoto,
- administración web,
- y recopilación de datos académicos.

La metodología SCRUM adaptada permitió organizar el desarrollo de manera iterativa, facilitando la integración progresiva de nuevas funcionalidades y tecnologías.

Además, el sistema quedó preparado para futuras integraciones relacionadas con:
- Inteligencia Artificial,
- recomendaciones académicas,
- análisis de datos,
- y mejoras avanzadas de accesibilidad.

---

# Trabajo Futuro

El desarrollo de Smart Learn continúa activo y se contempla la realización de nuevos sprints enfocados en:
- integración de Inteligencia Artificial mediante APIs,
- generación de recomendaciones académicas,
- ampliación del sistema de lenguaje de señas,
- optimización de accesibilidad,
- mejoras de rendimiento,
- fortalecimiento de ciberseguridad,
- expansión de analítica de datos,
- y optimización de experiencia de usuario.

