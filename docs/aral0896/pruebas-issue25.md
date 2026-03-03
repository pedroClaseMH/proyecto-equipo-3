# Pruebas para Issue #25 - Página HTML de Prueba

## Pruebas de Caja Blanca (Internas: Revisión del código fuente)
| Nº | Descripción | Entrada (Parte del código) | Salida Esperada | Resultado | Notas |
|----|-------------|----------------------------|-----------------|-----------|-------|
| 1  | Verificar DOCTYPE y meta tags | Líneas iniciales: <!DOCTYPE html>, <meta charset="UTF-8">, etc. | Presentes y correctos para compatibilidad | Pasa | Estructura válida, sin errores de sintaxis. |
| 2  | Validar CSS en <style> | Reglas como body { font-family: ... }, header { border-bottom: ... } | Sintaxis correcta, no conflictos | Pasa | Chequeado manualmente, estilos aplican sin problemas. |
| 3  | Chequear tags semánticos y lista añadida | <main>, <section>, <ul> en consejos | Tags cerrados, anidamiento correcto, lista con <li> válida | Pasa | Nueva sección integrada sin romper el código. |
| 4  | Verificar footer y copyright | <footer> con <p>&copy; 2026 - ...</p> | Presente y sin typos | Pasa | Todo OK. |

## Pruebas de Caja Negra (Externas: Como usuario final, sin ver código)
| Nº | Descripción | Entrada (Acción en browser) | Salida Esperada | Resultado | Notas |
|----|-------------|------------------------------|-----------------|-----------|-------|
| 1  | Cargar la página | Abrir archivo HTML en browser (Chrome/Firefox) | Contenido visible, header y secciones renderizadas con estilos | Pasa | Carga instantánea, sin errores en consola (presiona F12 para ver). |
| 2  | Verificar responsividad | Redimensionar ventana a ancho móvil (<600px) | Layout se adapta, texto no se desborda, viewport funciona | Pasa | Probado en modo desarrollador del browser. |
| 3  | Chequear visual de contenido | Scroll y ver secciones, lista de consejos | Todo legible, colores y padding correctos, sin elementos rotos | Pasa | Nueva lista se muestra bien estilizada. |
| 4  | Probar en diferentes browsers | Abrir en Edge o otro | Mismo renderizado sin variaciones | Pasa | Compatible. |
| 5  | Probar en modo oscuro del navegador | Activar modo oscuro en Chrome/Edge | La página se ve correctamente (colores legibles) | Pasa | Se adapta bien al tema del sistema. |