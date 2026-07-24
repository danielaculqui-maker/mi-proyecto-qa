# Casos de Prueba – HU-10: Notificaciones por correo (SMTP)

**Historia de usuario relacionada:** `historias_usuario/historia_10.md` (HU-10 – Módulo: Notificaciones)

---

## TC-019 – Envío exitoso de notificación por correo al registrar un ingreso

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-019 |
| **Tipo** | Positivo (flujo normal) |
| **Objetivo** | Validar que el sistema envíe automáticamente un correo de notificación con los detalles correctos al registrarse el ingreso de un vehículo. |
| **Precondiciones** | El servicio SMTP (Gmail) está configurado y operativo. El ambiente de pruebas redirige los correos a una dirección de prueba. Existe un vehículo activo asociado a un propietario. |
| **Datos de prueba** | Evento: `ENTRADA` · Placa: `PCD-5678` · Zona: `Zona A - Docentes` · Correo destino (ambiente de pruebas): `qa.pruebas@uisekp.edu.ec` |
| **Pasos** | 1. Registrar el ingreso del vehículo con placa `PCD-5678` en la zona "Zona A - Docentes" (vía sensor o manual).<br>2. Esperar a que el sistema procese el evento y dispare la notificación.<br>3. Revisar la bandeja de la dirección de correo de prueba.<br>4. Consultar el historial de notificaciones del sistema. |
| **Resultado esperado** | El sistema envía automáticamente un correo vía SMTP con tipo de evento "ENTRADA", placa, fecha/hora y zona correctos, dirigido a la dirección de prueba configurada; el envío queda registrado en el historial de notificaciones. |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |

---

## TC-020 – Manejo correcto de fallo en el envío de notificación por correo

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-020 |
| **Tipo** | Negativo (flujo alterno) |
| **Objetivo** | Validar que, si el envío del correo de notificación falla (por ejemplo, error del servicio SMTP), el sistema registre el error en logs sin interrumpir el flujo normal del parqueadero. |
| **Precondiciones** | Se simula una falla del servicio SMTP (credenciales inválidas o servicio no disponible). Existe un vehículo activo listo para registrar un movimiento. |
| **Datos de prueba** | Evento: `SALIDA` · Placa: `PCD-5678` · Condición simulada: servicio SMTP no disponible / credenciales inválidas |
| **Pasos** | 1. Configurar temporalmente el servicio SMTP con credenciales inválidas o simular su caída.<br>2. Registrar la salida del vehículo con placa `PCD-5678`.<br>3. Verificar si el registro del movimiento se completa correctamente.<br>4. Revisar los logs del sistema. |
| **Resultado esperado** | El movimiento de salida se registra correctamente en el historial a pesar del fallo de correo; el sistema no interrumpe el flujo del parqueadero, registra el error de envío en los logs y no genera una excepción visible para el usuario final. |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |
