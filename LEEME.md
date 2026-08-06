# Consulta de autorización de transporte (PWA)

App web instalable en el móvil. Modo B: abre la web oficial del Ministerio y muestra la matrícula en grande para escribirla/pegarla allí. No lee, no interpreta ni guarda ningún dato.

## Archivos
- `index.html` — la app (pantalla única).
- `manifest.webmanifest` — datos de instalación.
- `sw.js` — service worker (permite instalarla).
- `icon-192.png`, `icon-512.png`, `icon-512-maskable.png` — iconos.

## Subir a GitHub Pages (cuenta taxienalicante)
1. Entra en GitHub con la cuenta **taxienalicante**.
2. Crea un repositorio nuevo, p. ej. `autorizacion`, **público**.
3. Sube **todos** estos archivos a la raíz del repo (arrastrar y soltar en "Add file → Upload files" → Commit).
4. Settings → **Pages** → Source: `Deploy from a branch` → Branch: `main` / carpeta `/ (root)` → Save.
5. Espera ~1 minuto. La URL será: `https://taxienalicante.github.io/autorizacion/`

## Instalar en el móvil
- Abre esa URL en el navegador del teléfono.
- Menú → "Añadir a pantalla de inicio" (Android/Chrome) o Compartir → "Añadir a pantalla de inicio" (iPhone/Safari).

## Notas
- El lector por foto (OCR) necesita conexión la primera vez (descarga el motor). Si no lee bien, escribe la matrícula a mano; siempre es editable.
- La cámara y la instalación requieren HTTPS: GitHub Pages ya lo da.
- El CAPTCHA del Ministerio lo resuelve la persona en su web. La app no lo toca.
