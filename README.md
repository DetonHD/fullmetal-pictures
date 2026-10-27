# Fullmetal Pictures &middot; Sitio Web Oficial

Sitio web profesional para la agencia de fotografía social **Fullmetal Pictures** (Venezuela).

---

## 🚀 Cómo desplegar en Vercel

El proyecto está 100% configurado para desplegar en [Vercel](https://vercel.com) sin necesidad de configuraciones adicionales.

### Opción 1: Conectar con GitHub (Recomendada)
1. Sube esta carpeta a tu repositorio en **GitHub**.
2. Entra en [vercel.com](https://vercel.com) e inicia sesión.
3. Haz clic en **"Add New..."** > **"Project"**.
4. Selecciona tu repositorio de GitHub y haz clic en **"Import"**.
5. No necesitas cambiar nada en la configuración (el archivo `vercel.json` se encarga de todo automáticamente).
6. Haz clic en **"Deploy"**. En 10 segundos tu web estará en vivo con HTTPS gratuito y CDN global.

---

### Opción 2: Desde la terminal con Vercel CLI
Si tienes Node.js instalado, puedes desplegar en 1 minuto desde la consola:
```bash
npx vercel
```
- Sigue las preguntas interactivas en pantalla (presiona Enter para los valores por defecto).
- Para subir la versión final a producción:
```bash
npx vercel --prod
```

---

### Opción 3: Arrastrar la carpeta (Vercel Drag & Drop)
1. Entra en [vercel.com/new](https://vercel.com/new).
2. Si tienes la opción de desplegar arrastrando, sube la carpeta `v2` (que contiene `index.html` y la carpeta `img/`).
3. Haz clic en **Deploy**.

---

## 📁 Estructura del Proyecto

```
FULLMETAL PICTURES/
├── vercel.json           # Configuración de rutas, rewrites y cabeceras de seguridad para Vercel
├── .gitignore            # Archivos ignorados por Git
├── robots.txt            # Instrucciones para motores de búsqueda (SEO)
├── sitemap.xml           # Mapa del sitio para indexación en Google
├── v1/                   # Versión inicial anterior (archivo histórico)
└── v2/                   # VERSIÓN 2 (Sitio de producción activo)
    ├── index.html        # Página web completa (Intro, Header, Hero, Portafolio, Precios, etc.)
    ├── vercel.json       # Configuración autónoma para v2
    ├── robots.txt
    ├── sitemap.xml
    └── img/              # Fotografías optimizadas
        ├── fotografo.jpg
        ├── wedding_dance.jpg
        ├── xv_anos.jpg
        ├── retrato_mujer.jpg
        ├── evento_brindis.jpg
        └── anillos.jpg
```

---

## ⚙️ Características Técnicas
- **Intro cinemática** con obturador SVG y sonido visual.
- **Logo rediseñado** en cabecera con efecto blur al hacer scroll.
- **Portafolio interactivo** con filtros por categoría y visor en pantalla completa (Lightbox).
- **Formulario inteligente** que redirige directo a WhatsApp con los datos del evento redactados.
- **Cabeceras de seguridad HTTP** (`X-Content-Type-Options`, `X-Frame-Options`, `X-XSS-Protection`).
- **Cache inmutable de 1 año** para imágenes estáticas en CDN de Vercel.
