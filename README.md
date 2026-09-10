# Sitio web de Mateo Piñeros Bernal

Sitio de una sola página (HTML/CSS/JS puro, sin frameworks ni dependencias de pago) listo para publicarse gratis con **GitHub Pages**.

## Estructura del proyecto

```
mateo-site/
├── index.html
├── README.md
└── assets/
    ├── css/styles.css
    ├── js/main.js
    └── img/
        ├── mateo-1.webp
        └── mateo-2.webp
```

## Cómo publicarlo en GitHub Pages (gratis)

### 1. Crea el repositorio
1. Entra a [github.com](https://github.com) e inicia sesión con tu cuenta.
2. Haz clic en **New repository** (botón verde arriba a la derecha, o "+" → "New repository").
3. Nómbralo, por ejemplo: `mateo-pineros` (el nombre no importa mucho, pero mejor sin espacios ni tildes).
4. Déjalo en **Public** (para GitHub Pages gratis el repo debe ser público, salvo que tengas plan de pago).
5. No marques ninguna casilla de inicializar con README (ya tenemos uno) y da clic en **Create repository**.

### 2. Sube los archivos
La forma más fácil sin usar la terminal:
1. En la página del repo recién creado, haz clic en **uploading an existing file** (o "Add file" → "Upload files").
2. Arrastra **toda la carpeta** `mateo-site` (o todos sus archivos y subcarpetas: `index.html`, `README.md` y la carpeta `assets` completa).
3. Escribe un mensaje de commit, por ejemplo "Primera versión del sitio", y da clic en **Commit changes**.

> Si prefieres usar git desde la terminal:
> ```bash
> cd mateo-site
> git init
> git add .
> git commit -m "Primera versión del sitio"
> git branch -M main
> git remote add origin https://github.com/TU-USUARIO/mateo-pineros.git
> git push -u origin main
> ```

### 3. Activa GitHub Pages
1. En el repositorio, ve a **Settings** (pestaña arriba).
2. En el menú izquierdo, busca **Pages**.
3. En "Build and deployment" → "Source", selecciona **Deploy from a branch**.
4. En "Branch", elige `main` y la carpeta `/ (root)`. Da clic en **Save**.
5. Espera 1-2 minutos. GitHub te mostrará la URL pública, algo como:
   `https://tu-usuario.github.io/mateo-pineros/`

Listo — la página queda publicada gratis, sin servidores ni costos de hosting.

### 4. (Opcional) Dominio propio
Si más adelante compran un dominio (ej. `mateopineros.co`), en la misma sección **Pages** hay un campo **Custom domain** donde se configura, junto con un registro DNS tipo `CNAME` apuntando a `tu-usuario.github.io`.

## Qué falta completar

Dejé marcado en el código lo que quedó pendiente:

- **Sección "Propuestas"**: tiene 5 tarjetas con texto de relleno (Lorem Ipsum) solo para mostrar el diseño. Busca `<!-- ===== PROPUESTAS ===== -->` en `index.html` y reemplaza el `<h3>` y `<p>` de cada `<article class="card">` con el título y la descripción real de cada propuesta.
- **Redes sociales**: los íconos de Instagram, Facebook y WhatsApp en la sección de contacto (`<!-- ===== CONTACTO ===== -->`) apuntan a `href="#"` — hay que reemplazarlos por los enlaces reales de las cuentas de campaña.
- **Fotos**: se usaron las dos fotos que compartiste (`mateo-1.webp` en el inicio, `mateo-2.webp` en "Sobre mí"), ya optimizadas para que la página cargue rápido. Puedes agregar más o reemplazarlas por otras siguiendo el mismo formato cuadrado con fondo de color.

## Edición rápida sin saber programar

- Los textos están directamente en `index.html`, se pueden editar con cualquier editor de texto (o incluso directamente en GitHub, con el ícono de lápiz ✏️ al ver el archivo).
- Los colores y estilos están en `assets/css/styles.css`, en la parte de arriba (`:root`), tomados del manual de marca (morado `#7868F7`, negro `#1C263F`, amarillo `#F6DE06`, rojo `#DA131A`).
- Cada cambio que subas a GitHub se refleja automáticamente en la página publicada en 1-2 minutos.
