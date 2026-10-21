# Seguridad antes de publicar una versión pública

Este repositorio contiene una muestra preparada para portafolio. Al revisar los archivos originales se encontraron **datos de una cuenta en la tabla `Usuarios`**, incluidos una dirección de correo y un valor de contraseña de demostración, así como **direcciones de correo y referencias a SharePoint** dentro de los paquetes originales.

Para evitar publicarlos:

- Se sustituyó la cuenta del Excel por un usuario ficticio (`demo@example.com`) con contraseña `NO_CONFIGURADA`.
- Se regeneraron los identificadores de filas de demostración.
- Se publicaron fórmulas `.pa.yaml` en lugar del paquete original de Power Apps.
- Se publicaron definiciones de flujos redactadas en lugar de la solución exportada original.
- Se incluyó el diseño del reporte Power BI en JSON, no el `.pbix` con su modelo y fuentes.

## Precauciones

1. **No subas el `.rar` original, el `.xlsx.xlsx` original ni los paquetes `.zip`/`.pbix` originales** a un repositorio público sin una auditoría de datos y conexiones.
2. Si la contraseña de prueba del archivo original se reutiliza en algún servicio, cámbiala de inmediato. No uses contraseñas almacenadas como texto plano para autenticación real.
3. Al añadir nuevas capturas o exportaciones, verifica direcciones de correo, usuarios, enlaces internos, nombres y datos privados.
4. La eliminación posterior de un archivo en GitHub **no garantiza** eliminarlo del historial Git. Evita publicarlo desde el inicio.
5. No confundas los JSON redactados con paquetes importables: las conexiones deben configurarse en el entorno de destino.
