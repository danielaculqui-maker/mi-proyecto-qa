# Casos de Prueba – HU-08: Dashboard administrativo

**Historia de usuario relacionada:** `historias_usuario/historia_8.md` (HU-08 – Módulo Administrativo)

---

## TC-015 – Visualización correcta de métricas en el panel administrativo

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-015 |
| **Tipo** | Positivo (flujo normal) |
| **Objetivo** | Validar que el administrador pueda visualizar correctamente las métricas generales del parqueadero (usuarios activos, vehículos activos, cupos disponibles y movimientos del día) en su panel. |
| **Precondiciones** | El administrador tiene sesión iniciada con rol **Administrador**. Existen datos de usuarios, vehículos y movimientos registrados en el sistema. |
| **Datos de prueba** | Rol: `Administrador` · Estado del sprint: `Activo` |
| **Pasos** | 1. Iniciar sesión con un usuario de rol Administrador.<br>2. Acceder al panel administrativo.<br>3. Verificar las métricas mostradas: usuarios activos, vehículos activos, cupos disponibles y movimientos del día.<br>4. Revisar el gráfico de flujo de entradas y salidas del día. |
| **Resultado esperado** | El panel muestra correctamente el estado del sprint y todas las métricas solicitadas, coherentes con los datos almacenados en el historial y la base de datos, incluyendo el gráfico de flujo de entradas/salidas. |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |

---

## TC-016 – Bloqueo de acceso al panel administrativo para usuarios sin rol Administrador

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-016 |
| **Tipo** | Negativo (flujo alterno) |
| **Objetivo** | Validar que un usuario sin rol Administrador no pueda acceder al panel administrativo completo con sus métricas. |
| **Precondiciones** | Existe un usuario válido con rol distinto a Administrador (por ejemplo, Estudiante) con sesión iniciada. |
| **Datos de prueba** | Correo: `estudiante.prueba@uisekp.edu.ec` · Rol: `Estudiante` |
| **Pasos** | 1. Iniciar sesión con un usuario de rol Estudiante.<br>2. Intentar acceder directamente a la URL/ruta del panel administrativo.<br>3. Observar la respuesta del sistema. |
| **Resultado esperado** | El sistema deniega el acceso al panel administrativo, redirige al usuario a su panel correspondiente o muestra un mensaje de "Acceso no autorizado", sin exponer las métricas administrativas. |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |
