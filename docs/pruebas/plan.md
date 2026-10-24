# Plan y registro de pruebas

No hay pruebas ejecutadas: el prototipo todavía no está implementado.

## Registro obligatorio

Por ejecución: fecha, autor, versión/commit, requisitos, hardware, sistema operativo, topología, configuración de red, número de saltos, tamaño y cantidad de mensajes, pasos, resultado esperado, resultado observado y archivos de evidencia. No publicar contraseñas, claves privadas ni datos personales.

## Escenarios

1. Configuración válida e inválida; identidades y nombres repetidos.
2. Descubrimiento, retiro y reconexión de nodos; documentar cobertura multisalto.
3. Envío, recepción, orden local y validación de entradas.
4. Confirmaciones, pérdida de confirmación y retransmisión sin duplicados.
5. Reinicio, persistencia y cierre controlado.
6. Ausencia de Internet y de servidor central.
7. Cinco nodos, un salto estable, mensajes hasta 2 KiB: al menos 95 % confirmado en menos de 2 s. Medir desde envío a confirmación con reloj monotónico local.
8. Prueba estable de 100 mensajes: al menos 99 confirmados y cero duplicados visibles. Contar fallos; no excluirlos de los resultados.
9. Seguridad del canal, identidad inválida, permisos del historial y registros sin texto.
10. Usabilidad, instalación Linux, CPU, memoria y tráfico en reposo/carga.
11. Reproducción por una segunda persona.

Usar tiempos locales de ida y confirmación evita asumir sincronización entre nodos. Una prueba sobre un punto de acceso convencional verifica la aplicación, pero no demuestra por sí sola una red ad hoc.
