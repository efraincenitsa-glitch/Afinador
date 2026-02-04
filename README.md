# Afinador de Cuerdas (PWA)

Afinador cromático para guitarra, bajo (4/5), violín, viola, cello, ukelele y mandolina. **Notas en español** (Do, Re, Mi, Fa, Sol, La, Si). Funciona como **PWA**, se puede **agregar a pantalla de inicio** en iPhone y Android.

## 🧩 Contenido
- `index.html` — App completa (UI + detección de tono + PWA)
- `manifest.webmanifest` — Manifest con iconos 192/512/1024
- `sw.js` — Service Worker (cache-first)
- `icons/` — Iconos PNG (`180`, `192`, `512`, `1024`)

## 🚀 Cómo desplegar en GitHub Pages
1. Crea un repositorio (por ejemplo `afinador-pwa`).
2. Sube **todos** los archivos de esta carpeta.
3. Activa **Settings → Pages → Deploy from branch** (main / root o `/docs`).
4. Abre la URL que te indique Pages (normalmente `https://<usuario>.github.io/<repo>/`).

> Las rutas son **relativas**, así que funcionan tanto en la raíz como en una subcarpeta (Project Pages).

## 📱 Agregar a pantalla de inicio (iPhone)
1. Abre la URL en **Safari** (importante: debe ser **HTTPS**).
2. Toca **Compartir** → **Agregar a pantalla de inicio**.
3. Confirma el nombre ("Afinador").

## 🎤 Permisos de micrófono
- iOS/Safari exige **gesto del usuario** para iniciar el audio → usa el botón **Iniciar micrófono**.
- iOS requiere **HTTPS** o `localhost` para habilitar `getUserMedia`.

## 🛠️ Notas técnicas
- Detección de tono por **autocorrelación** en señal temporal (50–1500 Hz).
- Calibración **La4 (A4)** ajustable 415–466 Hz.
- Afinaciones incluidas: guitarra, bajo 4/5, violín, viola, cello, ukelele, mandolina, modo cromático.

## ✏️ Personalización
- Si quieres añadir **afinaciones alternativas** (Drop D, DADGAD, etc.) o mostrar **bemoles (♭)** en vez de sostenidos (♯), edita `index.html` y escríbeme para generarlo automáticamente.

---
© 2026. José y colaboradores.
