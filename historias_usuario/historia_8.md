Sistema Inteligente de Control de Parqueaderos UISEK

---

Información General

| Campo      | Detalle                        |
|------------|-------------------------------|
| ID         | HU-08                         |
| Módulo     | Módulo Administrativo         |
| Prioridad  | Media                         |
| Estimación | 4 puntos de historia          |

---

Historia de Usuario

Como administrador del sistema,
quiero visualizar un panel con métricas generales del parqueadero,
para tomar decisiones basadas en datos reales de ocupación y actividad del sistema.

---

Flujo Guiado

1. El administrador inicia sesión y accede a su panel administrativo.
2. El sistema muestra el estado actual del sprint (Activo/Inactivo).
3. Visualiza las métricas generales: usuarios activos, vehículos activos, cupos
   disponibles y movimientos del día.
4. Revisa el gráfico de flujo de entradas y salidas del día.
5. Si necesita activar o desactivar el sprint, hace clic en el botón correspondiente.
6. Los datos se actualizan automáticamente al recargar el panel.

---

Criterios de Aceptación

- El panel muestra usuarios activos, vehículos activos, cupos disponibles y
  movimientos del día.
- El estado del sprint (Activo/Inactivo) se muestra claramente en el encabezado.
- El administrador puede activar o desactivar el sprint desde el panel.
- Incluye un gráfico de flujo de entradas y salidas con datos simulados.
- Solo el rol Administrador puede acceder al panel completo.
- Las métricas son coherentes con los datos del historial y la base de datos.
- El panel es responsivo y se visualiza correctamente en distintos dispositivos.
