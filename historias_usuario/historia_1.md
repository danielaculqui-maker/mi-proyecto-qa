Sistema Inteligente de Control de Parqueaderos UISEK

---

Información General

| Campo      | Detalle                        |
|------------|-------------------------------|
| ID         | HU-01                         |
| Módulo     | Autenticación y Seguridad     |
| Prioridad  | Alta                          |
| Estimación | 3 puntos de historia          |

---

Historia de Usuario

Como miembro institucional (Administrador, Guardia, Docente o Estudiante),
quiero ingresar al sistema con mi correo @uisekp.edu.ec y seleccionar mi rol,
para acceder únicamente a las funciones y vistas que me corresponden según mi perfil.

---

Flujo Guiado

1. El usuario ingresa a la pantalla de login institucional.
2. Escribe su correo con dominio @uisekp.edu.ec.
3. Selecciona su rol en el menú desplegable (Estudiante, Docente, Administrativo, Guardia).
4. Hace clic en ingresar.
5. El sistema valida las credenciales contra la base de datos.
6. Si son correctas, redirige al panel correspondiente según el rol.
7. Si son incorrectas, muestra un mensaje de error sin revelar cuál campo falló.

---

Criterios de Aceptación

- El formulario solicita correo institucional y un menú de selección de rol.
- Solo se aceptan correos con dominio @uisekp.edu.ec.
- Cada rol es redirigido a su panel correspondiente tras autenticarse correctamente.
- La pantalla incluye opciones de accesibilidad: modo claro, oscuro, contraste y dislexia.
- Las contraseñas se almacenan con hash y salt, nunca en texto plano.
- El sistema con datos simulados valida que el usuario esté activo antes de permitir el acceso.
