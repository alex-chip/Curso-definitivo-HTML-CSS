# Curso definitivo de HTML y CSS

HTML = Hypertext Markup Language (lenguaje de marcado de texto), es la opción que nos permite saltar entre páginas por medio de hipervínculos.



## Anatomía de una página Web

Es la estructura en cual esta formado nuestra página web. Existen etiquetas para diferenciar cada parte de esta tales como, `Header`, `Main`, `Sidebar` y `Foooter`, estos entre los más conocidos.



### Index y su estructura básica

Cuando creamos un proyecto lo primero es crear un archivo de HTML el cuál lo nombraremos `index.html`, este nombre se le da por el simple motivo que el navegador web busca este archivo por defecto a menos que se le indique lo contrario, la extensión `.html` es con el cuál se define un archivo `HTML`.



- `<!DOCTYPE html> `= Con esta etiqueta indicamos al navegador que es lenguaje HTML5.
- `<html lang="es">` Esta etiqueta `<html>` indicamos el lenguaje nuestra página web, es el contenedor padre, la atributo `lang="es"` es para indicar el idioma en que esta la página.
- `<head> ` Con esta etiqueta determinamos los encabezados.
- `<meta charset="UTF-8">` Con esta etiqueta definimos el tipo de encoding que se usara.
- `<meta name="description" content="Breve descripción de la página" />` Etiqueta meta para ponerle una descripción a la página y así los buscadores poder indexar la página.
- `<meta name="viewport" content="width=device-width, initial-scale=1.0">` Etiqueta meta para indicar al buscador que se usará Responsive Design

```html
  <!DOCTYPE html>
  <html lang="es">
  <head>
    <meta charset="UTF-8">
    <meta name="description" content="Esta pagina te mostrara fotos de gatos" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
  </head>
  <body>
  </body>
  </html>
```


### Anatomía de una etiqueta de HTML

![Antomía-etiqueta-html](https://raw.githubusercontent.com/alex-chip/Curso-definitivo-HTML-CSS/master/Images/anatomia%20de%20html-fc475d3a-6d91-41b5-a893-ee4790dcb637.webp)



## Tipos de Imágenes

### Existen 2 tipos de imágenes:

- `Sin perdida ( Lossless)` : capturan todos los datos de su archivo original. Por esto, estas imágenes suelen ser pesadas porque no pierden calidad.

- `Con perdida (Lossy)` : son imágenes de un formato que nos ayudan a perder un poco la calidad pero vamos a mejorar mucho el tamaño de la misma y con esto el tiempo de carga en los navegadores. Suelen ser muchos más pequeñas que los archivos Lossless y esto es lo ideal para que carguen más rápido en el navegador al ser más ligeras.
  el formato de imagen que utilicemos, va a determinar si es una imagen con perdida o sin perdida.
  Si ocupamos imágenes muy pesadas, que no tienen mucha perdida, nuestras páginas se van a abrir muy lento
  y esto va a perjudicar la experiencia del usuario.

  

Dicho esto, ¿qué formatos de imágenes existen? :

- `GIF (graphics Interchange Format):` Imagen tipo Lossless. No se pueden comprimir más. Tienen un máximo de 256 colores. Se los utiliza para mostrar animaciones simples y gráficos con colores planos.

- `PNG-8 (Portable Network Graphics)` : Imagen tipo Lossless. Tienen un máximo de 256 colores. Son ideales para iconos. No tiene animaciones. Poseen fondos transparentes

- `PNG-24` : Imagen tipo Lossless. Uso de colores ilimitados. Por esto, este formato es más pesado que un GIF y un PNG-8.

- `JPG/JPEG (Photographic Experts Group)` : Imagen tipo Lossy. Es un formato para fotografía. Tiene millones de colores disponibles.

- `SVG(scalable Vector Graphics)` : Formato vector/Lossless. Es un formato muy ligero que nos puede generar íconos y logotipos que estén hechos para escalar. Los vamos a utilizar generalmente para pantallas de retina, que van a multiplicar los pixeles de la pantalla y la imagen va a crecer, y sin embargo no perderá calidad.

  

### Diferencia de Imágenes

![Tipo de Imágenes](https://raw.githubusercontent.com/alex-chip/Curso-definitivo-HTML-CSS/master/Images/table%20for%20diferent%20images-42fdf349-a492-4ff5-afbd-1f437c804e4a.webp)



### Optimización de imágenes

Tamaño máximo recomendado para una imagen: 70kb

Herramientas para optimizar imágenes:

-  [Tiny PNG](https://tinypng.com/): comprime el tamaño de una imagen, para hacerla más ligera.
- [Squoosh](https://squoosh.app/): También nos ayuda a reducir el tamaño de las imágenes.
- [Verefix](https://www.verexif.com/): Elimina los meta-datos de una imagen, para reducir su tamaño.



## Etiquetas HTML

### Etiqueta Vídeo

Está etiqueta `<video></video>` nos permite insertar vídeo a nuestra página web.

Atributos que podemos usar en la etiqueta vídeo.



- `controls` : Atributo que nos muestra los controles del reproductor para manipular el vídeo.

- `preload`: Con este atributo le indicamos al navegador que cargue de manera anticipada  el vídeo para estar listo para la reproducción.



  En la etiqueta vídeo podemos usar otra etiqueta llamada `<source/>` este nos permite indicar el vídeo en varios formatos dejando al navegador la responsabilidad de reproducir el que el entienda, en caso de conocer más de un formato tomará el primero de manera descendente.

  Atributos de la etiqueta `<source/>`

  - `preload = "metadata"`: Este nos carga los meta-datos del vídeo de manera previa.
  - `preload="none"`: No existe carga previa del vídeo

``````html
<video controls preload>
    <source preload="metadata" preload="none" src="./my-video.m4v" />
	<source src="./my-video.mp4" />
</video>
``````



### Formularios

Los formularios nos ayudan a poder recolectar información de los usuarios, tal como inicio de sesión, información de contacto, compra de producto etc.

Para indicar al navegador que habrá un formulario utilizamos la etiqueta `form`



