# [SmileMe](https://app-smileme.herokuapp.com/)
#### Proyecto para la asignatura de Implementación e Implantación de Sistemas Software

### Integrantes del grupo:
+ Felipe Bedoya Castaño
+ Manuel Bonat Lucia
+ Salvador Carmona Román

## Documentación

## Índice de contenidos
#### <a href="#lnk1">1.Introducción</a>
#### &nbsp;&nbsp;&nbsp;&nbsp;<a href="#lnk1.1">1.1 Motivación</a>
#### &nbsp;&nbsp;&nbsp;&nbsp;<a href="#lnk1.2">1.2 Descripción del sistema</a>
#### <a href="#lnk2">2.Planteamiento</a>
#### &nbsp;&nbsp;&nbsp;&nbsp;<a href="#lnk2.1">2.1 Organización de tareas</a>
#### &nbsp;&nbsp;&nbsp;&nbsp;<a href="#lnk2.2">2.2  Etapas de ejecución del proyecto</a>
#### &nbsp;&nbsp;&nbsp;&nbsp;<a href="#lnk2.3">2.3 Sistemas para el desarrollo de la aplicación web</a>
#### <a href="#lnk3">3. Requisitos y análisis</a>  
#### &nbsp;&nbsp;&nbsp;&nbsp;<a href="#lnk3.1">3.1  Requisitos funcionales</a>
#### &nbsp;&nbsp;&nbsp;&nbsp;<a href="#lnk3.2">3.2  Requisitos no funcionales</a>   
#### <a href="#lnk4">4. Despliegue</a>
#### <a href="#lnk5">5. Automatización de tareas</a>
#### &nbsp;&nbsp;&nbsp;&nbsp;<a href="#lnk5.1">5.1 Compilación automática de less a css</a>
#### &nbsp;&nbsp;&nbsp;&nbsp;<a href="#lnk5.2">5.2 Concatenación de css y javascript</a>
#### &nbsp;&nbsp;&nbsp;&nbsp;<a href="#lnk5.3">5.3 Minificación de css y javascript</a>
#### <a href="#lnk6">6. Pruebas</a>
#### &nbsp;&nbsp;&nbsp;&nbsp;<a href="#lnk6.1">6.1 Pruebas unitarias</a>
#### &nbsp;&nbsp;&nbsp;&nbsp;<a href="#lnk6.2">6.2 Pruebas de integración</a>
#### &nbsp;&nbsp;&nbsp;&nbsp;<a href="#lnk6.3">6.3 Pruebas de verificación html y css</a>  
#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#lnk6.3.1">6.3.1 Verificación HTML</a>
#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#lnk6.3.2">6.3.2 Verificación CSS</a>
#### <a href="#lnk7">7. Bibliografía</a>

----------------------------------------------------------------------------------

## Historial de cambios

 * 03-02-2015   v0.7.0   Despliegue en Heroku.
 * 01-02-2015   v0.6.0   Pruebas unitarias, correción de diseño, inclusión de servicios  ofertados, galeria.
 * 21-01-2015   v0.4.0   Automatización de tareas.
 * 14-01-2015   v0.3.0   Uso de plantilla.
 * 07-01-2015   v0.2.0   Persistencia, información se guarda en base de datos.
 * 27-12-2014   v0.1.1   Inyección de vistas, formulario.
 * 03-12-2014   v0.1.0   Comienzo del proyecto, trabajo en progreso.
 
 ------------------------------------------------------------

#### <a name="lnk1">1. Introducción</a>

SmileMe está formado por un grupo de jóvenes con muchas ganas de hacer reír a los niños. Este grupo trabaja en comuniones, reuniones, fiestas, etc. Siempre estando relacionado con la animación infantil y deportiva.

#### &nbsp;&nbsp;&nbsp;&nbsp;<a name="lnk1.1">1.1 Motivación</a>

>Ofrecer un portal web elegante y vistoso que permita consultar sobre los servicios que SmileMe oferta y acceder a estos de una manera fácil y rápida para los clientes. Ya sea recorriendo el catálogo de servicios o enviando una pregunta directamente.

