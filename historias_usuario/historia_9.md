Sistema Inteligente de Control de Parqueaderos UISEK

---

Información General

| Campo      | Detalle                        |
|------------|-------------------------------|
| ID         | HU-09                         |
| Módulo     | Reportes                      |
| Prioridad  | Media                         |
| Estimación | 3 puntos de historia          |

---

Historia de Usuario

Como administrador del sistema,
quiero generar y descargar reportes en formato PDF de usuarios y vehículos,
para documentar y compartir el estado actual del parqueadero institucional.

---

Flujo Guiado

1. El administrador accede al módulo de reportes desde su panel.
2. Visualiza las opciones disponibles: PDF de Vehículos y PDF de Usuarios.
3. Selecciona el tipo de reporte que desea generar.
4. El sistema genera el archivo PDF con los datos actualizados del sistema.
5. El archivo se descarga automáticamente en el navegador del administrador.
6. El PDF contiene toda la información registrada al momento de su generación.

---

Criterios de Aceptación

- Se pueden generar dos tipos de reporte: PDF de Vehículos y PDF de Usuarios.
- Cada PDF se descarga automáticamente al hacer clic en el botón correspondiente.
- El archivo contiene los datos actualizados del sistema al momento de generarlo.
- El PDF conserva la integridad de la información sin datos faltantes o corruptos.
- Solo el rol Administrador puede generar y descargar reportes.
- La generación del PDF se completa en menos de 5 segundos.
- El reporte incluye fecha y hora de generación como sello temporal.
