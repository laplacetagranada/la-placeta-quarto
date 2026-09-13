# La Placeta Granada — web (Quarto)

Instrucciones para probar y editar la web en tu ordenador. Todavía no está subida a GitHub — esto es para verla funcionando en local, añadir fotos reales y ajustar textos antes de publicarla.

## 1. Instalar Quarto (solo la primera vez)

Tienes dos opciones — cualquiera de las dos sirve:

- **Si usas RStudio**: las versiones recientes de RStudio ya traen Quarto integrado. Prueba directamente el paso 2; si te falla, instala Quarto por separado con la opción de abajo.
- **Instalador independiente**: ve a https://quarto.org/docs/get-started/, descarga el instalador para Windows y ejecútalo con las opciones por defecto. Es un único instalador, sin dependencias adicionales.

Para comprobar que quedó instalado, abre una terminal (o la pestaña "Terminal" dentro de RStudio) y escribe:

```         
quarto check
```

Debería confirmar que Quarto y Pandoc están instalados correctamente.

## 2. Ver la web en local

**Desde RStudio** (recomendado, si ya lo usas): abre esta carpeta como proyecto (File → Open Project, o simplemente abre cualquier archivo `.qmd` de la carpeta) y pulsa el botón **Render** en la barra superior del archivo. Se abre una vista previa de esa página. Para ver el sitio completo navegable, usa el botón "Preview" que aparece al abrir `_quarto.yml`, o ejecuta en la Terminal de RStudio:

```         
quarto preview
```

**Desde una terminal normal** (sin RStudio): dentro de esta carpeta, ejecuta:

```         
quarto preview
```

Se abre el navegador automáticamente con la web, y **cada vez que guardes un cambio en un archivo, la página se actualiza sola**. Para parar, `Ctrl+C` en la terminal.

## 3. Editar textos

Cada página es un archivo `.qmd` en la raíz de esta carpeta:

- `index.qmd` → Home
- `about-us.qmd` → About us
- `programmes.qmd` → Programmes
- `giving-back.qmd` → Giving Back
- `contact.qmd` → Contact

Es Markdown: los títulos empiezan por `#`/`##`, los párrafos son texto normal. Puedes editar libremente cualquier texto que no esté dentro de algo con esta forma: `::: {.nombre-de-clase}` ... `:::` — esas líneas marcan el principio y el final de un bloque de diseño (por ejemplo, la sección de citas de la Home, o una ficha de programa). No las borres ni las muevas; el texto que hay *dentro* de ellas sí lo puedes cambiar sin problema.

Ejemplo — esto es siempre seguro de cambiar:

```         
## Behind every stay

Every La Placeta Granada programme is run by a small, dedicated team...
```

Cambias el título y el párrafo como cualquier texto normal.

Si alguna vez rompes sin querer un bloque `:::`, Quarto te avisará en la vista previa con un mensaje de aviso (no rompe silenciosamente toda la página, a diferencia de HTML) — así sabrás que algo no cuadra antes de publicar.

## 4. Cambiar fotos

Las fotos están en `images/photography/`. Ahora mismo son marcadores de posición con el nombre de lo que deberían mostrar (ej. `albaicin.jpg`).

Para poner una foto real: **sustituye el archivo por tu foto, con el mismo nombre exacto**. Así no hace falta tocar ningún archivo de texto — la web la recoge sola la próxima vez que hagas Render/Preview.

## 5. Redes sociales, menú y pie de página

Todo esto se configura en el archivo `_quarto.yml`, en la sección `website:`. Por ejemplo, para poner tu Instagram real, busca esta línea dentro de `navbar: right:`:

```         
- icon: instagram
  href: "#"
```

y cambia `"#"` por tu URL real. El email de contacto y el resto de enlaces del pie de página están un poco más abajo en el mismo archivo, en `page-footer:`.

## 6. Activar "Who we collaborate with" / "Who we support" (Giving Back)

En `giving-back.qmd`, busca la línea:

```         
::: {.content-hidden}
```

Cuando tengas los nombres/logos confirmados, cambia `content-hidden` por `content-visible` en esa línea y esas dos secciones aparecerán en la web. Es la única línea que hay que tocar.

## 7. Cuando quieras dar el siguiente paso

Esto es una copia local, no está publicada todavía. Quarto tiene un comando propio para publicar en GitHub Pages más adelante (`quarto publish gh-pages`) — lo hacemos juntos paso a paso cuando llegue el momento.
