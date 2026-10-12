# Encantos Nativos — sitio web

Página de Encantos Nativos, turismo rural y ecohotel en la vereda La Honda,
San Rafael, Antioquia. RNT 240497.

Sitio estático: HTML, CSS e imágenes. No necesita compilarse ni instalar nada.

## Estructura

```
index.html        la página completa (HTML + CSS + JS en un solo archivo)
img/              fotos, logo, íconos e imagen para compartir en redes
vercel.json       caché de las imágenes en Vercel
.htaccess         equivalente para hosting Apache / LiteSpeed (Vercel lo ignora)
robots.txt        permite la indexación de buscadores
sitemap.xml       mapa del sitio para Google
```

## Publicar

Conectado a Vercel desde este repositorio: cada cambio que se guarde en la rama
principal se publica solo. En Vercel, el framework es **Other** y no hay comando
de build ni carpeta de salida: los archivos van en la raíz.

## Editar

- **Textos:** se editan directamente en `index.html`.
- **Fotos:** se reemplazan en `img/` conservando el mismo nombre de archivo.
  Antes de subirlas, reducirlas a 1000 px de ancho y menos de 250 KB.
  Como el nombre no cambia, los navegadores que ya tengan la foto vieja la
  conservan hasta un día. Para que el cambio se vea de inmediato, súbele el
  número de versión a la URL en `index.html`: `img/foto.jpg?v=2` → `?v=3`.
- **Dominio:** aparece en `index.html` (canonical, `og:url`, `og:image`) y en
  `sitemap.xml`. Si cambia, hay que actualizarlo en los cuatro sitios.

## Enlaces del negocio

- WhatsApp de reservas: <https://wa.me/573147953068>
- Instagram: <https://www.instagram.com/encantosnativosturismorural/>
- Google Maps: <https://maps.app.goo.gl/cBhWujCbDsFYWjBEA>
