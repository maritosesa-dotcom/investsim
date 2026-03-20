# InvestSim 📈

Simulador de inversiones PWA para iPhone con análisis IA via Claude.

## Archivos

- `index.html` — La app completa
- `manifest.json` — Configuración PWA
- `sw.js` — Service Worker (offline)

> Los iconos (`icon-192.png`, `icon-512.png`) los tienes que generar tú o usar cualquier imagen PNG.

---

## Despliegue en GitHub Pages

1. Crea un repositorio en GitHub (ej: `investsim`)
2. Sube los 3 archivos (+ iconos)
3. Ve a Settings → Pages → Branch: main → Save
4. La app estará en: `https://tuusuario.github.io/investsim/`

---

## Configurar el Cloudflare Worker (IA)

1. Ve a [dash.cloudflare.com](https://dash.cloudflare.com)
2. **Workers & Pages → Create → Create Worker**
3. Borra el código de ejemplo y pega el código que aparece en la app (pestaña Config → "Copiar código del Worker")
4. **Deploy**
5. Ve a **Settings → Variables → Environment Variables**
6. Añade: `ANTHROPIC_API_KEY` = tu API key de Anthropic
7. Copia la URL del Worker (ej: `https://investsim.tuusuario.workers.dev`)
8. Pégala en la app → pestaña **Config** → guarda

---

## Instalar como app en iPhone

1. Abre la URL en Safari
2. Botón compartir → "Añadir a pantalla de inicio"
3. ¡Listo!
