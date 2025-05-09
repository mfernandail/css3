# CSS

## Selectores:
| Selector                   | Nombre                   | Qué hace                                                                 | Ejemplo                                                                 |
|----------------------------|--------------------------|--------------------------------------------------------------------------|-------------------------------------------------------------------------|
| `padre > hijo`             | Hijo directo             | Selecciona solo los hijos **directos** del elemento padre.               | `div > p` selecciona `<p>` dentro de `<div>`                           |
| `elemento:first-child`     | Primer hijo              | Selecciona el **primer hijo** si coincide con el tipo especificado.      | `p:first-child` si el `<p>` es el primer hijo de su padre              |
| `elemento:first-of-type`   | Primer hijo del tipo     | Selecciona el **primer hijo de su tipo**, aunque no sea el primero.      | `p:first-of-type` selecciona el primer `<p>` entre varios hermanos     |
| `elemento1 + elemento2`    | Hermano siguiente        | Selecciona el hermano **inmediato** que sigue a `elemento1`.             | `h1 + p` selecciona `<p>` justo después de un `<h1>`                   |
| `elemento1 ~ elemento2`    | Hermanos siguientes      | Selecciona **todos los hermanos** que siguen a `elemento1`.              | `h1 ~ p` selecciona todos los `<p>` que siguen a un `<h1>`             |



## Display

### 🧱 Valores de `display` en CSS

| `display`         | Descripción breve                                                                 |
|-------------------|----------------------------------------------------------------------------------|
| `block`           | Ocupa todo el ancho disponible. Inicia en una nueva línea. Ej: `<div>`, `<p>`.   |
| `inline`          | No inicia en una nueva línea. Solo ocupa el ancho necesario. Ej: `<span>`, `<a>`.|
| `inline-block`    | Como `inline`, pero permite modificar ancho y alto.                              |
| `none`            | Oculta el elemento completamente (no se muestra ni ocupa espacio).               |
| `flex`            | Crea un contenedor flexible para alinear hijos (horizontales o verticales).     |
| `inline-flex`     | Igual que `flex`, pero en línea.                                                 |
| `grid`            | Crea una cuadrícula para organizar elementos en filas y columnas.               |
| `inline-grid`     | Igual que `grid`, pero en línea.                                                 |
| `table`           | Se comporta como una tabla HTML.                                                 |
| `table-row`       | Se comporta como una fila de tabla.                                              |
| `table-cell`      | Se comporta como una celda de tabla.                                             |
| `list-item`       | Elemento de lista. Muestra viñetas o números. Ej: `<li>`.                        |
| `contents`        | No genera caja para el elemento, pero sí muestra los hijos.                     |
| `inherit`         | Hereda el valor de su elemento padre.                                            |
| `initial`         | Restaura al valor por defecto definido por el navegador.                         |
| `unset`           | Hereda si es heredable, si no, aplica `initial`.                                |


## unidades de medida

### 📏 Unidades de medida en CSS

| Unidad  | Tipo       | Basado en...                                      | Ejemplo        | Comentario útil                                             |
|---------|------------|---------------------------------------------------|----------------|-------------------------------------------------------------|
| `px`    | Absoluta   | Píxeles de la pantalla                            | `16px`         | Fijo. No escala con el tamaño del texto del usuario.        |
| `%`     | Relativa   | Tamaño del elemento padre                         | `50%`          | Muy útil en diseños fluidos y responsivos.                  |
| `em`    | Relativa   | Tamaño de fuente del elemento **padre**           | `1.5em`        | Escala según el contenedor. Puede acumularse.              |
| `rem`   | Relativa   | Tamaño de fuente del **root** (`html`)            | `1rem`         | Más predecible que `em`. Ideal para diseño escalable.      |
| `lh`    | Relativa   | Altura de línea (`line-height`) del elemento      | `1lh`          | Muy útil para espaciado vertical en tipografía fluida.     |
| `vw`    | Relativa   | 1% del ancho de la ventana del navegador          | `50vw`         | Cambia con el tamaño de la ventana (viewport).             |
| `vh`    | Relativa   | 1% del alto de la ventana del navegador           | `100vh`        | Muy útil para secciones de pantalla completa.              |
| `vmin`  | Relativa   | 1% del valor menor entre `vw` y `vh`              | `10vmin`       | Escala proporcional al lado más corto del viewport.         |
| `vmax`  | Relativa   | 1% del valor mayor entre `vw` y `vh`              | `10vmax`       | Escala proporcional al lado más largo del viewport.         |
| `ch`    | Relativa   | Ancho del caracter "0" en la fuente actual        | `40ch`         | Útil para definir anchos de texto (p. ej. 60 caracteres).   |
| `ex`    | Relativa   | Altura de la letra "x" en la fuente actual        | `1ex`          | Menos usada, varía según la fuente.                         |
| `cm`, `mm`, `in` | Absoluta | Medidas físicas (centímetros, milímetros, pulgadas) | `2cm`, `1in` | Poco prácticas en pantallas, más útiles en impresión.      |

## 🧠 Mejores prácticas generales
1. Usa rem para la base tipográfica → así puedes cambiar todo el diseño desde una sola regla en html (ej: html { font-size: 16px; }).
2. Evita px para texto o espaciado si te importa la accesibilidad.
3. Usa em dentro de componentes pequeños si quieres que se escalen localmente.
4. Para diseños fluidos, mezcla rem + % + vw/vh dependiendo del caso.