#### &nbsp;&nbsp;&nbsp;&nbsp;<a name="lnk1.2">1.2 Descripción del sistema</a>

>Aplicación web que dará información sobre los servicios ofrecidos por la empresa Smileme, con la posibilidad de que el sistema pueda poner en contacto al cliente con la empresa Smileme.

#### <a name="lnk2">2.Planteamiento</a>

#### &nbsp;&nbsp;&nbsp;&nbsp;<a name="lnk2.1">2.1 Organización de tareas</a>

>El reparto de tareas se ha realizado de la manera más equitativa posible. A continuación se detalla dicho reparto:

>**Salvador Carmona**: coordinación general. Persistencia del sistema, implementando el almacenamiento de información en base de datos. Desarrollo general de HTML, CSS y Javascript. Implementación y prueba  de automatización de tareas. Redacción de documentación.

>**Felipe Bedoya**:  Desarrollo general de HTML, CSS y Javascript. Aportación de contenido a la web, servicios de la empresa, imágenes, diseño de vistas. Redacción de documentación. Despliegue de la aplicación web sobre Heroku.

>**Manuel Bonat**: Desarrollo general de HTML y Javascript. Implementación del sistema de vistas. Implementación y prueba de automatización de tareas. Implementación de pruebas unitarias. Redacción de documentación.

#### &nbsp;&nbsp;&nbsp;&nbsp;<a name="lnk2.2">2.2  Etapas de ejecución del proyecto</a>

>**Entrevista con el cliente**: antes de hacer nada, se realizó una entrevista al cliente con la que poder determinar los requisitos que tendría que cumplir la web.

>**Redacción de una primera versión de la documentación**: esta versión contiene una serie de requisitos iniciales, recogidos de la entrevista.

>**Determinar el reparto de tareas**: entre los integrantes del grupo se debatió qué tareas le corresponden a cada uno.

>**Determinar herramientas a usar**: Se eligieron las herramientas aprendidas en clase como Yeoman, Heroku, NodeJS, AngularJS, etc.

>**Comienzo del desarrollo de la web**: gracias a Yeoman el inicio del desarrollo fue cómodo y pudimos concentrarnos en añadir contenido y cumplir con los requisitos iniciales. Primero se implementó el formulario de la sección contacto seguido del sistema de vistas mediante el uso de Angular.

>**Implementación de la persistencia**: Para almacenar los mensajes de contacto se utilizó formato json para estructurar los datos y una base de datos no relacional, en nuestro caso, hemos usado MongoDB y el servicio en la nube de MongoLab para su gestión.

>**Cumplir nuevos requisitos**: el cliente nos pidió requisitos adicionales, tales como banners en la página de inicio. Se optó por utilizar una plantilla de Bootstrap que nos permitiría tener un Responsive Design y un slider o carousel en la página principal, además de un aspecto minimalista y moderno. Todo esto acompañado de la redacción de una nueva versión de la documentación.

>**Automatización de tareas**: Grunt nos permite automatizar tareas tales como la compilación de archivos .less a .css o la minificación de archivos CSS, para ello tuvimos que recurrir a varias páginas con información sobre la configuración del archivo Grunfile.js y búsqueda de librerías para dichas funcionalidades.

>**Pruebas unitarias**: Implementación de pruebas para comprobar la corrección de los patrones que validan si una consulta del formulario es válida o no. Se usó Karma y su plugin Jasmine.

>**Despliegue en servidor**: Se usa Heroku para el despliegue de la web y poder hacer así la prueba en un servidor.
    
>**Validación de HTML y CSS**: Comprobación de que el código se ciñe a los estándares.

#### &nbsp;&nbsp;&nbsp;&nbsp;<a name="lnk2.3">2.3 Sistemas para el desarrollo de la aplicación web.</a>

>Para el desarrollo del proyecto se ha utilizado la herramienta de ensamblaje Yeoman, compuesto por tres tipos de herramientas:

>>Yo: Proporciona herramientas de scaffolding.

