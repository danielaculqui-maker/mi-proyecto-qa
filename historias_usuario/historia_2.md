Sistema Inteligente de Control de Parqueaderos UISEK

---

Información General

| Campo      | Detalle                        |
|------------|-------------------------------|
| ID         | HU-02                         |
| Módulo     | Autenticación y Seguridad     |
| Prioridad  | Alta                          |
| Estimación | 3 puntos de historia          |

---

Historia de Usuario

Como visitante sin correo institucional,
quiero registrarme temporalmente con mis datos personales y los de mi vehículo,
para poder ingresar al parqueadero de la UISEK de forma autorizada y controlada.

---

Flujo Guiado

1. El visitante accede a la pantalla de login y selecciona la opción "Ir a Visitante".
2. Se muestra el formulario de registro temporal de visitantes.
3. El visitante completa: nombre completo, cédula, placa del vehículo, tipo de vehículo,
   marca/modelo, motivo de visita y duración estimada.
4. Opcionalmente ingresa su correo de contacto y marca si tiene discapacidad.
5. Hace clic en "Registrar y continuar".
6. El sistema guarda el registro y permite el acceso temporal al parqueadero.
7. El guardia o recepción puede verificar el registro desde su panel.

---

Criterios de Aceptación

- El formulario solicita nombre completo, cédula, placa, tipo de vehículo, marca/modelo,
  motivo de visita y duración estimada.
- El correo de contacto es opcional.
- Se puede indicar si el visitante tiene discapacidad.
- El sistema confirma el registro y habilita el acceso temporal.
- El guardia puede verificar y validar el registro del visitante desde su panel.
- La interfaz funciona en modo oscuro, claro y contraste alto.
- Los datos del visitante quedan registrados en la base de datos con fecha y hora.
