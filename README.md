# Posts más Votados
En este proyecto se va a construir una aplicación para organizar los **posts** del blog de [Make It Real](http://blog.makeitreal.camp/) por medio de votos. El funcionamiento es similar al de páginas como [Reddit](http://reddit.com/) o [Hacker News](https://news.ycombinator.com/).

Los casos de uso son los siguientes:

### Listar posts:

Cuando el usuario ingresa a la aplicación, el sistema le debe mostrar la lista de  **posts**. Por cada  **post**  se debe mostrar:

-   Título
-   Descripción
-   Foto del autor
-   Foto del post
-   Cantidad de votos

### Organizar la lista de forma ascendente o descendente por número de votos:

La aplicación debe tener dos botones, uno para organizar la lista de según el número de votos de menor a mayor, y otro para organizarla de mayor a menor. Los botones deben tener estilos que identifiquen qué opción se encuentra seleccionada.

### Votar por un post

Cada post debe contar con dos botones: un botón para incrementar el número de votos, y otro botón para disminuir el número de votos.

Si un post supera el número de votos de otro, la lista se debe reorganizar automáticamente.

**JSON** de ejemplo: 
```
const  data  =  [
  {
	  id:  1,
	  title:  'Manejo de dependencias en Ruby con Bundler',
	  description:  'Bundler es una manejador de dependencias para Ruby. Aunque viene incluido con Rails, Bundler no es exclusivo de Rails, lo puedes usar para manejar las dependencias de cualquier proyecto de Ruby.',
	  url:  'http://blog.makeitreal.camp/manejo-de-dependencias-en-ruby-con-bundler/',
	  votes:  42,
	  writer_avatar_url:  '//a.disquscdn.com/uploads/users/2864/1155/avatar92.jpg?1481303405',
	  post_image_url:  'http://blog.makeitreal.camp/assets/images/bg-images/bundler.jpg',
  },
  {
	  id:  2,
	  title:  'Descubre si Make it Real es para ti',
	  description:  'En Make it Real buscamos entrenar a los desarrolladores Web que nosotros mismos quisiéramos contratar. Personas con autodisciplina que sean capaces de resolver problemas complejos y se adapten rápidamente a nuevas tecnologías y escenarios. En este post vamos a discutir algunas características de nuestro programa para que descubras si Make it Real es para ti.',
	  url:  'http://blog.makeitreal.camp/descubre-si-make-it-real-es-para-ti/',
	  votes:  43,
	  writer_avatar_url:  '//a.disquscdn.com/uploads/users/2864/1155/avatar92.jpg?1481303405',
	  post_image_url:  'http://blog.makeitreal.camp/assets/images/bg-images/laptop-sublime.jpg',
  },
  {
	  id:  3,
	  title:  '¿Qué es código?',
	  description:  'Semáforos, automóviles, aviones, aeropuertos, satélites, el sistema financiero, gran parte de nuestras vidas depende del código que varias generaciones de programadores han escrito. Pero ¿qué es código? ¿quién lo ejecuta y cómo? En este post vamos a hacer un recorrido histórico para entender cómo es que la electricidad se convierte en código y cómo surgieron los lenguajes de programación.',
	  url:  'http://blog.makeitreal.camp/que-es-codigo/',
	  votes:  44,
	  writer_avatar_url:  '//a.disquscdn.com/uploads/users/2864/1155/avatar92.jpg?1481303405',
	  post_image_url:  'http://blog.makeitreal.camp/assets/images/bg-images/code.jpg',
  },
  {
	  id:  4,
	  title:  'Aprende Desarrollo Web gratis',
	  description:  '¿Quieres iniciar en el mundo del desarrollo Web y no sabes por dónde empezar? Conoce Aprende Desarrollo Web, un curso completamente gratis dirigido a personas sin experiencia en el que aprenderás a crear y publicar sitios interactivos en Internet con HTML, CSS y JavaScript.',
	  url:  'http://blog.makeitreal.camp/aprende-desarrollo-web-gratis/',
	  votes:  45,
	  writer_avatar_url:  '//a.disquscdn.com/uploads/users/2864/1155/avatar92.jpg?1481303405',
	  post_image_url:  'http://blog.makeitreal.camp/assets/images/bg-images/aprende-desarrollo-web-bg.png',
  },
 ]
```
