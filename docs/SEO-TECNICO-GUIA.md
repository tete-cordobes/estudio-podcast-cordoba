# GUÍA SEO TÉCNICO - Optimización para Google y LLMs

## Fecha: 27 Diciembre 2025

---

# 1. ANÁLISIS DEL HTML ACTUAL

## Lo que YA tienes bien:
- [x] `<!DOCTYPE html>` y `<html lang="es">`
- [x] Meta charset y viewport
- [x] Title y meta description
- [x] Open Graph tags
- [x] Twitter Cards
- [x] Schema.org LocalBusiness
- [x] Schema.org FAQPage
- [x] Canonical URL
- [x] Geo meta tags
- [x] Lazy loading en imágenes

## Lo que FALTA o se puede mejorar:
- [ ] Preload de recursos críticos
- [ ] Atributos width/height en imágenes (CLS)
- [ ] Schema Organization
- [ ] Schema Service
- [ ] Schema BreadcrumbList
- [ ] Archivo robots.txt
- [ ] Archivo sitemap.xml
- [ ] Archivo llms.txt (nuevo estándar para LLMs)
- [ ] Más HTML semántico (article, main, aside)
- [ ] Atributos ARIA mejorados
- [ ] Hreflang (si multiidioma)
- [ ] Meta theme-color
- [ ] Manifest.json (PWA)

---

# 2. HEAD OPTIMIZADO COMPLETO

```html
<!DOCTYPE html>
<html lang="es" dir="ltr">
<head>
    <!-- Charset y Viewport - PRIMERO -->
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">

    <!-- Preconnect a recursos externos - ANTES de cargarlos -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link rel="preconnect" href="https://cdn.tailwindcss.com">

    <!-- DNS Prefetch para recursos secundarios -->
    <link rel="dns-prefetch" href="https://www.google-analytics.com">
    <link rel="dns-prefetch" href="https://www.googletagmanager.com">

    <!-- Preload recursos críticos -->
    <link rel="preload" href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap" as="style">

    <!-- SEO Primario -->
    <title>Estudio de Podcast en Córdoba | Alquiler Grabación Profesional Audio y Video</title>
    <meta name="description" content="Alquila el estudio de podcast #1 en Córdoba. Grabación profesional de audio y video 4K con micrófonos Shure SM7B. Sets premium desde 50€/hora. Reserva ahora.">

    <!-- SEO Secundario -->
    <meta name="keywords" content="estudio podcast cordoba, alquiler estudio podcast, grabar podcast cordoba, estudio grabacion cordoba">
    <meta name="robots" content="index, follow, max-image-preview:large, max-snippet:-1, max-video-preview:-1">
    <meta name="googlebot" content="index, follow">
    <meta name="bingbot" content="index, follow">

    <!-- Canonical y alternates -->
    <link rel="canonical" href="https://podcastcordoba.es/">
```

---

# 3. CORE WEB VITALS

## Métricas objetivo

| Métrica | Objetivo | Acción |
|---------|----------|--------|
| LCP (Largest Contentful Paint) | < 2.5s | Optimizar imagen hero, preload |
| FID (First Input Delay) | < 100ms | Defer JS no crítico |
| CLS (Cumulative Layout Shift) | < 0.1 | Width/height en imágenes |
| INP (Interaction to Next Paint) | < 200ms | Optimizar event handlers |

---

# 4. CHECKLIST FINAL SEO TÉCNICO

## Implementación obligatoria
- [ ] DOCTYPE HTML5
- [ ] lang="es" en <html>
- [ ] Meta charset UTF-8
- [ ] Meta viewport responsive
- [ ] Title único y descriptivo (50-60 chars)
- [ ] Meta description (150-160 chars)
- [ ] Canonical URL
- [ ] H1 único con keyword principal
- [ ] Jerarquía H1 > H2 > H3 correcta
- [ ] Alt text en todas las imágenes
- [ ] Width/height en imágenes
- [ ] Lazy loading en imágenes below fold
- [ ] Schema.org LocalBusiness
- [ ] Schema.org FAQPage
- [ ] robots.txt
- [ ] sitemap.xml
- [ ] Favicon completo

## Implementación recomendada
- [ ] Open Graph tags completos
- [ ] Twitter Card tags
- [ ] Preconnect/preload recursos críticos
- [ ] HTML semántico (main, article, section)
- [ ] ARIA labels para accesibilidad
- [ ] Skip links
- [ ] Schema Organization
- [ ] Schema BreadcrumbList
- [ ] llms.txt para AI crawlers
- [ ] Manifest.json (PWA)
- [ ] theme-color meta

## Para producción
- [ ] HTTPS obligatorio
- [ ] Compresión GZIP/Brotli
- [ ] Cache headers
- [ ] CDN para assets
- [ ] Minificación CSS/JS
- [ ] Google Search Console verificado
- [ ] Google Analytics 4 instalado
- [ ] Core Web Vitals < umbrales

---

*Documento generado: 27/12/2025*
*Referencia: Google SEO Starter Guide 2025, Schema.org, Web.dev*
