# CSS - Cascada y Especificidad

CSS significa **Cascading Style Sheets** que en español es **Hojas de Estilo en Cascada**.

Esto significa que el orden de las reglas en CSS importa. Por ejemplo:

```css
/*  queda de azul  */
h1 {
  color: red;
}

h1 {
  color: blue;
}
```

# Navegadores y CSS

Los navegadores determinan qué reglas de CSS deben aplicarse a las etiquetas HTML.

El orden y el origen de clasificación del CSS, intervienen en este proceso.

# Conflicto de Reglas en CSS

Sin embargo, no todo es color de rosa. A veces los navegadores entran en conflicto porque no saben qué regla aplicar.

# Especificidad en CSS

Creo que estoy causando problemas así que yo solito buscaré una solución.

La **especificidad** de los selectores en CSS es cómo el CSS tiene una manera de lidiar con los conflictos.

# Especificidad en CSS

Entre mayor especificidad, mayor va a ser la probabilidad de que sus declaraciones se usen sobre las demás.

# ¿Cómo podemos saber qué reglas de CSS tienen mayor especificidad?

| Especificidad | Selector                          |
| ------------- | --------------------------------- |
| 1 0 0 0 0     | `!important`                      |
| 0 1 0 0 0     | Estilos en línea                  |
| 0 0 1 0 0     | `#id`                             |
| 0 0 0 1 0     | Clases, atributos y pseudoclases. |
| 0 0 0 0 1     | Elementos y pseudoelementos.      |
| 0 0 0 0 0     | Selector universal.               |

# calculadora de specificidad

https://specificity.keegan.st/
