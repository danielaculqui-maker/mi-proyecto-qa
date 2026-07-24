# Casos de Prueba – mi-proyecto-qa

Esta carpeta contiene los casos de prueba correspondientes a cada historia de usuario definida en `historias_usuario/`, siguiendo el sistema **Sistema Inteligente de Control de Parqueaderos UISEK**.

Por cada historia de usuario se elaboraron **2 casos de prueba**:

- **Caso positivo (flujo normal):** valida que la funcionalidad se cumple correctamente con datos válidos.
- **Caso negativo (flujo alterno):** valida que el sistema responde adecuadamente ante errores, datos inválidos o condiciones no permitidas.

## Índice

| Archivo | Historia de usuario | Casos de prueba |
|---|---|---|
| `casos_historia_1.md` | HU-01 – Inicio de sesión con roles | TC-001, TC-002 |
| `casos_historia_2.md` | HU-02 – Registro temporal de visitantes | TC-003, TC-004 |
| `casos_historia_3.md` | HU-03 – Gestión CRUD de usuarios | TC-005, TC-006 |
| `casos_historia_4.md` | HU-04 – Gestión CRUD de vehículos | TC-007, TC-008 |
| `casos_historia_5.md` | HU-05 – Control de accesos (ingreso/salida) | TC-009, TC-010 |
| `casos_historia_6.md` | HU-06 – Historial de movimientos | TC-011, TC-012 |
| `casos_historia_7.md` | HU-07 – Mapa interactivo del parqueadero | TC-013, TC-014 |
| `casos_historia_8.md` | HU-08 – Dashboard administrativo | TC-015, TC-016 |
| `casos_historia_9.md` | HU-09 – Exportación de reportes PDF | TC-017, TC-018 |
| `casos_historia_10.md` | HU-10 – Notificaciones por correo (SMTP) | TC-019, TC-020 |

## Campos de cada caso de prueba

Cada caso documenta: ID, tipo (positivo/negativo), objetivo, precondiciones, datos de prueba, pasos, resultado esperado, resultado obtenido, estado y notas/evidencias. Los campos "Resultado obtenido", "Estado" y "Notas/Evidencias" quedan marcados como **Pendiente** hasta que se ejecuten las pruebas.
