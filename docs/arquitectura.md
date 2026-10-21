# Arquitectura y recorrido funcional

## Datos

- **Excel Online:** tablas `TblProductos` y `TblUsuarios` utilizadas como datos de demostración en la aplicación original. El archivo público incluye únicamente un libro de ejemplo anonimizado.
- **SharePoint:** lista `UserInventory` usada por el proceso de alta y aprobación de usuarios.
- **Power BI:** conjunto de datos conectado a los productos para presentar indicadores y detalle del inventario.

## Recorridos principales

1. **Consulta y mantenimiento de productos:** desde Power Apps se pueden buscar, ver, crear, editar y eliminar productos, con una confirmación de eliminación.
2. **Registro y aprobación:** un registro nuevo genera una solicitud en SharePoint; un flujo envía una solicitud de aprobación, cambia el estado del registro y notifica la decisión.
3. **Reposición:** un flujo programado consulta la tabla de productos y filtra `StockActual <= StockMinimo` para generar un correo de alerta.
4. **Actualización de reporte:** desde Power Apps se inicia un flujo que solicita una actualización del conjunto de datos de Power BI.
5. **Asistente:** Copilot Studio invoca un flujo que consulta productos en Excel Online, selecciona campos y devuelve la respuesta.

## Limitaciones de portabilidad

Los vínculos a conexiones y recursos específicos del entorno original no están incluidos en el repositorio público. Los componentes publicados son útiles para una revisión técnica, pero no conforman una solución lista para desplegar sin configuración.
