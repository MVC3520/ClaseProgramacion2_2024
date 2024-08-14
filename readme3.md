### Ejercicio 1: Posicionamiento Estático (Static Positioning)

**Descripción:** El valor `static` es el valor por defecto de la propiedad `position`. No afecta la posición del elemento, que permanece en el flujo normal del documento.

**Instrucciones:**

1. Crea un contenedor con tres elementos hijos.
2. Aplica `position: static` a uno de los elementos (aunque este es el valor predeterminado).

**Explicación:**
El elemento `Caja 2` tiene `position: static`, lo que significa que se comporta de manera normal, sin que su posición se vea afectada por el CSS. El resultado es que todos los elementos se apilan uno tras otro de acuerdo al flujo del documento.


### Ejercicio 2: Posicionamiento Relativo (Relative Positioning)

**Descripción:** El valor `relative` permite mover un elemento con respecto a su posición original en el flujo del documento usando las propiedades `top`, `bottom`, `left`, y `right`.

**Instrucciones:**

1. Crea un contenedor con tres elementos.
2. Aplica `position: relative` a uno de ellos y mueve su posición 20px hacia abajo.

**Explicación:**
El elemento `Caja 2` tiene `position: relative` y se desplaza 20px hacia abajo desde su posición original. Aunque su posición ha cambiado, todavía ocupa su espacio original, afectando el flujo del documento.


### Ejercicio 3: Posicionamiento Absoluto (Absolute Positioning)

**Descripción:** Con `position: absolute`, un elemento se posiciona respecto al contenedor más cercano con `position: relative`, `absolute`, o `fixed`. Si no hay un contenedor posicionado, se posiciona respecto al viewport.

**Instrucciones:**

1. Crea un contenedor con un `div` que tenga `position: relative`.
2. Coloca otro `div` dentro de este con `position: absolute` y posiciónalo en la esquina inferior derecha.

**Explicación:**
El `div` con clase `absoluta` se posiciona en la esquina inferior derecha del contenedor porque su `position` es `absolute` y el contenedor tiene `position: relative`. Si el contenedor no tuviera `position: relative`, el elemento se posicionaría respecto al viewport.


### Ejercicio 4: Posicionamiento Fijo (Fixed Positioning)

**Descripción:** El valor `fixed` mantiene el elemento en una posición fija dentro del viewport, incluso cuando se desplaza la página.

**Instrucciones:**

1. Crea un encabezado con `position: fixed` y haz que permanezca en la parte superior de la ventana del navegador al hacer scroll.

**Explicación:**
El `header` se mantiene en la parte superior de la pantalla incluso cuando el usuario hace scroll. Esto es útil para barras de navegación o encabezados persistentes.


### Ejercicio 5: Posicionamiento Sticky (Sticky Positioning)

**Descripción:** Con `position: sticky`, el elemento se comporta como `relative` hasta que se alcanza una posición específica en la página, momento en el cual se "pega" y se comporta como `fixed`.

**Instrucciones:**

1. Crea un encabezado que se "pegue" a la parte superior del viewport cuando el usuario haga scroll hacia abajo.

**Explicación:**
El `header` se comporta como un elemento `relative` hasta que el usuario hace scroll y el encabezado alcanza la parte superior del viewport. En ese momento, se "pega" a la parte superior y se comporta como `fixed`.


### Ejercicio 6: Página Web Completa con Posicionamiento Avanzado

**Descripción:**
Crear una página web que simule una estructura básica de un sitio, con un encabezado fijo, un menú de navegación, un contenido principal que incluye una sección de noticias con elementos posicionado de forma relativa y absoluta, una barra lateral fija, y un pie de página con posición estática. Además, una barra de navegación que se mantenga fija (sticky) al hacer scroll.

**Objetivos:**

* Utilizar diferentes valores de la propiedad `position` en distintos elementos.
* Implementar una estructura básica de página web con etiquetas HTML5.
* Hacer uso de CSS para crear una disposición visual coherente y funcional.


**Explicación:**

1. **Header (Encabezado):** El `header` está fijado en la parte superior de la página usando `position: fixed`. Esto significa que se mantiene visible incluso al hacer scroll.
2. **Nav (Navegación):** La barra de navegación utiliza `position: sticky`, lo que permite que permanezca en la parte superior de la ventana del navegador una vez que el usuario hace scroll más allá del encabezado.
3. **Main (Contenido Principal):** El `main` contiene dos elementos principales: `section` y `aside`. La `section` es donde se encuentran los artículos y contiene elementos posicionados de manera relativa y absoluta. El `aside` es una barra lateral que está fijada en la parte derecha de la pantalla, utilizando `position: fixed`.
4. **Relativo (Elemento Relativo):** Dentro del primer artículo, se ha posicionado un `div` de manera relativa (`position: relative`), moviéndolo 10px hacia abajo y 10px hacia la derecha.
5. **Absoluto (Elemento Absoluto):** Dentro del segundo artículo, se ha posicionado un `div` de manera absoluta (`position: absolute`), colocándolo en la esquina inferior derecha del contenedor `section`.
6. **Footer (Pie de Página):** El pie de página se coloca de forma estática al final del documento, sin ser afectado por el posicionamiento de otros elementos.

Este ejercicio avanzado combina diferentes valores de `position` para crear una página web funcional y dinámica. Puedes modificar y experimentar con los valores para comprender mejor cómo funciona cada tipo de posicionamiento.
