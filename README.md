# Book profesional — Andrés Gamonal

Página única con la trayectoria, los casos, la formación y los datos de contacto de Andrés Gamonal.
Se publica en **Cloudflare Pages** con la dirección **https://book.gamonal.app**.
No aparece en Google: está marcada como "no indexar", porque es un enlace que se comparte directamente.

## Qué hay en el proyecto

| Archivo o carpeta | Qué es | ¿Lo edito? |
|---|---|---|
| `index.html` | El book completo: textos, diseño y funcionamiento | Sí, los textos y enlaces (ver tabla de abajo) |
| `imagenes/` | Retrato de "Sobre mí", imagen para compartir el enlace e íconos | Solo para reemplazar una imagen (ver notas) |
| `favicon.ico` | Ícono de la pestaña del navegador | No (archivo técnico) |
| `_headers` | Configuración de Cloudflare: privacidad y seguridad | No (archivo técnico) |
| `DECISIONES-VISUALES.md` | Registro de decisiones de diseño vigentes | Solo para consultar o sumar decisiones |
| `README.md` | Este mapa | — |

## Quiero cambiar X → busco Y

Abre `index.html` y usa Ctrl+F (Cmd+F en Mac) con el texto de la segunda columna.
Cambia solo lo que está entre las etiquetas, sin tocarlas.

| Quiero cambiar | Busco |
|---|---|
| La píldora de la portada (cargo actual) | `Actualmente en` |
| El texto de bienvenida | `Bienvenido a mi` |
| La lámina de certificaciones de la portada | `Certificaciones<br>digitales` |
| El texto de "Sobre mí" | `Trabajo el marketing` |
| La foto de "Sobre mí" | `retrato-andres-gamonal` |
| Una marca o un caso | `CASO 01` … `CASO 07` |
| Las cifras de resultados de un caso | `TARJETAS DE RESULTADOS` |
| Formación, certificaciones, gremios o idiomas | `FORMACIÓN Y CREDENCIALES` |
| El CV (aparece en 3 lugares: menú, barra lateral y cierre) | `CV-Andr` |
| Correo, WhatsApp o LinkedIn | `mailto:` · `wa.me` · `linkedin.com/in/andresgamonal` |
| Lo que se ve al compartir el enlace (WhatsApp, LinkedIn) | `og:` (al inicio del archivo) |

## Contenido del book

1. Menú superior: logo y botón **Descargar CV**, visible en todas las pantallas.
2. Barra lateral flotante (solo en pantallas muy anchas): WhatsApp, correo, LinkedIn y CV.
3. Portada en carrusel: bienvenida con video y certificaciones digitales.
4. Cifras: 17+ años, 6 mercados, 6 compañías y Effie de Bronce.
5. Disciplinas en cinta móvil.
6. Sobre mí, con retrato.
7. Marcas (7) y un caso por marca: resumen, resultados, documentos, videos y audios. El orden va de la más reciente (Zurich) a la más antigua (Santander).
8. Formación y credenciales: educación, certificaciones, gremios, jurado Effie e idiomas.
9. Cierre con correo, WhatsApp, LinkedIn y CV.

## Cómo se publica (Cloudflare Pages)

El repositorio está conectado a Cloudflare Pages. **Cada cambio que llega a la rama `main` se publica solo** en 1 o 2 minutos.
Eso incluye los cambios hechos con el editor de contenido.
Para ver la versión nueva, recarga con Ctrl+Shift+R (Cmd+Shift+R en Mac).

Configuración inicial (se hace una sola vez, en el panel de Cloudflare):

1. **Workers & Pages** → **Create** → pestaña **Pages** → **Connect to Git**.
2. Elegir el repositorio `mio-book-profesional`.
3. Production branch: `main` · Framework preset: `None` · Build command: *(vacío)* · Build output directory: `/`.
4. **Save and Deploy**. Queda en `mio-book-profesional.pages.dev`.
5. En el proyecto → **Custom domains** → **Set up a custom domain** → `book.gamonal.app`.

Las otras ramas del repositorio generan una **vista previa** con su propia dirección (`<rama>.mio-book-profesional.pages.dev`), útil para revisar antes de publicar.

## Notas

- **Reemplazar una imagen de `imagenes/`:** usa un nombre nuevo (por ejemplo `retrato-andres-gamonal-2.webp`) y cámbialo en `index.html`. Los navegadores guardan esas imágenes una semana.
- **Vista previa al compartir:** WhatsApp y LinkedIn guardan la vista previa varios días. Para refrescarla en LinkedIn usa https://www.linkedin.com/post-inspector/.
- **Archivos externos:** las imágenes de marcas y casos están en `andresgamonal.com` y los PDF y audios en sus subdominios `cdn-*`. El CV, los certificados y el logo de Radar están en Cloudflare R2 (`pub-…r2.dev`). El ícono de Zurich está en `imagenes/logo-zurich.png` (isotipo oficial). Los videos se reproducen desde YouTube (`youtube-nocookie.com`).
- **Diseño:** paleta Gamonal (azul `#040764`, azul secundario `#1C73CB`, turquesa `#20B6B6`, amarillo `#FCE865`, gris `#3B3B3B`) y tipografía Roboto. Las decisiones vigentes están en `DECISIONES-VISUALES.md`.

---

© Andrés Gamonal · Brandformance Lab
