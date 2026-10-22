# Newsletter | Laboratorio de Ciencia de Datos e IA – UCA

Archivo web de los newsletters mensuales del Laboratorio (GitHub Pages).

## Estructura

```
index.html                  ← landing con la lista de ediciones
assets/                     ← logos de la landing
newsletters/
  2026-10/index.html        ← edición de octubre (+ carpeta imagenes/)
  2026-11/index.html        ← página "en preparación" (reemplazar cuando esté lista)
.nojekyll                   ← evita que GitHub procese el sitio con Jekyll
```

## Publicar por primera vez

1. Crear un repositorio en GitHub (por ejemplo `newsletter-lab-uca`), público.
2. Subir **el contenido** de esta carpeta a la raíz del repositorio (Add file → Upload files).
3. En el repositorio: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   rama `main`, carpeta `/ (root)` → Save.
4. En 1–2 minutos el sitio queda en `https://<usuario>.github.io/newsletter-lab-uca/`.

## Publicar la edición de noviembre (y las siguientes)

1. Tomar la versión **editable** del newsletter (la que usa una carpeta de imágenes, no la autónoma en base64).
2. Copiarla como `newsletters/2026-11/index.html` (reemplaza la página "en preparación").
3. Copiar las imágenes en `newsletters/2026-11/imagenes/` y cambiar en el HTML
   `imagenes-newsletter-noviembre/` por `imagenes/`.
4. (Opcional) Pegar arriba del preheader la barra "← Volver al archivo" que tiene la edición de octubre.
5. En `index.html`: sacar el chip "En preparación" y la clase `nueva` de noviembre, y cambiar el botón a
   `class="btn"` con el texto "Leer edición".
6. Para un mes nuevo: crear `newsletters/AAAA-MM/` y copiar un bloque `<li>` arriba de todo en `index.html`.

Las rutas son relativas, así que el sitio funciona igual abriéndolo local o publicado.
