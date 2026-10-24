# Guía de seguimiento

## Flujo

Requerimiento → Issue → rama → Pull Request → prueba → evidencia → cierre.

Cada Issue tiene un responsable principal que debe asignarse en la reunión inicial. No se han asignado personas sin conocer la distribución del equipo.

Estados: Pendiente, Listo para iniciar, En desarrollo, En revisión, En pruebas y Terminado. Registrar bloqueos como campo separado y explicar la dependencia en la Issue.

Crear ramas como `feat/rf05-envio-mensajes` o `test/rnf03-tiempo-entrega`. Los PR deben enlazar Issues mediante `Refs #N`. Utilizar `Closes #N` solo cuando el PR complete los criterios y las evidencias del requisito. No cerrar requisitos por código sin verificar.

## Configuración manual pendiente: Projects

La conexión usada para preparar este repositorio no permite crear Projects, Milestones ni etiquetas. Estos elementos no están creados.

Crear un Project con vista de tablero, vincular este repositorio y agregar las 26 Issues existentes. Configurar los seis estados anteriores y campos Tipo, Prioridad, Semana, Fecha objetivo y Bloqueado. Usar Assignees para responsables. Revisar que las Issues estén efectivamente añadidas al Project.

## Configuración manual pendiente: Milestones

Crear desde la sección Issues → Milestones, con estos títulos y vencimientos; asociar las Issues según la semana indicada en su descripción.

| Título | Vencimiento |
|---|---|
| S1 — Análisis y preparación | 2026-11-01 |
| S2 — Diseño de la solución | 2026-11-08 |
| S3 — Mensajería básica | 2026-11-15 |
| S4 — Confiabilidad y protección | 2026-11-22 |
| S5 — Integración y evaluación | 2026-11-29 |
| S6 — Entrega final | 2026-12-06 |

S1 y S2 agrupan tareas de preparación y diseño que el equipo debe desglosar; los requerimientos principales se cierran al verificarse. Crear tareas semanales adicionales cuando corresponda.

Etiquetas sugeridas: funcional, no-funcional, documentacion, pruebas, bloqueado. No son necesarias para usar las plantillas.

## Revisión semanal

Registrar resultados, Issues verificadas, PR integrados, pruebas, bloqueos, acciones, responsables y fechas en una Issue usando la plantilla Seguimiento semanal. Revisar retrasos y actualizar el cronograma sin borrar decisiones previas.

Indicadores: RF verificados/13; RNF verificados/13; tareas semanales terminadas/comprometidas; bloqueos y antigüedad; defectos abiertos. La cantidad de commits no es una medida suficiente del aporte.

## Definición de terminado

- Criterios de aceptación cumplidos.
- Cambios revisados y enlazados.
- Pruebas con condiciones, resultados y evidencia.
- Documentación actualizada y limitaciones explícitas.
- Issue cerrada y estado del tablero actualizado.

Recomendación: configurar una regla de protección para main con revisión por PR cuando haya otro revisor disponible. No se ha aplicado protección de ramas.
