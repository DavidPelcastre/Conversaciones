# Conversación: Sistema de memoria con repositorio
Fecha: 2026-04-11

## 🎯 Objetivo
Definir una forma de guardar conversaciones del proyecto para reutilizarlas como contexto en futuras sesiones.

## 🧩 Contexto
El usuario busca que el asistente tenga acceso al historial de trabajo para mantener continuidad entre conversaciones, especialmente en el desarrollo de proyectos como Smart Learn.

## 💡 Ideas clave
- El asistente no puede recordar automáticamente conversaciones pasadas fuera del chat actual.
- Se puede crear una “memoria externa” usando archivos markdown.
- Un repositorio permite centralizar, organizar y versionar la información.
- Es importante estructurar bien los resúmenes para que sean reutilizables.

## ⚙️ Decisiones tomadas
- Se utilizará un repositorio (por ejemplo en GitHub) para almacenar resúmenes de conversaciones.
- Al finalizar cada conversación relevante, se generará un resumen en formato markdown.
- El usuario compartirá esos resúmenes en futuras sesiones para recuperar el contexto.

## 🛠️ Trabajo realizado
- Se definió un formato estándar de resumen en markdown.
- Se estableció un flujo de trabajo para guardar y reutilizar conversaciones.
- Se propuso una estructura de carpetas para organizar la información.

## ⚠️ Problemas / dudas
- El asistente no puede acceder automáticamente a repositorios ni aprender de ellos sin que el usuario comparta el contenido.
- La continuidad depende de que el usuario proporcione el contexto manualmente.

## ✅ Conclusiones
- Es posible simular una memoria persistente mediante un repositorio de resúmenes bien estructurados.
- El éxito del sistema depende de la consistencia en cómo se guardan y reutilizan los resúmenes.

## 📌 Pendientes / siguientes pasos
- Crear el repositorio y la estructura de carpetas.
- Empezar a guardar resúmenes de conversaciones relevantes.
- Probar el flujo compartiendo un resumen en una nueva conversación.
