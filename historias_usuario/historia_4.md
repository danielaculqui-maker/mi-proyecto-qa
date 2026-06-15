Sistema Inteligente de Control de Parqueaderos UISEK

---

Información General

| Campo      | Detalle                        |
|------------|-------------------------------|
| ID         | HU-03                         |
| Módulo     | Gestión de Usuarios           |
| Prioridad  | Alta                          |
| Estimación | 4 puntos de historia          |

---

Historia de Usuario

Como administrador del sistema,
quiero crear, editar, activar/desactivar y eliminar usuarios,
para mantener actualizado el registro de personas autorizadas en el parqueadero.

---

Flujo Guiado

1. El administrador accede al menú "Gestionar Personas" desde su panel.
2. Visualiza la lista de usuarios con nombre, correo, estado y tipo (UISEK/Visitante).
3. Para agregar un usuario hace clic en el botón "+" e ingresa los datos requeridos.
4. Para editar selecciona el ícono de lápiz junto al usuario y modifica los campos.
5. Para cambiar el estado hace clic en el ícono de estado (Activo/Inactivo).
6. Para eliminar selecciona el ícono de basura y confirma la acción.
7. Los cambios se reflejan inmediatamente en la lista de usuarios.

---

Criterios de Aceptación

- La lista muestra nombre, correo, estado (Activo/Inactivo) y tipo (UISEK/Visitante).
- No se permiten dos usuarios registrados con el mismo correo.
- El cambio de estado (activar/desactivar) se aplica con un solo clic.
- La eliminación de un usuario requiere confirmación antes de ejecutarse.
- Solo el rol Administrador puede acceder a la gestión de usuarios.
- Los cambios quedan guardados inmediatamente en la base de datos.
- Se puede distinguir visualmente entre usuarios institucionales y visitantes.
