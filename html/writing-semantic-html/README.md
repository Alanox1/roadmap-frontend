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



# Nav

La etiqueta `<nav>` se usa para poner los enlaces de navegación, al usarla le decimos tanto al motor de busqueda como a los usuarios que esa parte de la página web esta hecha para la navegación.

```html
<!-- Non-semantic navigation -->
<div class="navigation">
  <a href="#">Home</a>
  <a href="#">About</a>
  <a href="#">Contact</a>
</div>

<!-- Semantic navigation -->
<nav>
  <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">About</a></li>
    <li><a href="#">Contact</a></li>
  </ul>
</nav>
```


# Main

La etiqueta `<main>` se usa para poner el contenido principal de la página web, solo puede haber uno por documento HTML y posiblemente es donde los usuarios pasen el mayor tiempo en su estadia por la pagina web. 


```html
<!-- Non-semantic main content -->
<div class="main-content">
  <h2>About Us</h2>
  <p>Welcome to our website. We are a company that specializes in widgets.</p>
</div>

<!-- Semantic main content -->
<main>
  <h2>About Us</h2>
  <p>Welcome to our website. We are a company that specializes in widgets.</p>
</main>
```



# Article

Sirve para poner un contenido independiente, como una entrada de blog, algún comentario o un artículo de noticias. El contenido dentro de la etiqueta `<article>` tiene que ser independiente y significativo y puede incluir párrafos, imágenes, títulos,etc.


```html
<!-- Non-semantic article -->
<div class="article">
  <h2>How to Make a Widget</h2>
  <p>Widgets are great. Here's how to make one.</p>
</div>

<!-- Semantic article -->
<article>
  <h2>How to Make a Widget</h2>
  <p>Widgets are great. Here's how to make one.</p>
</article>

```







# Aside

La etiqueta `<aside>` sirve para la información relacionada con la página pero que no pertenece al contenido principal de ella, principalmente se usa como una barra lateral y se pone elementos como información complementaria, anuncios o artículos relacionados.


```html
<div>
  <article>
    <h2>Article Title</h2>
    <p>Article content goes here</p>
  </article>
  <aside>
    <h3>Related Articles</h3>
    <ul>
      <li><a href="#">Article 1</a></li>
      <li><a href="#">Article 2</a></li>
      <li><a href="#">Article 3</a></li>
    </ul>
  </aside>
</div>
```





# Section

La etiqueta `<section>` en HTML se usa para dividir una página en partes que tienen algo en común, como si estuvieras separando una página en secciones para que todo quede más prolijo y entendible. Cada `<section>` agrupa contenido relacionado, como si estuvieras separando en partes una página para que sea más fácil de leer.

```html
<section>
  <h2>Introducción</h2>
  <p>Bienvenidos al evento anual.</p>
</section>

<section>
  <h2>Cronograma</h2>
  <p>El evento arranca a las 9 AM.</p>
</section>

<section>
  <h2>Detalles del Lugar</h2>
  <p>Centro de Convenciones de Buenos Aires.</p>
</section>
```





# Footer

El `<footer>` en HTML es como el pie de página de un documento. Es el lugar donde metés la info que va al final de la página, como derechos de autor, enlaces a redes sociales, o info de contacto. Es como el espacio donde cerrás la página con datos importantes

```html
<footer>
  <p>&copy; 2024 Mi Sitio Web. Todos los derechos reservados.</p>
  <p>Seguinos en <a href="#">Twitter</a> y <a href="#">Facebook</a></p>
  <p>Contacto: <a href="mailto:info@misitio.com">info@misitio.com</a></p>
</footer>
```
.






# Figure y Figcaption

La etiqueta `<figure>` se usa para contenido que puede ser independiente del resto del documento, como imágenes, gráficos, o cualquier otro contenido visual, y la etiqueta `<figcaption>` sirve para agregarle una descripción.


```html
<figure>
  <img src="imagen.jpg" alt="Una imagen copada">
  <figcaption>Esta es una imagen copada de mi último viaje.</figcaption>
</figure>
```

Acá, `<figure>` agrupa la imagen y su descripción, y `<figcaption>` agrega el pie de foto. La idea es que, si sacás todo el bloque `<figure>`, siga teniendo sentido por sí solo, como un post de Instagram con su foto y descripción.




# Las etiquetas `<div>` y `<span>` son etiquetas semánticas?

Las etiquetas `<div>` y `<span>` no son etiquetas semánticas. Se utilizan para marcar áreas de contenido genéricas y no transmiten ningún significado específico. Solo debes utilizar estas etiquetas si no tienes otra opción.



# En el archivos index.html, pueden ver una página hecha con etiquetas semánticas.

# Muchas gracias a Semrush y a pexels por las fotos, pueden ir a ver su página y aprender de ellos también.

- [Semrush Blog](https://es.semrush.com/blog/html-semantico/) 
- [Daniel Nettesheim](https://www.pexels.com/es-es/foto/logotipo-blanco-y-azul-de-la-ruta-66-1162361/) 
- [Pixabay](https://www.pexels.com/es-es/foto/ruta-66-impresa-en-la-carretera-210112/) 
- [Łukasz Kondracki](https://www.pexels.com/es-es/foto/carretera-firmar-estados-unidos-linea-5988878/) 
- [Patrick Gamelkoorn](https://www.pexels.com/es-es/foto/blanco-y-negro-monocromo-escala-de-grises-senalizacion-13709137/) 

## Páginas que me sirvieron: 

- [Semrush Blog](https://es.semrush.com/blog/html-semantico/) 
- [cs.fyi](https://cs.fyi/guide/writing-semantic-html) 
- [Pexels](https://www.pexels.com/es-es/)


