Sistema Inteligente de Control de Parqueaderos UISEK

---

Información General

| Campo      | Detalle                        |
|------------|-------------------------------|
| ID         | HU-07                         |
| Módulo     | Mapa y Eventos                |
| Prioridad  | Media                         |
| Estimación | 4 puntos de historia          |

---

Historia de Usuario

Como usuario del sistema,
quiero visualizar el estado del parqueadero en un mapa interactivo con marcadores,
para conocer de forma visual y rápida los cupos disponibles, bloqueados y alertas
activas en el campus.

---

Flujo Guiado

1. El usuario accede al módulo de mapa desde su panel.
2. El sistema carga el mapa interactivo centrado en el Campus Miguel de Cervantes.
3. Se muestran marcadores de colores según el estado de cada zona del parqueadero.
4. El encabezado muestra contadores de cupos bloqueados, disponibles y alertas activas.
5. El usuario hace clic en un marcador para ver la información detallada del cupo o evento.
6. El mapa se puede desplazar y hacer zoom para explorar las diferentes zonas.

---

Criterios de Aceptación

- El mapa se centra automáticamente en el Campus Miguel de Cervantes de la UISEK.
- Los marcadores muestran colores distintos según su estado: disponible, bloqueado y alerta.
- El encabezado muestra contadores en tiempo simulado de bloqueados, disponibles y alertas.
- Cada marcador es clicable y muestra información detallada del cupo o evento.
- El mapa utiliza OpenStreetMap como base cartográfica.
- La información mostrada es simulada pero visualmente coherente con el campus real.
