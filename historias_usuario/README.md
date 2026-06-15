Sistema Inteligente de Control de Parqueaderos UISEK

- Descripción del Proyecto
Sistema web desarrollado en arquitectura MVC que digitaliza y centraliza la gestión
del parqueadero institucional del Campus Miguel de Cervantes (Carcelén) de la UISEK.
Permite controlar el ingreso y salida de vehículos, administrar usuarios por rol,
visualizar el estado del parqueadero en un mapa interactivo y generar reportes,
todo desde una plataforma accesible, responsiva y segura.

- Funcionalidades principales

1. Inicio de sesión con roles:** acceso seguro con validación de credenciales y
   redirección según rol (Administrador, Guardia, Docente, Estudiante).
2. Registro temporal de visitantes: formulario de acceso rápido para personas
   sin correo institucional, con placa, motivo de visita y duración estimada.
3. Gestión CRUD de usuarios: registrar, editar, activar/desactivar y eliminar
   personas del sistema según perfil institucional o visitante.
4. Gestión CRUD de vehículos: registrar y administrar vehículos con placa,
   tipo, marca/modelo y propietario asociado.
5. Control de accesos (ingreso/salida): simular entradas y salidas de vehículos
   con fecha, hora, zona y fuente del registro (sensor o manual).
6. Historial de movimientos: consultar ingresos y salidas con filtros por evento,
   fecha y zona, con paginación de resultados.
7. Mapa interactivo del parqueadero: visualizar cupos disponibles, bloqueados
   y alertas en tiempo simulado mediante marcadores en el mapa.
8. Dashboard administrativo: ver métricas generales como usuarios activos,
   vehículos, cupos disponibles y flujo de entradas/salidas del día.
9. Exportación de reportes PDF: generar y descargar reportes de vehículos
   y usuarios en formato PDF.
10. Notificaciones por correo (SMTP): envío automático de correos ante eventos
    como ingresos, salidas y confirmaciones, vía Gmail.

- Estructura del repositorio

historias_usuario/
├── historia_1.md  → Inicio de sesión con roles
├── historia_2.md  → Registro temporal de visitantes
├── historia_3.md  → Gestión CRUD de usuarios
├── historia_4.md  → Gestión CRUD de vehículos
├── historia_5.md  → Control de accesos (ingreso/salida)
├── historia_6.md  → Historial de movimientos
├── historia_7.md  → Mapa interactivo del parqueadero
├── historia_8.md  → Dashboard administrativo
├── historia_9.md  → Exportación de reportes PDF
├── historia_10.md → Notificaciones por correo (SMTP)
└── README.md      → Este archivo
