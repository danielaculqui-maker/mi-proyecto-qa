Sistema Inteligente de Control de Parqueaderos UISEK

---

Información General

| Campo      | Detalle                        |
|------------|-------------------------------|
| ID         | HU-10                         |
| Módulo     | Notificaciones                |
| Prioridad  | Baja                          |
| Estimación | 2 puntos de historia          |

---

Historia de Usuario

Como usuario del sistema,
quiero recibir notificaciones automáticas por correo ante eventos del parqueadero,
para estar informado sobre ingresos, salidas y confirmaciones sin necesidad de
revisar el sistema constantemente.

---

Flujo Guiado

1. El sistema detecta un evento definido: ingreso, salida o confirmación de registro.
2. El sistema genera automáticamente el correo con los detalles del evento.
3. El correo se envía vía Gmail mediante SMTP al destinatario correspondiente.
4. El destinatario recibe el correo con: tipo de evento, placa, fecha/hora y zona.
5. El envío queda registrado en el historial de notificaciones del sistema.
6. En caso de fallo en el envío, el sistema registra el error en logs sin interrumpir
   el flujo normal del parqueadero.

---

Criterios de Aceptación

- El sistema envía correo automáticamente al registrar el ingreso de un vehículo.
- El sistema envía correo automáticamente al registrar la salida de un vehículo.
- El correo incluye tipo de evento, placa, fecha/hora y zona del movimiento.
- El envío utiliza Gmail vía SMTP como servicio de correo.
- En ambiente de pruebas los correos se redirigen a una dirección de prueba.
- Si el envío falla, el error queda registrado en logs sin afectar el sistema.
- El historial de notificaciones enviadas queda disponible para revisión del administrador.
