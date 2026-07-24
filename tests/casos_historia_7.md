# Casos de Prueba – HU-07: Mapa interactivo del parqueadero

**Historia de usuario relacionada:** `historias_usuario/historia_7.md` (HU-07 – Módulo: Mapa y Eventos)

---

## TC-013 – Visualización correcta del mapa y detalle de un marcador

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-013 |
| **Tipo** | Positivo (flujo normal) |
| **Objetivo** | Validar que el usuario pueda visualizar el mapa interactivo del Campus Miguel de Cervantes con sus marcadores y consultar el detalle de un cupo al hacer clic sobre él. |
| **Precondiciones** | El usuario tiene sesión iniciada y existen cupos con estados simulados (disponible, bloqueado, alerta) cargados en el sistema. |
| **Datos de prueba** | Marcador seleccionado: `Zona A - Cupo 12` (estado: disponible) |
| **Pasos** | 1. Acceder al módulo de mapa desde el panel del usuario.<br>2. Esperar a que el mapa cargue centrado en el Campus Miguel de Cervantes.<br>3. Verificar los contadores de cupos bloqueados, disponibles y alertas en el encabezado.<br>4. Hacer clic sobre el marcador "Zona A - Cupo 12". |
| **Resultado esperado** | El mapa carga correctamente centrado en el campus, muestra marcadores con colores según su estado y, al hacer clic en el marcador, se despliega la información detallada del cupo seleccionado (estado, zona). |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |

---

## TC-014 – Manejo de error cuando el mapa no logra cargar la base cartográfica

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-014 |
| **Tipo** | Negativo (flujo alterno) |
| **Objetivo** | Validar que el sistema informe adecuadamente al usuario cuando el mapa (OpenStreetMap) no puede cargarse, sin bloquear el resto de la aplicación. |
| **Precondiciones** | El usuario tiene sesión iniciada. Se simula la pérdida de conexión al servicio de OpenStreetMap (por ejemplo, bloqueando la petición de red al proveedor del mapa). |
| **Datos de prueba** | Condición simulada: servicio de mapas (OpenStreetMap) no disponible |
| **Pasos** | 1. Simular la falla de conexión al servicio de mapas.<br>2. Acceder al módulo de mapa desde el panel del usuario.<br>3. Observar el comportamiento de la pantalla. |
| **Resultado esperado** | El sistema muestra un mensaje indicando que el mapa no pudo cargarse (sin pantalla en blanco ni error no controlado) y el resto de la interfaz (encabezado, contadores, menú) permanece funcional. |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |
