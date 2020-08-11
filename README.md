# LIGNUM BOOTCAMP 07/2020 #

### Bienvenidos al bootcamp acelerado de agosto 2020.  ###

Este curso supone que ya superaron los conocimientos básicos de HTML-CSS-JS, validaciones, accesibilidad, media-queries, layouts, 
css-reset para mayor consistencia entre browsers como normalize.css, configuración de servidores locales, manejo de paquetes tanto locales como algún sistema de manejo de paquetes como npm,
entendimiento de CORS https://web.dev/cross-origin-resource-sharing/, Bootstrap,
el uso de herramientas de depuración como la consola de Chrome -> https://developers.google.com/web/tools/chrome-devtools/console?utm_campaign=2016q3&utm_medium=redirect&utm_source=dcc, entre otros.

### Preparacion ###
1)Descargar e instalar un entorno de desarrollo, por ejemplo, apache -> https://www.apachefriends.org/es/index.html

2)Descargar e instalar laravel -> https://laravel.com/docs/7.x/installation

3)Asegurarse de estar usando la última versión de su navegador, Firefox, Chrome, Edge, etc.

### Actividades ###

A pesar de que las palabras MVC ya no sirven para definir la estructura del proyecto, debido a la gran cantidad de capas extra que se agregaron en la complejidad de las aplicaciones, ya que Modelo es solo
una parte de la estructura de App, Controller es una parte de Http junto a Middleware, request, routes. Views es una parte de Resources...  Las siguientes actividades deben ser realizadas utilizando 
una estructura de Modelo-Vista-Controlador, un recurso didáctico un poco antiguo que podrían revisar si es que se les escapa algún concepto es este https://styde.net/laravel-5/

## Usted dispondrá de 48 horas para entregar o hacer lo mayor posible de las siguientes tareas. ##


1)
Crear las migraciones de las siguientes tablas: -> https://laravel.com/docs/7.x/migrations

Película:
Año
Titulo
Duración
Sinopsis
Imagen
ActorPrincipalID

Actor:
Nombre
FechaNacimiento

2)
Crear las relaciones película-actor y actor-película -> https://laravel.com/docs/7.x/eloquent-relationships

3)
Crear el CRUD de los mismos utilizando eloquent para el manejo de los datos y guardarlos en MySQL -> https://laravel.com/docs/7.x/controllers#resource-controllers

4)
Visualización de imagen de la película y el cargado de la misma desde el ABM (Desde local, no un link a una imagen).

5)
Poder marcar las películas como favoritas y visualizarlo con AJAX.


Extra:

Sencillo:

Botones de clear data de los campos.
Drag and Drop para las imágenes

Medio:

buscador con sugerencias - hacer un endpoint de API que devuelva un JSON y le muestre al usuario sugerencias de lo que escribió o el listado de las películas o algo por el estilo
ejemplo: https://darkville.tv/ o el de Netflix (puntos extra por este último).

Avanzado:

Websockets - Abrir un websocket y probarlo contra http://www.websocket.org/echo.html

### Criterios a tener en cuenta ###

*El proyecto deberia ser tan modular como sea posible.
Es decir, las funciones de una persona deberian estar en PeliculaController y las de un usuario en UsuarioController, no mezcladas en el mismo archivo.

*El naming de las funciones deberia ser segun funcionalidad y luego el modelo, si el nombre es autodescriptivo todavia mejor.
Por ejemplo, si tengo una funcion para crear una persona y otra para crear una pelicula deberian llamarse crearPersona() y crearPelicula()

### Consejos ###
Las aplicaciones se pueden hacer en cualquier orden, pero talvez seguir estos pasos te ayuden.

*Crear las migraciones sus controladores, modelos y vistas.

*Crear la relación en los modelos.

*Crear las vistas que permitan al superusuario cargar los datos de la película

*Crear la funcionalidad en el controlador para actualizar los datos.



*Crear una vista donde el usuario visualice las películas y pueda darle al botón de "Favorito" (Muestre el cambio con AJAX sin necesidad de recargar la pantalla)

*Crear una vista donde el usuario pueda ver su listado de películas favoritas.



*Crear lo necesario para que el superusuario pueda editar y borrar películas.

### ¿Como comienzo? ###

Primero, piensa cual debería ser la estructura de tu aplicación (Primero estructura de datos de la base de datos, luego en que orden irían las pantallas).
No hace falta crear usuarios ni roles, pero sí que las pantallas se diferencien de cual sería para cada uno.

Luego piensa en las pantallas del CRUD de la película/actor.
El siguiente paso sería poder visualizar las películas como el usuario que visita la página y permitir elegir como favoritos.
Ahora crea la pantalla para ver el listado de las películas favoritas.

Por último, afina los detalles (drag & drop de imágenes, estética, etc.).


### ¡Es imposible que logre terminar esto! ###
No te preocupes por eso e intenta completar los puntos importantes.

Ten en cuenta que todo conocimiento sirve y que no hay un puntaje específico para cada actividad, no hay porque ponerse nervioso, es solo una pequeña muestra de lo que sabemos o aprendimos
en el bootcamp.

¡Manos a la obra!
