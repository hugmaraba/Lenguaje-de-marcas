# UD 2.1 - Ejercicio 4: Identificadores y atributos

## Parte A. Selector de id

### 1. Error por repetir un id

He asignado temporalmente el mismo id (`corp`) a dos elementos HTML y he validado la página con el validador W3C.

**Mensaje de error del validador:**

[Pega aquí el mensaje exacto que aparece en el validador.]

### 2. Corrección del error

He corregido el error cambiando el id del segundo elemento por una clase. De esta forma, el id `corp` solo aparece una vez en la página.

### 3. ¿Por qué se desaconseja utilizar selectores de id para estilizar?

Se desaconseja porque los selectores de id tienen una especificidad mayor que los selectores de clase y de tipo. Esto puede dificultar la modificación de los estilos cuando varias reglas afectan al mismo elemento. Además, un id no debe repetirse en una misma página, mientras que una clase se puede utilizar en varios elementos.

## Parte B. Selector de atributo

### 1. Enlaces con target

He utilizado el selector `a[target]` para cambiar el color de los enlaces que tienen el atributo `target`. Los enlaces sin ese atributo mantienen su estilo predeterminado.

### 2. Párrafos con class

He utilizado el selector `p[class]` para aplicar un fondo amarillo claro a los párrafos que tienen el atributo `class`. Los párrafos que no tienen ese atributo no reciben ese estilo.
