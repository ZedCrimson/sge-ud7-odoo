# Proceso de Venta Completo (End-to-End)

1. **Creación del Presupuesto**
   - **Usuario:** `comercial@TecnoSalva.com` (Comercial)
   - **Referencia:** `S00001`
   - **Cliente:** Ayuntamiento Sevilla
   - **Líneas de producto (3 líneas):**
     - 2x Placa Base 
     - 1x Ratón Ergonómico
     - 1x Tableta Gráfica
   - **Plazo de pago:** 30 días. Fecha de validez: +15 días.
   - **Documento generado:** `presupuesto.pdf` (Guardado en `venta/presupuesto.pdf`).

2. **Confirmación del Pedido**
   - **Usuario:** `respventas@TecnoSalva.com` (Responsable de Ventas)
   - **Acción:** Conversión de presupuesto a pedido de venta confirmado.

3. **Validación de la Entrega en Inventario**
   - **Usuario:** `respventas@TecnoSalva.com` (o almacenero)
   - **Referencia de Albarán:** `1111111`
   - **Acción:** Validación de salidas de stock (Cantidad hecha = Cantidad pedida). Comprobación de que el stock de la batería y el teclado se redujo correctamente en el inventario.

4. **Facturación y Registro de Pago**
   - **Usuario:** `adminfactura@TecnoSalva.com` (Administración / Facturación)
   - **Referencia de Factura:** `INV/2026/00001`
   - **Acción:** Creación de la factura desde el pedido de venta, revisión, publicación y registro del pago completo.
   - **Documento generado:** `factura.pdf` (Guardado en `venta/factura.pdf`, con estado **Pagado**).