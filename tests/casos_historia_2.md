# Casos de Prueba – HU-02: Registro temporal de visitantes

**Historia de usuario relacionada:** `historias_usuario/historia_2.md` (HU-02 – Módulo: Autenticación y Seguridad)

---

## TC-003 – Registro exitoso de un visitante con todos los datos obligatorios

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-003 |
| **Tipo** | Positivo (flujo normal) |
| **Objetivo** | Validar que un visitante sin correo institucional pueda registrarse temporalmente completando los datos obligatorios y que el sistema habilite su acceso al parqueadero. |
| **Precondiciones** | El visitante no está registrado previamente en el sistema. Se encuentra en la pantalla de login y selecciona la opción "Ir a Visitante". |
| **Datos de prueba** | Nombre completo: `Ana Pérez` · Cédula: `1712345678` · Placa: `PBX-1234` · Tipo de vehículo: `Auto` · Marca/Modelo: `Chevrolet Sail` · Motivo de visita: `Reunión con docente` · Duración estimada: `2 horas` · Correo de contacto: (vacío, opcional) |
| **Pasos** | 1. Acceder a la pantalla de login y seleccionar "Ir a Visitante".<br>2. Completar el formulario con nombre completo, cédula, placa, tipo de vehículo, marca/modelo, motivo de visita y duración estimada.<br>3. Dejar el correo de contacto vacío (campo opcional).<br>4. Hacer clic en "Registrar y continuar". |
| **Resultado esperado** | El sistema guarda el registro con fecha y hora, confirma el registro exitoso y habilita el acceso temporal del visitante al parqueadero. El guardia puede verificar el registro desde su panel. |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |

---

## TC-004 – Rechazo del registro de visitante con campos obligatorios incompletos

| Campo | Detalle |
|---|---|
| **ID del caso de prueba** | TC-004 |
| **Tipo** | Negativo (flujo alterno) |
| **Objetivo** | Validar que el sistema no permita completar el registro de un visitante cuando faltan datos obligatorios (por ejemplo, la placa del vehículo). |
| **Precondiciones** | El visitante se encuentra en el formulario de registro temporal, accedido desde la opción "Ir a Visitante". |
| **Datos de prueba** | Nombre completo: `Ana Pérez` · Cédula: `1712345678` · Placa: _(vacío)_ · Tipo de vehículo: `Auto` · Marca/Modelo: `Chevrolet Sail` · Motivo de visita: _(vacío)_ · Duración estimada: `2 horas` |
| **Pasos** | 1. Acceder a la pantalla de login y seleccionar "Ir a Visitante".<br>2. Completar el formulario dejando en blanco los campos obligatorios "Placa" y "Motivo de visita".<br>3. Hacer clic en "Registrar y continuar". |
| **Resultado esperado** | El sistema no guarda el registro, muestra un mensaje de error indicando qué campos obligatorios faltan y no habilita el acceso temporal al parqueadero. |
| **Resultado obtenido** | _Pendiente de ejecución_ |
| **Estado** | Pendiente |
| **Notas/Evidencias** | _Pendiente de ejecución_ |
