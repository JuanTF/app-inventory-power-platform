# Power Automate — Definiciones de flujos

Se publican **solo las definiciones JSON** de los cuatro flujos presentes en la solución original. Se retiraron los metadatos de conexión del entorno de origen y se sustituyeron las direcciones de correo y rutas personales de SharePoint por datos ficticios.

| Archivo | Disparador y propósito |
| --- | --- |
| `aprobacion-usuarios.json` | Al crearse un elemento en SharePoint, solicita aprobación, actualiza el estado y envía un correo al solicitante. |
| `alerta-stock-bajo.json` | Ejecución programada cada día, consulta productos y envía por correo aquellos con `StockActual <= StockMinimo`. |
| `actualizar-reporte-power-bi.json` | Invocado desde Power Apps, solicita actualización del conjunto de datos de Power BI y responde a la aplicación. |
| `consulta-inventario-agente.json` | Invocado por un agente, lee productos, selecciona campos y devuelve resultados. |

Estos archivos permiten **leer la lógica** de las automatizaciones; **no son paquetes importables** como una solución de Power Automate. Para ejecutar los flujos es necesario configurarlos en un entorno propio y reemplazar conexiones, identificadores de recursos y destinatarios.
