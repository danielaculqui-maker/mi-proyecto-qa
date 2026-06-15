Sistema Inteligente de Control de Parqueaderos UISEK

---

Información General

| Campo      | Detalle                        |
|------------|-------------------------------|
| ID         | HU-05                         |
| Módulo     | Control de Accesos            |
| Prioridad  | Alta                          |
| Estimación | 5 puntos de historia          |

---

Historia de Usuario

Como sistema de control del parqueadero,
quiero registrar automáticamente el ingreso y salida de vehículos mediante sensores,
para llevar un control preciso de los movimientos vehiculares del campus sin depender
del factor humano.

---

Flujo Guiado

1. El sensor detecta el ingreso o salida de un vehículo en la garita.
2. El sistema registra automáticamente el evento, fecha, hora y zona.
3. El registro queda guardado en la base de datos con fuente "SENSOR".
4. En caso de fallo del sensor, el guardia puede registrar el movimiento manualmente
   con fuente "MANUAL" como plan de contingencia.
5. El administrador o guardia puede consultar el historial filtrando por tipo de evento
   y rango de fechas.
6. Se puede limpiar los filtros con el botón "Limpiar" para ver todos los registros.

---

Criterios de Aceptación

- El sistema registra automáticamente entradas y salidas mediante sensores.
- Cada movimiento almacena evento, fecha/hora, zona y fuente (SENSOR o MANUAL).
- El registro manual por parte del guardia solo aplica como plan de contingencia.
- Se puede filtrar el historial por tipo de evento y rango de fechas.
- Los movimientos quedan guardados inmediatamente en la base de datos.
- El historial muestra fecha, evento, zona, observación y fuente de cada registro.
