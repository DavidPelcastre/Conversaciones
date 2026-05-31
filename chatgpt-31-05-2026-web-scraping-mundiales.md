# Objetivo

Desarrollar una tarea de Web Scraping en Python utilizando Beautiful Soup para obtener los resultados de los partidos de grupos de Copas Mundiales de la FIFA desde Wikipedia y generar automáticamente la tabla de posiciones aplicando criterios de desempate.

# Contexto

Se trabajó en una tarea de la materia Introducción al Análisis de Datos. El programa realiza scraping de páginas de Wikipedia en inglés correspondientes a grupos de la fase de grupos de distintos mundiales.

El usuario decidió utilizar una URL parametrizable mediante:
- año
- grupo

de forma que el mismo código pudiera reutilizarse para distintos mundiales cambiando únicamente dichas variables.

Además de generar la tabla, el programa debía ordenar a los equipos utilizando los siguientes criterios:

1. Puntos obtenidos.
2. Diferencia de goles.
3. Goles a favor.
4. Enfrentamiento directo.

# Ideas clave

- Uso de requests para descargar el HTML.
- Uso de BeautifulSoup para analizar la estructura de Wikipedia.
- Extracción de partidos desde elementos con clase `footballbox`.
- Generación de la tabla de posiciones a partir de los resultados obtenidos.
- Implementación de una función específica para resolver empates mediante enfrentamiento directo.
- Impresión tanto de la tabla final como de los partidos encontrados para evidenciar el scraping realizado.

# Decisiones

- Utilizar Wikipedia en inglés porque las URLs siguen una estructura más consistente.
- Mantener una única URL construida dinámicamente a partir del año y grupo.
- Conservar el sistema de puntuación de 3 puntos por victoria para todos los ejemplos utilizados.
- Demostrar el funcionamiento mediante ejemplos de:
  - Mundial 2002 Grupo G.
  - Mundial 1994 Grupo F.
  - Mundial 1974 Grupo A.
  - Mundial 1974 Grupo 2.
- No realizar modificaciones adicionales al código antes de la entrega.

# Trabajo realizado

- Revisión del código completo.
- Implementación del cuarto criterio de desempate mediante enfrentamiento directo.
- Uso de `cmp_to_key` para permitir una comparación personalizada durante el ordenamiento.
- Verificación conceptual del funcionamiento de los criterios de desempate.
- Revisión del PDF entregable.
- Validación de los ejemplos incluidos en el documento.
- Confirmación de que el Grupo F de 1994 demuestra correctamente:
  - igualdad en puntos,
  - igualdad en diferencia de goles,
  - desempate por goles a favor,
  - desempate por enfrentamiento directo.
- Confirmación de que los ejemplos de 1974 muestran correctamente la diferencia histórica en el sistema de puntuación y el uso de grupos numerados.

# Problemas/dudas

- El archivo Python utiliza `re.findall(...)` pero no incluye explícitamente `import re`, lo que podría provocar un error de ejecución si no se agregó posteriormente.
- El sistema de puntuación histórico no se adapta automáticamente a mundiales anteriores a 1994.
- En el PDF se explica correctamente esta diferencia histórica, pero el programa no la corrige automáticamente.
- Dependiendo del criterio de evaluación del profesor, podría considerarse únicamente una observación o una mejora pendiente.

# Conclusiones

- La solución cumple adecuadamente con los objetivos de scraping y generación de tablas.
- El código es reutilizable para distintos grupos y mundiales mediante cambios mínimos.
- El criterio de enfrentamiento directo quedó implementado.
- El PDF demuestra el funcionamiento de los criterios de desempate mediante casos reales.
- La explicación sobre los formatos históricos de grupos añade contexto útil sobre las diferencias entre mundiales.
- Como mejora futura, podría implementarse el cálculo automático de puntos históricos (2 puntos por victoria antes de 1994) para que los resultados coincidan completamente con las tablas oficiales de todos los mundiales.

# Pendientes

- Ninguno para esta entrega.
- Posible mejora futura: adaptar automáticamente la puntuación según el año del mundial.
