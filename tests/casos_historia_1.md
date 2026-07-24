# Casos de Prueba – HU-01: Inicio de sesión con roles

**Historia de usuario relacionada:** `historias_usuario/historia_1.md` (HU-01 – Módulo: Autenticación y Seguridad)

---

## TC-001 – Inicio de sesión exitoso con correo institucional válido

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-001 |
| **Tipo** | Positivo (flujo normal) |
| **Objetivo** | Validar que un usuario institucional con credenciales correctas y rol válido pueda iniciar sesión y sea redirigido al panel correspondiente a su rol. |
| **Precondiciones** | El usuario existe en la base de datos, su cuenta está en estado **Activo**, y tiene un rol asignado (Administrador, Guardia, Docente o Estudiante). |
| **Datos de prueba** | Correo: `docente.prueba@uisekp.edu.ec` · Contraseña: `Uisek#2025` (válida, correspondiente al hash almacenado) · Rol seleccionado: `Docente` |
| **Pasos** | 1. Ingresar a la pantalla de login institucional.<br>2. Escribir el correo `docente.prueba@uisekp.edu.ec` en el campo correspondiente.<br>3. Seleccionar el rol "Docente" en el menú desplegable.<br>4. Ingresar la contraseña válida.<br>5. Hacer clic en el botón "Ingresar". |
| **Resultado esperado** | El sistema valida las credenciales contra la base de datos, reconoce al usuario como activo y redirige automáticamente al panel correspondiente al rol Docente. No se muestra ningún mensaje de error. |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |

---

## TC-002 – Rechazo de inicio de sesión con correo no institucional o contraseña incorrecta

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-002 |
| **Tipo** | Negativo (flujo alterno) |
| **Objetivo** | Validar que el sistema rechace el inicio de sesión cuando el correo no pertenece al dominio institucional `@uisekp.edu.ec` o la contraseña es incorrecta, sin revelar cuál campo falló. |
| **Precondiciones** | El usuario intenta acceder desde la pantalla de login institucional; no se requiere sesión previa iniciada. |
| **Datos de prueba** | Caso A – Correo: `docente.prueba@gmail.com` (dominio inválido), Contraseña: `Uisek#2025`. Caso B – Correo: `docente.prueba@uisekp.edu.ec` (válido), Contraseña: `ClaveIncorrecta1` (inválida). |
| **Pasos** | 1. Ingresar a la pantalla de login institucional.<br>2. Escribir un correo con dominio no institucional (Caso A) o una contraseña incorrecta (Caso B).<br>3. Seleccionar cualquier rol del menú desplegable.<br>4. Hacer clic en el botón "Ingresar". |
| **Resultado esperado** | El sistema no permite el acceso, no redirige a ningún panel y muestra un mensaje de error genérico (p. ej. "Credenciales incorrectas") sin especificar si el error corresponde al correo, la contraseña o el rol. |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |
