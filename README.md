# Studio 39

Landing page para un estudio de desarrollo web freelance, hecha como pieza de portafolio y como sitio real de contacto.

**Demo en vivo:** https://studio39-dev.netlify.app

## Qué muestra

Servicios, proceso de trabajo y un caso de estudio real ([Filo — Barbería](https://github.com/Lissandra2009/Barberia)), con un sitio completamente bilingüe (español / inglés) sin recargar la página.

## Stack

- HTML, CSS y JavaScript vanilla — sin frameworks ni build step
- Sistema de traducción propio (`data-i18n` + diccionario JS), con persistencia en `localStorage`
- [Netlify](https://netlify.com) para el deploy

## Características técnicas

- **Bilingüe en cliente**: todo el contenido vive en un diccionario JS (`translations.es` / `translations.en`), aplicado vía atributos `data-i18n`. Detecta el idioma del navegador la primera vez y recuerda la elección del usuario.
- Menú mobile, animaciones de aparición al hacer scroll (`IntersectionObserver`) y estados con `focus-visible` para navegación con teclado.
- Sin dependencias externas de imágenes — el caso de estudio usa un mockup hecho en CSS puro.

## Estructura

```
index.html   → sitio completo (una sola página)
```

## Correrlo local

No necesita build ni dependencias:

```bash
git clone https://github.com/Lissandra2009/studio39.git
cd studio39
npx serve .
```

## Nota

Proyecto en construcción — todavía no tiene sección de contacto activa.
