# Casos de Prueba – HU-03: Gestión CRUD de usuarios

**Historia de usuario relacionada:** `historias_usuario/historia_3.md` (HU-03 – Módulo: Gestión de Usuarios)

---

## TC-005 – Creación exitosa de un nuevo usuario con correo único

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-005 |
| **Tipo** | Positivo (flujo normal) |
| **Objetivo** | Validar que el administrador pueda registrar un nuevo usuario con un correo que no existe previamente en el sistema. |
| **Precondiciones** | El usuario que ejecuta la prueba tiene sesión iniciada con rol **Administrador** y se encuentra en el menú "Gestionar Personas". |
| **Datos de prueba** | Nombre: `Carlos Ramírez` · Correo: `carlos.ramirez@uisekp.edu.ec` (no registrado previamente) · Tipo: `UISEK` · Rol: `Estudiante` |
| **Pasos** | 1. Acceder al menú "Gestionar Personas" desde el panel de administrador.<br>2. Hacer clic en el botón "+".<br>3. Completar los datos requeridos: nombre, correo, tipo y rol.<br>4. Confirmar el guardado del nuevo usuario. |
| **Resultado esperado** | El nuevo usuario se agrega a la lista con estado "Activo", mostrando nombre, correo, estado y tipo correctamente. Los cambios se reflejan inmediatamente y quedan guardados en la base de datos. |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |

---

## TC-006 – Rechazo al crear un usuario con correo duplicado

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-006 |
| **Tipo** | Negativo (flujo alterno) |
| **Objetivo** | Validar que el sistema impida registrar dos usuarios con el mismo correo electrónico. |
| **Precondiciones** | Existe previamente un usuario registrado con el correo `carlos.ramirez@uisekp.edu.ec`. El administrador tiene sesión iniciada y está en el menú "Gestionar Personas". |
| **Datos de prueba** | Nombre: `Carlos R. Duplicado` · Correo: `carlos.ramirez@uisekp.edu.ec` (ya existente) · Tipo: `UISEK` · Rol: `Docente` |
| **Pasos** | 1. Acceder al menú "Gestionar Personas".<br>2. Hacer clic en el botón "+".<br>3. Completar el formulario utilizando un correo ya registrado en el sistema.<br>4. Intentar guardar el nuevo usuario. |
| **Resultado esperado** | El sistema rechaza la creación del usuario, muestra un mensaje de error indicando que el correo ya está registrado y no agrega ningún registro duplicado a la lista. |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |
