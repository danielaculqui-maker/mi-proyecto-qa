Sistema Inteligente de Control de Parqueaderos UISEK

---

Información General

| Campo      | Detalle                        |
|------------|-------------------------------|
| ID         | HU-06                         |
| Módulo     | Historial de Movimientos      |
| Prioridad  | Media                         |
| Estimación | 3 puntos de historia          |

---

Historia de Usuario

Como administrador o guardia del sistema,
quiero consultar el historial completo de ingresos y salidas con filtros por fecha
y tipo de evento,
para auditar movimientos y hacer seguimiento de vehículos en el parqueadero.

---

Flujo Guiado

1. El usuario accede al módulo de historial desde su panel correspondiente.
2. Visualiza la tabla con todos los movimientos registrados en el sistema.
3. Selecciona el tipo de evento a filtrar: ENTRADA o SALIDA.
4. Ingresa un rango de fechas para acotar los resultados.
5. Hace clic en "Filtrar" para aplicar los criterios seleccionados.
6. El sistema muestra los registros que coinciden con los filtros aplicados.
7. Si desea ver todos los registros nuevamente, hace clic en "Limpiar".

---

Criterios de Aceptación

- La tabla muestra fecha/hora, evento, zona, observación y fuente de cada movimiento.
- Se puede filtrar por tipo de evento (ENTRADA/SALIDA) y rango de fechas.
- El botón "Limpiar" reinicia todos los filtros aplicados.
- Los resultados son consistentes con la información almacenada en la base de datos.
- El guardia visualiza los movimientos de su zona; el administrador visualiza todos.
- El historial se actualiza en tiempo real con cada nuevo movimiento del sistema.
- Los registros muestran claramente si el movimiento fue detectado por SENSOR o MANUAL.