>>Grunt: Para la ejecución de tareas, construcción, previsualización, y probar los avances del proyecto, además de la automatización de tareas.

>>Bower y nmp: Administradores de paquetes, dependencias de la página.

>Para el desarrollo del código HTML nos hemos ayudado del framework AngularJS, que ayuda a la legibilidad y mejora del código.

>Para la creación y manejo de base de datos instalamos MongoDB packages mediante la terminal.

>Para el despliegue de la aplicación sobre Heroku, se necesitaba instalar heroku toolbelt mediante la terminal.

>Además de esto, los integrantes del equipo de desarrollo del proyecto, han usado el programa Brackets con el plugin de git para actualizar los cambios en el repositorio alojado en GitHub.

>Todo el equipo trabajó sobre un sistema operativo Linux.

#### <a name="lnk3">3. Requisitos y análisis</a>
#### &nbsp;&nbsp;&nbsp;&nbsp;<a name="lnk3.1">3.1 Requisitos funcionales</a>

>Página de bienvenida
>>En esta página se mostrará a grandes rasgos los servicios ofrecidos por SmileMe, además de la experiencia y calidad que los avala. Por otro lado, se da la bienvenida y se invita al visitante a que explore el sitio web por sus distintas secciones.

>Sección de contacto
>>Página compuesta por un formulario a rellenar para la consulta de información concreta.

>Sección de galería
>>Página para mostrar los trabajos llevados a cabo por SmileMe con fotografías de las actividades.

>Sección acerca de
>>Página dónde se muestra la historia de SmileMe y su trayectoria profesional.

>Sección servicios
>>Conjunto de páginas donde se informa de los distintos servicios ofrecidos al público.

>>Dichos servicios son:
>>>+ Cumpleaños y comuniones
>>>+ Alquiler de material
>>>+ Excursiones

#### &nbsp;&nbsp;&nbsp;&nbsp;<a name="lnk3.2">3.2 Requisitos no funcionales</a>

>**Minificación de recursos**
>>Se ha minificado los recursos javascript y css para que el tiempo de carga sea el menor posible.

>**Framework Javascript**
>>Se ha usado el framework javascript AngularJS para el desarrollo de la aplicación web.

>**Framework CSS**
>>Se ha usado el framework Bootstrap 3 para ofrecer un diseño más profesional y actual al sitio web.

>**Responsive Design**
>>Se ha utilizado el Grid System de Bootstrap 3 para adaptar la visibilidad del sitio a todo tipo de dispositivos, PCs, tablets o móviles.

#### <a name="lnk4"> 4. Despliegue </a>

>Para el despliegue de la web usamos Heroku. A continuación, se detallan los pasos que fueron necesarios seguir para el correcto funcionamiento.

>**Primer paso.**
Para subir nuestra aplicación Angular a Heroku tuvimos la necesidad de añadir las siguientes dependencias para el servidor: Gzippo, Morgan, and Express

>Pues bien, instalamos mediante nuestra terminal las dependencias con el comando:
	
>>		npm install gzippo express morgan --save

>Una vez instaladas, el siguiente paso es crear un fichero para el servidor en el directorio raíz, a este fichero
le daremos el nombre, por ejemplo, de web.js. El contenido de este fichero es básico:

>>    
    var gzippo = require('gzippo');
    var express = require('express');
    var morgan = require('morgan');
    var app = express();
>>
    app.use(morgan('dev'));
    app.use(gzippo.staticGzip("" + __dirname + "/dist"));
    app.listen(process.env.PORT || 5000);


>Una vez que hemos creado el fichero para el servidor, nosotros necesitamos que grunt nos construya el directorio /dist
para ello usaremos en nuestra consola de comando y estando sobre nuestro proyecto, en este caso realizado con Yeoman, el siguiente comando:

>>				grunt build

>Con esto, grunt creará la carpeta /dist con el contenido de nuestra aplicación a desplegar en Heroku.

