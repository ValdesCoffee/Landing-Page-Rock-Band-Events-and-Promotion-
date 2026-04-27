# 🎸 Generic Band — Unofficial Fan Page

> Proyecto académico de desarrollo web | Clan 3: Mulata | Auri Marcela Valdes Mendoza | 27-04-2026

---

## 📄 Descripción del proyecto

**Generic Band** es una página web de fan no oficial de una banda de rock ficticia llamada *Shattered Riffs*, creada como ejercicio académico de desarrollo web. La página recrea la experiencia visual de un sitio real de banda musical, con una estética oscura de rock/metal en tonos burgundy, rosa y negro.

Incluye:
- Video de fondo en pantalla completa (hero section)
- Barra de navegación con links externos
- Galería multimedia de fotos del concierto
- Mapa embebido de Google Maps (Hollywood Walk of Fame)
- Sección *About* con historia e influencias de la banda
- Formulario de contacto funcional vía Formspree

---

## 🛠️ Tecnologías utilizadas

| Tecnología | Uso |
|---|---|
| **HTML5** | Estructura semántica de la página (`header`, `nav`, `section`, `article`, `footer`) |
| **CSS3** | Estilos, animaciones (`@keyframes`), layout con Grid y Flexbox, fuentes personalizadas (`@font-face`), diseño responsive con media queries |
| **JavaScript (ES6)** | Año dinámico en el footer — archivo `aña.js` (listo para expandir) |
| **Google Maps Embed** | Iframe con la ubicación del Paseo de la Fama de Hollywood |
| **Formspree** | Envío del formulario de contacto sin backend propio |

---

## 📁 Estructura del proyecto

```
project-root/
├── index.html                  ← Archivo HTML principal
├── assets/
│   ├── css/
│   │   └── style.css           ← Todos los estilos y reglas responsive
│   ├── js/
│   │   └── aña.js              ← JavaScript (año dinámico, expandible)
│   ├── fonts/
│   │   ├── roll.ttf            ← Fuente de títulos/display
│   │   └── rock.woff           ← Fuente de párrafos
│   ├── images/
│   │   ├── thunder.svg         ← Logo de la banda
│   │   ├── img-1.jpg
│   │   ├── img-3.jpg           ← Imágenes de galería y sección About
│   │   └── img-4 ... img-10.jpg
│   └── videos/
│       └── *.mp4               ← Video de fondo del hero
└── README.md
```

### Secciones del HTML

| Sección | Descripción |
|---|---|
| `<header>` | Contiene el video de fondo y la barra de navegación |
| `<nav class="navbar">` | Nombre de la banda, links a merch & música, logo SVG |
| `.hero section` | Título grande superpuesto sobre el video (*Generic / Band*) |
| `.mainsection` | Texto descriptivo de la banda + iframe de Google Maps |
| `#media .mediacontainer` | Galería de 6 fotos en grid |
| `#about .about_container` | Historia, foto y lista de influencias de la banda |
| `<footer> #contact` | Copyright, links a redes sociales y formulario de contacto |

---

## 🚀 Cómo ejecutar el proyecto localmente

### Opción A — Abrir directo en el navegador *(más simple)*

1. Descarga o clona todos los archivos manteniendo la estructura de carpetas.
2. Abre `index.html` directamente en cualquier navegador moderno (Chrome, Firefox, Edge).

> ⚠️ El video de fondo y las fuentes personalizadas deben estar en sus rutas relativas correctas para cargar bien.

---

### Opción B — Servidor local *(recomendado)*

Un servidor local evita restricciones de seguridad del navegador al cargar archivos locales.

**Con VS Code — extensión Live Server:**
```bash
# 1. Instala la extensión "Live Server" en VS Code
# 2. Clic derecho en index.html → "Open with Live Server"
# 3. Se abre automáticamente en http://127.0.0.1:5500
```

**Con Node.js:**
```bash
npm install -g serve
serve .
# Luego abre http://localhost:3000
```

**Con Python:**
```bash
# Python 3
python -m http.server 8080
# Luego abre http://localhost:8080
```

---

### ✅ Checklist antes de visualizar

- [ ] Las carpetas `css/`, `js/`, `fonts/`, `images/` y `videos/` están dentro de `assets/`
- [ ] Los archivos de fuente `roll.ttf` y `rock.woff` están en `assets/fonts/`
- [ ] Hay al menos un archivo `.mp4` en `assets/videos/`
- [ ] Las imágenes de galería (`img-1.jpg`, `img-3.jpg` – `img-10.jpg`) están en `assets/images/`
- [ ] El logo `thunder.svg` está en `assets/images/`
- [ ] Tienes conexión a internet (para el mapa de Google Maps y el formulario de Formspree)

---

## 📝 Notas adicionales

- El formulario de contacto usa **Formspree** — no se requiere código del lado del servidor.
- El CSS incluye animaciones `@keyframes bounce` aplicadas a la galería, sección *About* y footer.
- Los breakpoints responsive están definidos en `max-width: 768px` y `max-width: 920px`.
- El archivo `aña.js` está vinculado al final del `<body>` por rendimiento y actualmente rellena el `<span id="year">` con el año actual dinámicamente.
- Se incluyen meta tags SEO en el `<head>` para mejorar la visibilidad en buscadores.

---

*Generic Band Unofficial Page — Clan 3: Mulata*