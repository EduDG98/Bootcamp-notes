# HTML5

El documento HTML es un documento de texto que esta dividido en dos partes: - `<!DOCTYPE html>` : tipo de documento para facilitar al navegador. - `<html></html>` : donde se añaden todas las etiquetas.

# _display_

Las etiquetas pueden ser de tipo : - **block**: como los `<div>` - **inline** : como los `<span>` si se define un alto / ancho el elemento lo ignorara porque es un elemento en línea. - **inline-block**: se trata de un elemento en línea al que sí se puede editar en alto y ancho.

# _Atributos_ comunes para todas las etiquetas

- id
- class
- style: para dar estilo (no se suele usar)
- title: para los tooltip (cuando se pone el ratón por encima).
- data-role: un meta dato que no aparece en la pág. web pero si utilizar en JS.

# Etiquetas del _head_

- `<title>`
- `<link>`
- `<meta>` : manda información meta que usa el navegador
  - ` <meta charset="UTF-8" />` Codificación del documento

# Etiquetas de agrupación

- `<p>`
- `<hr>` : cambio de tema entre párrafos (una línea horizontal pero se puede ocultar o cambiar)
- listas:
  - ordenada: `<ol>`
  - desordenadas: `<ul>`

# Etiquetas textuales

- enlaces: `<a href="https://..."> ... </a>`
- `<p>`
  - `<em>` : sustituye a italica/cursiva.
  - `<strong>` : sustituye a bold/negrita.
  - `<span>`
  - `<mark>`

# Etiquetas multimedia

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

# Etiquetas multimedia alternativa

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

# Formularios

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
  `html
 <select name="">
	<option value="..."> Opción 1 </option>
	<option value="..." selected> Opción 2 </option>
</select>`
- `<button>`

# Scripts

- `<script src="index.js"> .... <script/>`
  - **src**: añadir la ruta de un archivo js.
- `<noscript> ... </noscript>` : para los usuarios que tienen JS desactivado.

# Acordeón

```html
<details>
  <summary>Tema 1:</summary>
  <div>...</div>
</details>
```

# SEMÁNTICA

- `<article>` : tiene suficiente importancia de contenido.
  - `<header>`
  - `<section>` : una parte de la web.
  - `<footer>`
