# Bugis
Proyecto final realizado para el curso de JavaScript, brindado por Coderhouse. 
**Autor** Ariel Fumagalli / **Año** 2021



## Sobre el proyecto

El proyecto, surge a partir de la idea de crear una sección web interactiva, para una hipotética empresa dedicada a la venta de hamburguesas, cuyo principal diferencial y atractivo, es la venta de combos custom, es decir, que el usuario pueda armar su propio combo de la forma que lo desee, ya sea, desde elegir el tipo de pan, el tipo de carne, los agregados y aderezos, como así también el tipo de guarnición y bebida.



## Funcionalidad

El contenido de la sección, está estructurado y desarrollado con el fin de que entre todo dentro de la pantalla, sin que sea necesario que el usuario haga scroll o hayan diferentes páginas o pasos de por medio que afecten a la experiencia de usuario.

En cuanto a la etapa de armado del combo, la sección incluye un selector de categorías, para seleccionar la etapa de armado de la hamburguesa, un selector para seleccionar el tipo de guarnición y un selector para seleccionar la bebida.

Se utilizó Swiper (https://swiperjs.com/) para colocar cada ítem en una tarjeta dentro del carrusel, y de este modo generar una mejor experiencia de usuario y limpieza en el diseño, ya que ofrece la posibilidad de cargar una infinidad de productos y mostrarlos horizontalmente de a tres items por slide, y a su vez es compatible con mobile. 

Se incluyeron también botones de siguiente y anterior, para facilitarle el recorrido al usuario, y para el armado de la hamburguesa también se incluyó un selector con las categorias Pan, Carne, Agregados y Aderezos, que funciona como atajo, en caso que el usuario desee acceder directamente a una categoría sin necesidad de tener que llegar por medio del botón siguiente.

En cuanto al modo de visualización del combo, la sección incluye dos modos de visualización. Por un lado, se incluyó un bloque a la derecha en el cual se van imprimiendo en pantalla los nombres de los items seleccionados, acompañados del precio de cada uno, y a su vez, el precio final del total del combo, que resulta de la suma del precio de cada ítem.

En ese mismo bloque se incluye un botón para eliminar un tipo de agregado o aderezo seleccionado y a su vez un botón para eliminar por completo el combo y resetearlo.

Por otro lado, la sección incluye un bloque en el cual se va mostrando de manera visual como se va armando el combo, es decir, que a medida de que el usuario va seleccionando los diferentes ítems, se va armando visualmente la hamburguesa, luego se agrega la guarnición y finalmente la bebida. De este modo, se enrriquece la experiencia, y el usuario puede ver de una manera mas o menos aproximada el producto final, mas allá de ver el nombre y precio en pantalla.

Si bien el proceso de armado del combo es bastante libre, se incluyeron ciertas reglas pensadas estratégicamente y que hacen a la lógica y al funcionamiento general, y que son necesario cumplir para poder avanzar.

Por un lado, se utilizó el componente modal de Bootstrap (https://getbootstrap.com/docs/5.0/components/modal/) para mostrar determinados mensajes, en caso de que el usuario no seleccione un tipo de carne, guarnición o bebida y no lo deje continuar con el proceso.

También se los utilizó para mostrar un aviso en el caso de las secciones que no están disponibles, y para colocar los elementos que se encuentran dentro del carrito de compras y los pasos relacionados con la etapa de pago y finalización de la compra.



## Archivos

El proyecto cuenta con un archivo **index.html**, el presente archivo **README.md** y tres carpetas: **assets**, **js** y **style**.

La carpeta assets, incluye dos carpetas, una en donde se alojan las imágenes (img), en su mayoría en mapa de bits, y otra en donde se alojan los iconos en formato SVG (icon).

En la carpeta js, se pueden encontrar los diferentes archivos en JavaScript, utilizados en el proyecto.

**inventario.js** contiene el listado de productos dentro de una variable en formato JSON.

**funciones-generales.js** contiene algunas funciones generales, como por ejemplo realizar determinado efecto al abrir el modal de Bootstrap.

**imprimir-productos.js** contiene el código necesario para imprimir en el DOM, los productos que se encuentran en inventario.js

**selectores.js** contiene el código utilizado para generar la funcionalidad de los selectores que se utilizan en el armado del combo.

**armar-combo.js** contiene todo lo referente a la funcionalidad utilizada en la etapa de armado del combo y, a su vez, realizar modificaciones en el DOM.

**pedido.js** contiene el codigo utilizado para consolidar el combo generado por el usuario en un objeto, que luego se imprimirá dentro del carrito.

**pago.js** contiene el código utilizado en lo referente a la etapa de pago del pedido.

**formulario.js** contiene el código utilizado en el formulario que se encuentra dentro del modal, en la etapa de pago del pedido.

**swiper-initialize.js** contiene lo referente a la inicialización y configuración de swiper.js

En la carpeta style, se encuentran los archivos SCSS, en los cuales se trabajaron los estilos visuales del sitio, como así también las versiones compiladas a CSS y map, y el CSS utilizado por swiper.js

En **style.scss**, se encuentran los estilos generales del sitio, y en **combo.scss**, los estilos utilizados para generar visualmente el combo.



## Demo

Para ver el sitio de manera online y chequear el funcionamiento en dispositivos móviles, se puede acceder a la siguiente dirección: http://arielfumagalli.com/bugis/