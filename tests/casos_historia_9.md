# Casos de Prueba – HU-09: Exportación de reportes PDF

**Historia de usuario relacionada:** `historias_usuario/historia_9.md` (HU-09 – Módulo: Reportes)

---

## TC-017 – Generación y descarga exitosa de un reporte PDF de vehículos

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-017 |
| **Tipo** | Positivo (flujo normal) |
| **Objetivo** | Validar que el administrador pueda generar y descargar correctamente un reporte PDF de vehículos con los datos actualizados del sistema. |
| **Precondiciones** | El administrador tiene sesión iniciada con rol **Administrador**. Existen vehículos registrados en el sistema. |
| **Datos de prueba** | Tipo de reporte: `PDF de Vehículos` |
| **Pasos** | 1. Acceder al módulo de reportes desde el panel de administrador.<br>2. Seleccionar la opción "PDF de Vehículos".<br>3. Hacer clic en el botón de generar/descargar reporte.<br>4. Medir el tiempo de generación y abrir el archivo descargado. |
| **Resultado esperado** | El sistema genera el archivo PDF en menos de 5 segundos, se descarga automáticamente en el navegador, contiene los datos actualizados de los vehículos sin información faltante o corrupta, e incluye fecha y hora de generación. |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |

---

## TC-018 – Bloqueo de generación de reportes para usuarios sin rol Administrador

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-018 |
| **Tipo** | Negativo (flujo alterno) |
| **Objetivo** | Validar que un usuario sin rol Administrador no pueda generar ni descargar reportes PDF del sistema. |
| **Precondiciones** | Existe un usuario válido con rol distinto a Administrador (por ejemplo, Guardia) con sesión iniciada. |
| **Datos de prueba** | Correo: `guardia.prueba@uisekp.edu.ec` · Rol: `Guardia` · Tipo de reporte solicitado: `PDF de Usuarios` |
| **Pasos** | 1. Iniciar sesión con un usuario de rol Guardia.<br>2. Intentar acceder al módulo de reportes (directamente por menú o por URL).<br>3. Intentar generar el "PDF de Usuarios". |
| **Resultado esperado** | El sistema deniega el acceso a la funcionalidad de reportes, no genera ningún archivo PDF y muestra un mensaje indicando que el usuario no tiene permisos suficientes. |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |
