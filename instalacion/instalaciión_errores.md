# Registro de Errores de Instalación

| Error o Mensaje | Causa | Solución Aplicada | Fuente Consultada |
| :--- | :--- | :--- | :--- |
| `Bind for 0.0.0.0:8069 failed: port is already allocated` | El puerto 8069 estaba ocupado por otra instancia local de Odoo o contenedor previo. | Modificar el archivo `docker-compose.yml` para mapear el puerto al `8070:8069` o detener el servicio en conflicto. | [Documentación oficial de Docker / StackOverflow] |
| `psycopg2.OperationalError: FATAL: database "odoo" does not exist` | El contenedor de Odoo arrancó antes de que PostgreSQL terminara de inicializar la base de datos interna. | Configurar `depends_on` en el fichero de Docker Compose o reiniciar el contenedor de Odoo tras 15 segundos. | [Odoo Forums] |