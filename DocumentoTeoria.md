# HTML y CSS

## HTML

### Estructura HTML

<head> Es la etiqueta que indica el bloque o conjunto de cosas que se deben cargar primero en la pagina</head>

<meta nos sirve para especificaciones de la web (escala de la web o codificación de caracteres UTF-8)> (Dentro del contenido de head)

<body>  Contiene todo el cuerpo o maquetado de la web </body>

<title>Es únicamente para el titulo de la web</title>

<html>Etiqueta global</html>

#### Tipos de etiquetas

Autocontenidas: <meta name> nos especifica el nombre de la etiqueta, no tiene cierre y los atributos de la etiquetan están dentro de la misma etiqueta.

Contenedoras: <body>Tienen una apertura y un cierre, conteniendo en este espacio lo que se </body>. Así mismo las etiquetas contenedoras también tiene que poner sus atributos en la etiqueta de apertura.

#### Etiquetas

<h1→h6> Son títulos de texto del 1 al 6 cada número especifica un tamaño de letra en decremento desde el 1 al 6  siendo el 6 el titulo más pequeño </h1→h6>

<p> Párrafo de texto principal </p>

<span> texto secundario no reconocido como párrafo principal, puede estar contenido en la etiqueta <p> </span>

<ol> estructura para una lista ordenada <li>etiqueta para cada punto de la lista</li> cada punto estará numerado </ol>

<ul>estructura para una lista no ordenada <li>etiqueta para cada punto de la lista</li> cada punto tendrá una viñeta o punto</ul>

<!—  —> Esta es la etiqueta para comentarios.

<a target = “_blank” href=”URL A OTRA DIRECCIÓN”> esta etiqueta es para  redireccionamiento url, el atributo href es para contener la url de direccionamiento el atributo. El atributo target blank nos permite que la url se abra en una nueva pestaña </a> la diferencia en etiquetas a son la absolutas las cuales son urls externas a nuestro programa y las relativas son rutas de nuestra misma web o proyecto

<img src=”ruta de la imagen (url web o ruta de archivo)” width=”define el ancho de la imagen” alt=”Texto en caso de que la imagen no cargue en la web”>  

<form>etiqueta general para formularios</form>

<label>Etiqueta usada para dar la el nombre o descripción de un input</label>

<input type=”define el tipod e variable de entrar” placeholder=”espacio de texto en forma de ejemplo para la entrada de datos.”>

## CSS

Para indicar el stilo css existen 3 formas, forma lineal en donde se pone el atributo style en la etiqueta que queremos cambias, forma interna usamos la etiqueta style para poner los estilos indicando la etiqueta que queremos asignarle el estilo y forma externa contralando en un archivo externo.

Fuente:

