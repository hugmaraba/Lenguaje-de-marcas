
# UD 2.4 - Ejercicio Divs

## Parte A - Cajas visibles y centradas

He creado una página con una cabecera, un contenido y un pie de página.
He utilizado diferentes colores de fondo y bordes para distinguir
las cajas. La página tiene 800px de ancho y está centrada.

## Parte B - Display: de columna a fila

He utilizado display: flex para colocar las tres tarjetas
en una misma fila.

He elegido flex porque permite organizar las tarjetas fácilmente
y mantenerlas alineadas horizontalmente.

He cambiado el ancho de las tarjetas a 200px para que puedan caber
las tres en el espacio disponible.

## Parte C - Block, inline y none

He añadido una etiqueta llamada Nuevo dentro de la primera tarjeta.
He utilizado display: inline-block para que se apliquen
el ancho, la altura y los márgenes.

También he probado display: none en la tercera tarjeta.
Al utilizarlo, desaparece y las demás tarjetas ocupan su lugar.
Después he quitado esa regla.

## Preguntas

### 1. ¿Qué diferencia hay entre margin y padding?

El padding es el espacio interior entre el contenido y el borde.
El margin es el espacio exterior que separa una caja de las demás.

### 2. ¿Por qué saltaba la tercera tarjeta de línea?

Porque las tres tarjetas ocupaban más espacio del disponible.
Había que sumar el ancho, el padding, el borde y el margin.

### 3. ¿Qué propiedades ignoraba el span y por qué?

Ignoraba el ancho y la altura porque span es un elemento inline.
Al cambiarlo a inline-block, estas propiedades se aplican.

### 4. ¿Qué hace display: none con el espacio que ocupaba la caja?

Hace desaparecer el elemento y también elimina el espacio que ocupaba.
Las demás cajas aprovechan ese espacio.
