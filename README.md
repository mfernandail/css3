# CSS

## Selectores:
| Selector                   | Nombre                   | Qué hace                                                                 | Ejemplo                                                                 |
|----------------------------|--------------------------|--------------------------------------------------------------------------|-------------------------------------------------------------------------|
| `padre > hijo`             | Hijo directo             | Selecciona solo los hijos **directos** del elemento padre.               | `div > p` selecciona `<p>` dentro de `<div>`                           |
| `elemento:first-child`     | Primer hijo              | Selecciona el **primer hijo** si coincide con el tipo especificado.      | `p:first-child` si el `<p>` es el primer hijo de su padre              |
| `elemento:first-of-type`   | Primer hijo del tipo     | Selecciona el **primer hijo de su tipo**, aunque no sea el primero.      | `p:first-of-type` selecciona el primer `<p>` entre varios hermanos     |
| `elemento1 + elemento2`    | Hermano siguiente        | Selecciona el hermano **inmediato** que sigue a `elemento1`.             | `h1 + p` selecciona `<p>` justo después de un `<h1>`                   |
| `elemento1 ~ elemento2`    | Hermanos siguientes      | Selecciona **todos los hermanos** que siguen a `elemento1`.              | `h1 ~ p` selecciona todos los `<p>` que siguen a un `<h1>`             |