>**Segundo paso.**
Esto es algo que en nuestro caso no nos ocurrió, pero había que comprobarlo. Por defecto en el fichero oculto .gitignore puede incluirse el directorio dist, si es así, deberemos borrarlo del fichero ya que Heroku usa el
protocolo git para el despliegue. Guardar los cambios y cerramos.

>Ahora abrimos de nuevo un terminal y entramos en la carpeta de nuestro proyecto y creamos un repositorio git, haciendo
uso del comando:
>>				git init

>Además de un repositorio git necesitamos crear un Procfile, que Heroku utiliza para comprender cómo iniciar la aplicación. Pues bien, creamos en el direcorio raíz el Procfile al igual que hicimos con web.js, e incluímos la siguiente línea:

>>				web: node web.js

>Cerramos y guardamos.

>**Tercer Paso.**
El siguiente paso es crear nuestra aplicación Heroku. Es importante saber que debemos tener creada una cuenta en Heroku
y tener instalado el Heroku Toolbelt. Si tenemos todo, ejecutamos la linea de comando en nuestra terminal

>>				Heroku login


>y se nos pedirá nuestro email y contraseña para identificarnos en Heroku. Una vez identificados ejecutamos

>>				heroku create app_nombre

>donde "app_nombre" lo sustituiremos por el nombre de nuestra app.


>**Cuarto Paso.**
Ahora el siguiente paso es realizar un commit the todo el codigo y hacer un push en Heroku. Ejecutamos los siguientes
comandos:

>>			git add .

>>			git commit -m "Creación de app angular para el proyecto de ISS"

>>			git push heroku master



>Una vez que git y el servidor de realizar sus operaciones necesitamos al menos un proceso de Heroku que nos de servicio para ejecutar la aplicación, esto lo haremos con el siguiente comando:

>>				Heroku ps:scale web= 1

>Una vez hecho esto, nuestra aplicación debería estar ejecutandose sobre la dirección app_nombre.herokuapp.com

>Para comprobarlo, basta con ejecutar desde la terminal el comando:

>>				heroku open

>Entonces se nos abre una ventana del navegador y podremos ver nuestra aplicación desplegada sobre Heroku.

#### <a name="lnk5">5. Automatización de tareas</a>

>Se ha utilizado la herramienta Grunt para la automatización de tareas que se detallan a continuación.
    
#### &nbsp;&nbsp;&nbsp;&nbsp;<a name="lnk5.1">5.1 Compilación automática de less a css</a>

>Se ha usado un preprocesador CSS llamado less para la personalización del framework css Bootstrap 3, mediante el cual se compila los ficheros fuente en formato less de Bootstrap 3 junto con los ficheros de personalización.

>Para automatizar esta tarea, para que cada vez que se produzca un cambio en algún fichero less se compile automáticamente para generar los ficheros css correspondientes, se ha utilizado la biblioteca grunt-contrib-less.

#### &nbsp;&nbsp;&nbsp;&nbsp;<a name="lnk5.2">5.2 Concatenación de css y javascript</a>

>La idea ha sido mantener todos los recursos css y javascript en la menor cantidad posible de ficheros. Por tanto, se ha optado por unificar, tanto por un lado los ficheros css referente a bootstrap y su personalización, como por otro lado, los ficheros javascript referente a la aplicación en angularjs junto a sus controladores, en un único fichero.

>Para automatizar esta tarea, se ha definido en el fichero Gruntfile.js para que cuando se produzca un cambio en los ficheros css o cuando se ejecuta la orden build, se lleve a cabo la unificación. Se ha utilizado la biblioteca grunt-contrib-concat.

#### &nbsp;&nbsp;&nbsp;&nbsp;<a name="lnk5.3">5.3 Minificación de css y javascript</a>

>Para un entorno de desarrollo, tanto los ficheros css y javascript se usan siguiendo una estructura legible para que sea más sencillo su edición, pero para un entorno de producción, lo interesante es que dichos recursos ocupen la mínima cantidad de recursos posible para conseguir que el tiempo de carga del sitio web sea el mínimo posible, además de que en este entorno la legibilidad del código no es tan importante.

