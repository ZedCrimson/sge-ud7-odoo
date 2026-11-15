## Tabla de Usuarios
| Usuario | Puesto | Tipo de Usuario | Módulos / Permisos Principales | Justificación (Principio de Mínimo Privilegio) |
| :--- | :--- | :--- | :--- | :--- |
| `comercial@TecnoSalva.com` | Comercial | Interno | Ventas (Solo documentos propios), Sin Contabilidad. | Solo necesita registrar y consultar sus propias ofertas de venta. |
| `respventas@TecnoSalva.com` | Responsable de Ventas | Interno | Ventas (Administrador), Inventario (Lector/Gestor). | Supervisa al equipo comercial y valida operaciones globales. |
| `adminfactura@TecnoSalva.com` | Administración | Interno | Facturación (Administrador), Ventas (Solo lectura). | Gestiona cobros, facturas y pagos sin interferir en la creación de ventas. |
| `portalcliente@TecnoSalva.com` | Cliente Final | Portal | Acceso exclusivo al portal web para ver sus pedidos y facturas. | Restringido estrictamente a su propia información como cliente externo. |

## Grupo Propio Personalizado
- **Nombre del grupo:** `TecnoSalva / Comercial Junior`
- **Herencia:** Hereda de los permisos básicos de Ventas (`sales_team.group_sale_salesman`).
- **Derechos de acceso sobre modelos clave:**
  - `sale.order` (Pedidos de Venta): Lectura (Sí), Escritura (Sí), Creación (Sí), Eliminación (No).
  - `res.partner` (Contactos): Lectura (Sí), Escritura (Sí), Creación (Sí), Eliminación (No).