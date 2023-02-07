# HTML5

**ÍNDICE:**

1. [Etiquetas principales](#id1)
2. [`display`](#id2)
3. [Atributos comunes para todas las etiquetas](#id3)
4. [Etiquetas del _head_](#id4)
5. [Etiquetas de agrupación](#id5)
6. [Etiquetas textuales](#id6)
7. [Etiquetas multimedias](#id7)
8. [Etiquetas multimedias alternativas](#id8)
9. [Formularios](#id8)
10. [Scripts](#id10)
11. [Acordeón](#id11)
12. [Semántica](#id12)

# 1.Etiquetas principales<a name="id1"></a>

El documento HTML es un documento de texto que está dividido en dos partes:

- `<!DOCTYPE html>` : tipo de documento para facilitar al navegador.
- `<html></html>` : donde se añaden todas las etiquetas.

# 2. _display_ <a name="id2"></a>

Las etiquetas pueden ser de tipo :

- **block**: como los `<div>`
- **inline** : como los `<span>` si se define un alto / ancho el elemento lo ignorará porque es un elemento en línea.
- **inline-block**: se trata de un elemento en línea al que sí se puede editar en alto y ancho.

# 3. _Atributos_ comunes para todas las etiquetas <a name="id3"></a>

- id
- class
- style: para dar estilo (no se suele usar)
- title: para los tooltip (cuando se pone el ratón por encima).
- data-role: un meta dato que no aparece en la pág. web pero si utilizar en JS.

# 4. Etiquetas del _head_ <a name="id4"></a>

- `<title>`
- `<link>`
- `<meta>` : manda información meta que usa el navegador
  - ` <meta charset="UTF-8" />` Codificación del documento

# 5. Etiquetas de agrupación <a name="id5"></a>

- `<p>`
- `<hr>` : cambio de tema entre párrafos (una línea horizontal pero se puede ocultar o cambiar)
- listas:
  - ordenada: `<ol>`
  - desordenadas: `<ul>`

# 6. Etiquetas textuales <a name="id6"></a>

- enlaces: `<a href="https://..."> ... </a>`
- `<p>`
  - `<em>` : sustituye a italica/cursiva.
  - `<strong>` : sustituye a bold/negrita.
  - `<span>`
  - `<mark>`

# 7. Etiquetas multimedia <a name="id7"></a>

- imágenes: `<img src="imagen.jpg" alt="texto">`
  - src: ruta de la imagen.
  - alt: texto alternativo si no se carga la imagen.
- vídeo: `     <video src="video.mp4"
			poster="imagen.png"
			autoplay loop muted controls>
</video>`
  - Los ultimos atributos son _booleans_ que se activan al añadirlos.
  - _controls_ : muestra los controles.
- audio: `     <audio src="video.mp4"
			autoplay loop muted controls>
</audio>`

# 8. Etiquetas multimedia alternativa <a name="id8"></a>

- Varias alternativas de fuente:
  - ````<video>
    		<source = "...">
    		<source = "...">
    		<img ... >
    	</video>```
    ````
- Poner contenido de una página web (youtube, google maps, facebook, twitter, ...):
  - ```<iframe>
    		<src = "...">
    	</iframe>
    ```

# 9. Formularios <a name="id9"></a>

- `<input>`:

  - _type_:

    - text
    - search
    - tel: teléfono
    - url
    - email
    - password
    - hidden: informacion oculta que el usuario no ve pero que si se puede enviar.
    - number
    - date
      - min: fecha mínima.
      - max: fecha máxima.
    - color
    - radio
    - checkbox
      - checked
    - file: para añadir archivos.

    - **submit**: para enviar formulario
    - **image**: es para enviar un formulario pero presionando una imagen
      - src
    - **reset**: resetear formulario

  - _value_: el valor del input, aparece escrito en el input como si lo hubiera hecho el usuario.
  - _placeholder_: texto escrito hasta que se pincha.

- `<select>`
  ```html
  <select name="">
    <option value="...">Opción 1</option>
    <option value="..." selected>Opción 2</option>
  </select>
  ```
- `<button>`

# 10. Scripts <a name="id10"></a>

- `<script src="index.js"> .... <script/>`
  - **src**: añadir la ruta de un archivo js.
- `<noscript> ... </noscript>` : para los usuarios que tienen JS desactivado.

# 11. Acordeón <a name="id11"></a>

```html
<details>
  <summary>Tema 1:</summary>
  <div>...</div>
</details>
```

# 12. SEMÁNTICA <a name="id12"></a>

- `<article>` : tiene suficiente importancia de contenido.
  - `<header>` : encabezado
  - `<section>` : una parte de la web.
  - `<footer>` : pie de pág. o contenido de contacto.