>Por ello, se ha automatizado una tarea para que una vez se ha compilado los ficheros less a css, se han unificado tanto los ficheros css como javascript, se minifiquen generando ficheros *.min.css y *.min.js para el css y javascript respectivamente. Para ello se ha utilizado la biblioteca grunt-contrib-uglify y grunt-contrib-cssmin.


####<a name="lnk6">6. Pruebas</a>

#### &nbsp;&nbsp;&nbsp;&nbsp;<a name="lnk6.1">6.1 Pruebas unitarias</a>

>Se ha realizado pruebas unitarias sobre el formulario de contacto, donde se comprueban las expresiones regulares que deben pasar los distintos campos que componen el formulario.

#### &nbsp;&nbsp;&nbsp;&nbsp;<a name="lnk6.2">6.2 Pruebas de integración</a>

>[PENDIENTE]

#### &nbsp;&nbsp;&nbsp;&nbsp;<a name="lnk6.3">6.3 Pruebas de verificación html y css</a>
	
#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a name="lnk6.3.1">6.3.1 Verificación HTML</a>
>Se ha verificado todo el código html con la herramienta proporcionada por el consorcio W3C (http://validator.w3.org).

#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a name="lnk6.3.1">6.3.2 Verificación CSS</a>

>Se ha verificado todo el código css con la herramienta proporcionada por el consorcio W3C (https://jigsaw.w3.org/css-validator).

AQUI

# Markdown-tests

#### <a href="#anchorLink">Anchor link</a>
#### &nbsp;&nbsp;&nbsp;&nbsp;<a href="#anchorLink2">Anchor link2</a>

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi suscipit quam at mi luctus, at suscipit dolor sollicitudin. Etiam lobortis, magna quis consectetur euismod, enim libero elementum elit, vitae porttitor dolor lorem a est. Cras rhoncus laoreet dolor malesuada commodo. Nullam ultricies mi et nisi venenatis, in dictum sapien pellentesque. Aenean molestie augue id orci accumsan, at feugiat justo cursus. Sed nec elit nisl. Aliquam commodo magna auctor, dapibus erat eget, egestas est. Ut nec purus condimentum nisi tempor fermentum. Fusce eros dui, volutpat quis rutrum non, consequat ac sapien. Ut varius nisl erat, eget rhoncus orci accumsan eget. Praesent posuere rutrum feugiat. Praesent in egestas eros. Aliquam auctor quis risus id imperdiet. Ut maximus ultrices tempus. Ut aliquet tempor felis, at commodo leo ullamcorper at. Praesent molestie nibh sit amet elit aliquam, a gravida neque condimentum.

Praesent tincidunt accumsan sodales. Praesent sit amet blandit elit. Mauris et mi nec dolor vehicula blandit. Morbi lorem urna, lobortis suscipit feugiat vel, bibendum in ex. Nullam tortor nibh, convallis at convallis eget, ornare ac quam. Nullam tempus leo eget tortor eleifend, et aliquam mauris lacinia. Nulla facilisi. Donec vestibulum, leo non imperdiet vestibulum, nibh orci consectetur turpis, at luctus nibh quam eget justo. Praesent nulla justo, maximus vitae consectetur placerat, consectetur nec lacus. Sed aliquet tristique nisi ac ornare. Donec at sem mattis, maximus purus a, laoreet metus. Donec consequat at magna ac posuere. In vehicula varius gravida. Praesent lacinia in risus id ornare. Suspendisse potenti. Nam imperdiet tristique odio, non mattis est blandit quis.

Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Nullam auctor mollis nisi sit amet commodo. Mauris vel tincidunt diam, vitae gravida nulla. Sed sollicitudin dictum egestas. Quisque nec tortor maximus, sagittis massa sed, cursus est. Integer non leo pulvinar, porttitor elit ut, egestas dui. Vestibulum ex orci, euismod vulputate quam blandit, gravida mattis tellus.

<a name="anchorLink">Anchor link</a>
Testing Markdown support

<a name="anchorLink2">Anchor link</a>
Testing Markdown support

