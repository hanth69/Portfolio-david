# PROJECT.md — Memoria del Proyecto: Portafolio David González

## Descripción
Portafolio web de David González, arquitecto colombiano radicado en Stuttgart.
- **URL en vivo:** https://portfolio-david-three.vercel.app
- **Repositorio:** https://github.com/hanth69/Portfolio-david
- **Carpeta local:** `C:\Users\hanth\OneDrive\Documentos\GitHub\Portfolio-david-nuevo`

---

## Estructura del Proyecto
```
Portfolio-david/
├── public/              ← Output Directory (Vercel sirve desde aquí)
│   ├── index.html       ← Archivo principal del portafolio
│   ├── foto-david.jpg
│   ├── foto-landing.jpg
│   ├── lebenslauf-de.pdf
│   ├── hoja-de-vida-es.pdf
│   └── [imágenes de proyectos]
├── server.js
├── package.json
├── package-lock.json
├── .gitattributes
└── PROJECT.md           ← Este archivo
```

---

## Reglas Críticas del Proyecto

### 1. Archivos JPG y PDF — SIEMPRE desde GitHub web
- Ir a https://github.com/hanth69/Portfolio-david
- Navegar a la carpeta `public/`
- Clic en "Add file" → "Upload files"
- Arrastrar los archivos y hacer commit directo en la web
- **NUNCA** subir binarios por terminal Git (corrupción/problemas de tamaño)

### 2. Sin Git LFS
- Vercel plan gratuito NO soporta Git LFS
- No ejecutar `git lfs` bajo ninguna circunstancia

### 3. Sin vercel.json
- El archivo `vercel.json` causaba errores de despliegue
- No crear ni modificar este archivo

### 4. Output Directory = `public`
- Configurado en el dashboard de Vercel
- Todo el HTML, CSS, JS, imágenes y PDFs van dentro de `public/`

### 5. Para archivos de texto (HTML, JS, CSS, MD)
```bash
git add .
git commit -m "descripción del cambio"
git push origin main
```

---

## Proyectos en el Portafolio (6 + 1)

| # | Proyecto | Ciudad | Año | Tipo |
|---|----------|--------|-----|------|
| 01 | Zig Zag Park | Bogotá, Colombia | 2018 | Social / Bienal |
| 02 | Klinikum Schloss Winnenden | Winnenden, BW | 2021 | Hospital — 1. Preis |
| 03 | Klinikum Ortenau Achern | Achern, BW | 2022 | Hospital — Wettbewerb |
| 04 | Universitätsklinikum Tübingen NMK | Tübingen, BW | 2022 | Hospital — 2. Preis |
| 05 | Hann & Taste Café & Bar | Barcelona | 2023 | Interiorismo |
| 06 | Holz Blockbau Ulm | Ulm, BW | 2024 | Madera ecológica |
| 07 | Bundesagentur für Arbeit Mannheim | Mannheim, BW | 2024–2026 | Dirección LP 5–8 |

---

## Stack Técnico
- HTML5 estático + CSS inline + JavaScript vanilla
- Sin frameworks ni bundlers
- Vercel (plan gratuito) — despliegue automático desde GitHub main
- Bilingüe: DE / ES con toggle JavaScript

---

## Historial de Decisiones

- **vercel.json eliminado** — causaba errores de routing
- **Git LFS descartado** — incompatible con Vercel free plan
- **Imágenes subidas vía GitHub web** — método estable para binarios
- **Output Directory = `public`** — configurado manualmente en Vercel dashboard