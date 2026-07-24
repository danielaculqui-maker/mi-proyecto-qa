# Casos de Prueba – HU-06: Historial de movimientos

**Historia de usuario relacionada:** `historias_usuario/historia_6.md` (HU-06 – Módulo: Historial de Movimientos)

---

## TC-011 – Filtrado exitoso del historial por tipo de evento y rango de fechas válido

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-011 |
| **Tipo** | Positivo (flujo normal) |
| **Objetivo** | Validar que el usuario pueda filtrar el historial de movimientos por tipo de evento y un rango de fechas válido, obteniendo solo los registros que cumplen los criterios. |
| **Precondiciones** | El usuario (Administrador o Guardia) tiene sesión iniciada y existen movimientos registrados en el sistema dentro y fuera del rango a filtrar. |
| **Datos de prueba** | Tipo de evento: `ENTRADA` · Fecha inicio: `2026-07-01` · Fecha fin: `2026-07-23` |
| **Pasos** | 1. Acceder al módulo de historial desde el panel correspondiente.<br>2. Seleccionar el tipo de evento "ENTRADA".<br>3. Ingresar el rango de fechas del 01/07/2026 al 23/07/2026.<br>4. Hacer clic en "Filtrar". |
| **Resultado esperado** | El sistema muestra únicamente los registros de tipo "ENTRADA" ocurridos dentro del rango de fechas indicado, con fecha/hora, evento, zona, observación y fuente visibles. |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |

---

## TC-012 – Filtrado con rango de fechas inválido (fecha fin anterior a fecha inicio)

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-012 |
| **Tipo** | Negativo (flujo alterno) |
| **Objetivo** | Validar que el sistema no ejecute un filtrado incorrecto ni muestre resultados erróneos cuando la fecha fin es anterior a la fecha de inicio. |
| **Precondiciones** | El usuario tiene sesión iniciada y se encuentra en el módulo de historial de movimientos. |
| **Datos de prueba** | Tipo de evento: `SALIDA` · Fecha inicio: `2026-07-23` · Fecha fin: `2026-07-01` (anterior a la fecha de inicio) |
| **Pasos** | 1. Acceder al módulo de historial.<br>2. Seleccionar el tipo de evento "SALIDA".<br>3. Ingresar como fecha de inicio el 23/07/2026 y como fecha fin el 01/07/2026.<br>4. Hacer clic en "Filtrar". |
| **Resultado esperado** | El sistema detecta el rango de fechas inválido, muestra un mensaje de error solicitando corregir las fechas y no aplica el filtro ni muestra resultados incorrectos. |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |
