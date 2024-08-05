# HTML: writing semantic html

Usar HTML semánticamente es darle un significado a las etiquetas y al contenido que estamos usando y no encerrar todo en etiquetas `<div>`.

![Mozilla Developer (MDN)](https://static.semrush.com/blog/uploads/media/0a/0f/0a0fd07d0a6ee7a7f893b0e21379c0ae/ES-Semantic-Search-Non-Semantic.webp)

> Imagen tomada de [SEMRUSH](https://es.semrush.com/blog/html-semantico/).

Como vemos en la imagen, hay varias etiquetas `(<header>,<footer>,<aside>,<article>, etc.)` que nos servirán para darle al documento HTML el significado que nosotros queramos.

Usar HTML semántico ayuda a los motores de búsqueda a encontrar la página de manera más efectiva, mejorando su posicionamiento en los resultados de búsqueda. También, es fundamental para mejorar la accesibilidad y la funcionalidad con tecnologías de asistencia, como los lectores de pantalla, facilitando la navegación para personas con discapacidades. Además, el uso de HTML semántico mejora la mantenibilidad y la colaboración en el desarrollo web, ya que proporciona una estructura clara y comprensible del contenido.


Algunas de las etiquetas para escribir HTML semánticamente son:

# Header

Sirve para poner la parte superior o introductorio de la página web, generalmente suele usarse con algún logo, el título o los enlaces de navegación. Con la etiqueta `<header>` puede crear una separación clara entre el encabezado y el contenido principal de su página, lo que facilita que los usuarios comprendan y naveguen por su sitio web.

```html
<!-- Non-semantic header -->
<div class="header">
  <h1>My Site</h1>
  <nav>
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Contact</a>
  </nav>
</div>

<!-- Semantic header -->
<header>
  <h1>My Site</h1>
  <nav>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>
</header>
```