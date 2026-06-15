Sistema Inteligente de Control de Parqueaderos UISEK

---

Información General

| Campo      | Detalle                        |
|------------|-------------------------------|
| ID         | HU-04                         |
| Módulo     | Gestión de Vehículos          |
| Prioridad  | Alta                          |
| Estimación | 4 puntos de historia          |

---

Historia de Usuario

Como administrador del sistema,
quiero registrar, editar y eliminar vehículos asociados a usuarios,
para tener un control actualizado de los vehículos autorizados en el campus.

---

Flujo Guiado

1. El administrador accede al menú "Gestionar Vehículos" desde su panel.
2. Visualiza la lista de vehículos con placa, tipo, marca/modelo, propietario y estado.
3. Para agregar un vehículo hace clic en "+" e ingresa placa, tipo, marca/modelo
   y propietario.
4. Para editar selecciona el ícono de lápiz y modifica los campos necesarios.
5. Para cambiar el estado hace clic en el ícono de estado (Activo/Inactivo).
6. Para eliminar selecciona el ícono de basura y confirma la acción.
7. Los cambios se reflejan inmediatamente en la lista de vehículos.

---

Criterios de Aceptación

- El formulario solicita placa, tipo (Auto, Furgoneta, Eléctrico), marca/modelo
  y propietario asociado.
- No se permiten dos vehículos activos con la misma placa.
- Se puede cambiar el estado del vehículo entre Activo e Inactivo.
- La eliminación requiere confirmación previa antes de ejecutarse.
- Solo el rol Administrador puede gestionar vehículos.
- Los cambios quedan guardados inmediatamente en la base de datos.
- Se puede distinguir visualmente entre vehículos institucionales y de visitantes.
