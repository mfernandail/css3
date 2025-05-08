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