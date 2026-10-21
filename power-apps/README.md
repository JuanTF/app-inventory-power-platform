# Power Apps — AppInventory

Este directorio contiene los archivos **Power Fx / .pa.yaml** extraídos del archivo `.msapp` incluido en la exportación original de AppInventory. Se publican para poder revisar las fórmulas y la estructura de las pantallas sin exponer las referencias de conexión privadas del paquete original.

| Pantalla | Función principal |
| --- | --- |
| `ScrInicio.pa.yaml` | Inicio de sesión de prueba. |
| `ScrRegistro.pa.yaml` | Registro y solicitudes de acceso. |
| `ScrPrincipal.pa.yaml` | Consulta y búsqueda de productos, alerta de stock y actualización de BI. |
| `ScrNuevo.pa.yaml` | Formulario de nuevo producto. |
| `ScrDetalle.pa.yaml` | Visualización y edición de información. |
| `ScrDetalle_1.pa.yaml` | Confirmación / tratamiento de eliminación. |
| `App.pa.yaml` | Configuración general de la aplicación. |

**Nota:** Los `.pa.yaml` son una referencia técnica, no un archivo de instalación ni un paquete válido para importar directamente a Power Apps. La aplicación original requiere conexiones y configuración específicas de Microsoft 365. El proceso de autenticación utilizado es demostrativo y no debe reutilizarse en producción.
