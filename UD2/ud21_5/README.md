# UD 2.1 - Ejercicio 5: Colisiones y refactorización

## Parte A. Detective de colisiones

### 1. Predicciones antes de abrir el navegador

| Elemento | Color previsto | Motivo |
|---|---|---|
| Hola CSS | Marrón | El selector `#titulo` tiene mayor especificidad que `h1` y `.grande`. |
| Texto 1 | Morado | `p.aviso` es más específico que `.aviso` y `p`. |
| Texto 2 | Negro | El selector `#importante` tiene mayor especificidad que `p.aviso`. |
| Texto 3 | Naranja | El selector `div p` es más específico que `p`. |

### 2. Comprobación con el inspector

He abierto la página en el navegador y he utilizado las herramientas de desarrollo (F12) para comprobar los colores.

| Elemento | Color final | Explicación |
|---|---|---|
| Hola CSS | Marrón | Gana `#titulo` por tener mayor especificidad. |
| Texto 1 | Morado | Gana `p.aviso` frente a `.aviso` y `p`. |
| Texto 2 | Negro | Gana `#importante` porque es un selector de id. |
| Texto 3 | Naranja | Gana `div p` frente a las reglas generales `p`. |

Las predicciones coinciden con los resultados obtenidos. La especificidad determina qué selector tiene prioridad cuando varias reglas modifican la misma propiedad. Si dos reglas tienen la misma especificidad, normalmente gana la última.

## Parte B. Refactorización

He creado una página de ejemplo llamada `refactorizada.html` y he trasladado sus estilos a un archivo externo llamado `refactorizada.css`.

He enlazado el CSS mediante la etiqueta `<link>` y he evitado utilizar atributos `style` en el HTML.

### Requisitos cumplidos

- **Agrupación de selectores:** he utilizado `.tarjeta, h1` para centrar ambos elementos.
- **Agrupación de declaraciones:** he incluido varias propiedades dentro de la regla `h1`.
- **Selectores de clase:** he utilizado `.tarjeta`, `.descripcion`, `.precio` y `.boton`.
- **Comentarios CSS:** he organizado las reglas en secciones mediante comentarios `/* ... */`.
- **CSS externo:** los estilos están separados del contenido HTML.

La refactorización permite mantener el HTML más limpio y modificar los estilos desde un archivo independiente.
