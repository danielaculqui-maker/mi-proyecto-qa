# Casos de Prueba – HU-05: Control de accesos (ingreso/salida)

**Historia de usuario relacionada:** `historias_usuario/historia_5.md` (HU-05 – Módulo: Control de Accesos)

---

## TC-009 – Registro automático de ingreso de vehículo mediante sensor

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-009 |
| **Tipo** | Positivo (flujo normal) |
| **Objetivo** | Validar que el sistema registre automáticamente el ingreso de un vehículo detectado por el sensor, con fecha, hora, zona y fuente "SENSOR". |
| **Precondiciones** | El sensor de la garita está operativo y conectado al sistema. Existe un vehículo activo registrado en la base de datos. |
| **Datos de prueba** | Placa detectada: `PCD-5678` · Zona: `Zona A - Docentes` · Evento: `ENTRADA` · Fuente: `SENSOR` (generado automáticamente) |
| **Pasos** | 1. Simular la detección del vehículo `PCD-5678` por el sensor de la garita de ingreso.<br>2. Esperar a que el sistema procese el evento.<br>3. Consultar el historial de movimientos recién generado. |
| **Resultado esperado** | El sistema crea automáticamente un nuevo registro con evento "ENTRADA", fecha/hora actual, la zona correspondiente y fuente "SENSOR", sin intervención manual del guardia. |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |

---

## TC-010 – Registro manual de contingencia con datos obligatorios incompletos

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-010 |
| **Tipo** | Negativo (flujo alterno) |
| **Objetivo** | Validar que el sistema no permita guardar un registro manual de contingencia (por falla del sensor) si faltan datos obligatorios, como la zona del movimiento. |
| **Precondiciones** | El sensor de la garita presenta una falla simulada. El guardia tiene sesión iniciada y accede a la opción de registro manual como plan de contingencia. |
| **Datos de prueba** | Placa: `PCD-5678` · Evento: `SALIDA` · Zona: _(vacío)_ · Fuente: `MANUAL` |
| **Pasos** | 1. Simular la falla del sensor en la garita.<br>2. Acceder al registro manual de contingencia desde el panel del guardia.<br>3. Completar el evento y la placa, dejando el campo "Zona" vacío.<br>4. Intentar guardar el registro manual. |
| **Resultado esperado** | El sistema no guarda el movimiento, muestra un mensaje de error indicando que la zona es obligatoria y el registro no queda almacenado en la base de datos. |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |
