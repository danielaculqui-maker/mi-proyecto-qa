# Casos de Prueba – HU-04: Gestión CRUD de vehículos

**Historia de usuario relacionada:** `historias_usuario/historia_4.md` (HU-04 – Módulo: Gestión de Vehículos)

---

## TC-007 – Registro exitoso de un nuevo vehículo con placa única

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-007 |
| **Tipo** | Positivo (flujo normal) |
| **Objetivo** | Validar que el administrador pueda registrar un nuevo vehículo con una placa que no existe activa en el sistema. |
| **Precondiciones** | El administrador tiene sesión iniciada y se encuentra en el menú "Gestionar Vehículos". No existe un vehículo activo con la placa a registrar. |
| **Datos de prueba** | Placa: `PCD-5678` (no registrada) · Tipo: `Auto` · Marca/Modelo: `Toyota Corolla` · Propietario: `Carlos Ramírez` (usuario existente) |
| **Pasos** | 1. Acceder al menú "Gestionar Vehículos" desde el panel de administrador.<br>2. Hacer clic en el botón "+".<br>3. Ingresar placa, tipo, marca/modelo y propietario.<br>4. Confirmar el guardado del vehículo. |
| **Resultado esperado** | El vehículo se agrega a la lista con estado "Activo", mostrando correctamente placa, tipo, marca/modelo, propietario y estado. Los cambios se reflejan inmediatamente en la base de datos. |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |

---

## TC-008 – Rechazo al registrar un vehículo con placa ya activa

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-008 |
| **Tipo** | Negativo (flujo alterno) |
| **Objetivo** | Validar que el sistema no permita registrar dos vehículos activos con la misma placa. |
| **Precondiciones** | Existe un vehículo activo registrado con placa `PCD-5678`. El administrador tiene sesión iniciada y está en el menú "Gestionar Vehículos". |
| **Datos de prueba** | Placa: `PCD-5678` (ya activa) · Tipo: `Eléctrico` · Marca/Modelo: `Kia Soul EV` · Propietario: `Ana Pérez` |
| **Pasos** | 1. Acceder al menú "Gestionar Vehículos".<br>2. Hacer clic en el botón "+".<br>3. Completar el formulario utilizando una placa ya activa en el sistema.<br>4. Intentar guardar el nuevo vehículo. |
| **Resultado esperado** | El sistema rechaza el registro, muestra un mensaje de error indicando que la placa ya se encuentra activa y no crea un registro duplicado. |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |
