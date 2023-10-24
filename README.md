# api-geo
Creacion de ejemplo de utilizacion de apis de gogle maps

# ae instalan las bibliotecas
se utilizaran los siguientes comando 
$npm i @popperjs/core
&npm i bootstra

### 1. Index.html
En este archivo, se presenta la interfaz de la página web, que incluye referencias a la hoja de estilos, nuestro archivo JavaScript y elementos de Bootstrap. Al final del archivo, también se proporcionan las referencias necesarias para la integración y consumo de la API de Google Maps.

### 2. index.js
Se incorpora una función que define las características generales del mapa, incluyendo sus ajustes personalizados. Además, se introduce una constante llamada 'lugares', la cual alberga un arreglo de ubicaciones a ser mostradas en la página inicial, es decir, los nodos.

A continuación, se genera un nuevo mapa que incluye propiedades como el nivel de zoom y las coordenadas que establecen el centro de la Ciudad de Puebla.

"Posteriormente, se define una función llamada 'agregarMarcador' que toma tres parámetros: nombre, latitud y longitud. Dentro de esta función, se crea un nuevo objeto de marcador utilizando la clase 'google.maps.Marker', el cual representa un marcador en el mapa. Las coordenadas del marcador se establecen en la posición especificada, utilizando los valores proporcionados como argumentos de latitud y longitud.

Se asocia el marcador con el mapa mediante la propiedad 'map: mapa', indicando en qué mapa debe aparecer. Además, se permite que el marcador sea arrastrable con 'draggable: true', lo que permite al usuario hacer clic y arrastrar el marcador a una nueva ubicación en el mapa.

Se aplica un efecto de animación al marcador al agregarlo al mapa con 'animation: google.maps.Animation.DROP'. Además, se definen las propiedades del icono del marcador. La URL 'http://maps.google.com/mapfiles/ms/icons/blue-dot.png' especifica la imagen que se utilizará como icono, en este caso, un marcador azul de Google Maps. El tamaño del marcador se establece en 50x50 píxeles con 'scaledSize: new google.maps.Size(50, 50)'.

Luego, se muestra un fragmento de código con una imagen que podría representar un ejemplo del marcador configurado.

En otra sección del código, se presenta la función 'trazarRuta', que calcula y muestra una ruta en un mapa de Google Maps. Esta función utiliza los lugares de origen y destino proporcionados por el usuario a través de dos elementos con los IDs 'origenInput' y 'destinoInput'.

Se crean objetos para el servicio de direcciones y el renderizador de direcciones. El objeto 'directionsService' se utiliza para solicitar y calcular rutas, y el objeto 'directionsRenderer' se utiliza para mostrar la ruta en el mapa.

La ruta calculada se muestra en el mapa con 'directionsRenderer.setMap(mapa)'. Se utiliza 'directionsService.route(...)' para solicitar una ruta especificando el lugar de origen, el lugar de destino y el modo de viaje.

El tiempo estimado de viaje se muestra en un elemento con el ID 'tiempoViaje'. En caso de que no se pueda calcular la ruta, se muestra una alerta con un mensaje de error.

Finalmente, se limpian los campos de entrada después de calcular la ruta utilizando 'document.getElementById("origenInput")' y 'document.getElementById("destinoInput")'. La función se inicia mediante 'initMap();'."

Esta redacción ofrece una descripción más clara y organizada de las acciones y funciones en el código.



### 3. style.css
Encargado de brindar formatos y colores

### Recuerda que debes regentrar a Google Cloud para generar tu api key
Ademas de poder revisar la documentacion proporciona por google 