- Propiedades de texto
    - Color, es para cambiar el color de texto.
        - Ejemplo: [color: #FFF] [color rgb o rgba (255,255,255,0-1 opacidad)]
    - Font-family, asignar el tipo de letra para la web.
        - Ejemplo:  font-family: se asigna un tipo de letra principal y seguido de comas los que deberian estar disponibles en caso de que el navegador no soporte el tipo de letra.
    - Font-size, tamaño de la letra espesificado en pixeles.
        - Ejemplo: font-size: 16px
    - Font-weight, grosor de la negrita
        - Ejemplo: font-weight: bold (o usar porcentajes de negrita)
    - Line-height: espaciado entre líneas de parrafos
        - Ejemplo: line-height: “cantidad de espacio entre líneas de texto, 2”
    - letter-spacing: espaciado entre letras
        - Ejemplo: letter-spacing: “cantidad de espacio en px 10px”
    - text-aling: lineamiento del texto.
        - Ejemplo: tiene 7 alineaciónes pero por ejemplo center es para centrar y justify para justificar el texto.
- Formateo de pagina
    - Para cambiar propiedades del HTML a nivel general debemos encerar las propiedades dentro de <u>***{”porpiedades generales”},**</u> normalmente al formatear una pagina se manda el padding, el margin y el box-sizing a 0. quitando estas 3 capas.
    - padding: el espació entre el contenedor y su contenido (es como un relleno para empujar el contenido hacia dentro)
    - margin: es el espació entre los contenedores especificado en px
- Propiedades de contenedores
    - border-radius: darle curvatura a las esquinas de un contenedor
        - Ejemplo: border-radius: 10px 10px 10px 10px
    - border: asignarle un color, estilo de borde y grosor en px
        - Ejemplo: border: red 2px dashed
    - backgraund-color: darle color al fondo de un contenedor
    
    #### Organización de contenido
    
    - display: flex: propiedad para entender en que sentido se mostrará el diseño de la pagina.
    - flex-direction: especifica la dirección de la flexibilidad del contenido
    - Gap: espaciado entre contenedores (”separación”)
    - aling-items: especificar ubicación del contenido de arriba a abajo
    - justify-content: especificar ubicación del contenido de izquierda a derecha
    - position: relative: esta propiedad permite liberar el contenido del contenedor.
    - position: absolute: para usar la posision absoluta en un hijo debe existir un padre relativo, con esto podemos lograr que el hijo se adapte al tamaño cambiante del padre.
    - flex-warp: si el contenido no entra en una row pasará el contenido a la siguiente row.
    
    #### Maquetado web
    
    - display: grid: red de organización donde dividiremos el espació de la pagina web.
    - grid-template-areas: aqui se espesifica la estructura que tendran las areas asignadas en las clases usando el las etiquedas asignadas con grid-area.
        - Ejemplo: “Header Header Header”
        - Ejemplo: “Nav Main Slidebar”
        - Ejemplo: ”Footer Footer Footer”
    - grid-area: “etiqueta para identificar el area”
    - grid-template-rows: especificamos el tamaño de cada fila.
        - Ejemplo: grid-template-rows: 80px 1fr 80px
        - En este ejemplo estamos especificando que la primera fila ocupará 80px de la pagina, la segunda fila ocupara todo el espacio sobrante de la pagina y que la tercera fila ocuará 80px de la pagina.
    - grid-template-colums: sirve exactamente para lo mismo que grid-template-rows pero para las columnas.
- Estados
    - &: para empezar a usar un estado tenemos que definirlo con “&:”
    - &:hover: este es el estado cuando el mouse esta encima del contendedor donde se defina. y accionará las propiedades que se definan dentro del estado.
    - &:active: este estado es cuando se le da click al contenedor accionando las propiedades cuando se cliquee el contenedor.
- Diseño responsive
    - @media (”se debe definir el tamaño”){ dentro definimos las propiedades del contenedor cuando la pagina tenga este tamaño }
    - (min/max)-width: es para definir el tamaño de para @media min significa que apartir de ese tamaño o más y max significa que usará ese media hasta que llegue al tamaño indicado.
        - Ejemplo: @media(min-width: 576px) esto nos indica que usará las propiedades cuando el tamaño del dispositivo o el navegador lleguen a 576px
        - Ejemplo: @media(max-width: 575px) esto nos indica que estará usando las propiedades hasta que el tamaño del dispositivo o el navegador lleguen a 575px
- Animación
    
    Cuando tenemos un estado de cambio podemos darle un suavizado o tiempo de ejecución con transition.
    
    - transition: especificamos la transición o para todas poner all, el tiempo de ejecución y la forma de la transición [cubic-bezier.com/](http://cubic-bezier.com/) (URL para generar tiempos de movimiento es la forma enq ue se va a mover la transición en un hover) ejemplo: transition: “transiciones afectadas” “tiempo efectivo” “tipo de transición (cubic-bezier(0,-1.88,1,1.78))”
    - transition-delay: permite definir un tiempo de espera previa a una transición
    
    la estructura de animaciones es @keyframes “nombre de la animación” y dentro de {pondremos los porcentajes donde estaran los cambios de transición}
    
    - animation: “nombre de la animación” duración de la animación infinite, esto es para definir que objeto o contenedor realizara la animación creada.
    - 0 - 100%: podremos usar estos porcentajes para especificar el comportamiento de la animación.
    - movimiento: left, right, top, bottom especificado en pixeles el movimiento de la animación.
    - rotación: transform: rotate(0deg - 360deg) el objeto rotará.
    -