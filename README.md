# Retro Garage — Landing Page

Página pública del restaurante **Retro Garage**, desplegada en GitHub Pages. Muestra el menú, información del local, galería de fotos y un enlace de descarga de la app móvil.

🌐 **[Ver sitio en vivo](https://lguerrero01.github.io/retro-garage-landing/)**

---

## Páginas

| Ruta | Descripción |
|---|---|
| `/index.html` | Landing principal — Hero, Menú, Nosotros, Galería, Contacto, Descarga |
| `/privacy.html` | Política de Privacidad de la app móvil |

---

## Características

- **Menú en tiempo real** — lee los productos directamente de Supabase, filtrable por categoría
- **Configuración dinámica** — toda la información del restaurante (fotos, textos, redes sociales) se gestiona desde el panel de administración de la app, sin tocar código
- **Sin frameworks** — HTML, CSS y JavaScript puro. Sin dependencias, carga instantánea
- **Animaciones** — floating shapes, scroll reveal, galería con lightbox
- **Responsive** — optimizado para móvil, tablet y escritorio
- **GitHub Pages** — deploy automático al hacer push a `main`

---

## Cómo funciona

El sitio lee datos de dos tablas en **Supabase** usando la API REST pública (sin autenticación):

```
restaurant_config  →  nombre, eslogan, imágenes, horario, contacto, redes
products           →  menú completo con precios, categorías e imágenes
```

Cualquier cambio guardado desde el **panel admin de la app** se refleja automáticamente en esta landing al recargar la página.

---

## Actualizar contenido

Todo se configura desde la app (Panel Admin → botón **Landing**):

| Campo | Dónde configurarlo |
|---|---|
| Nombre, eslogan, descripción | Tab "Info" |
| Imagen hero, logo, foto "Acerca de" | Tab "Imágenes" |
| Galería de fotos | Tab "Imágenes" → sección galería |
| Play Store, Instagram, Facebook | Tab "Social / Links" |
| Menú y precios | Panel Admin → productos |

---

## Estructura

```
retro-garage-landing/
├── index.html      # Landing principal
├── privacy.html    # Política de privacidad
└── README.md
```

---

## Stack

- HTML5 / CSS3 / JavaScript ES Modules
- [Supabase](https://supabase.com) — base de datos y almacenamiento de imágenes
- [Google Fonts](https://fonts.google.com) — Bebas Neue + Inter
- GitHub Pages — hosting gratuito

---

## Repositorio de la app

El código de la aplicación móvil (Angular 17 + Supabase) se encuentra en el repositorio principal de **Retro Garage**.

---

## Contacto

**Retro Garage** · Valencia · 04244095467
