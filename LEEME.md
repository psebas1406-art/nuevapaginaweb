# Subir esta página a GitHub Pages

Cada página es **un solo archivo**: el diseño, las animaciones, las fuentes, los íconos, tu foto y tu video van dentro. No hay carpetas.

Archivos que debes subir (los 6 `.html`):

- `index.html` (la página principal)
- `privacidad.html`, `cookies.html`, `terminos.html` y `reembolsos.html` (documentos legales)
- `404.html` (la página de "no encontrada")

## Pasos

1. Entra a https://github.com/new, crea un repositorio **público** (por ejemplo `mi-web`) y pulsa **Create repository**.
2. Haz clic en **"uploading an existing file"** y luego en **"choose your files"**.
3. En esta carpeta selecciona los **6 archivos `.html`** (Ctrl + clic en cada uno) y pulsa **Abrir**.
4. Espera a que suban (`index.html` pesa 1,3 MB porque lleva el video dentro) y pulsa **Commit changes**.
5. Ve a **Settings → Pages**. En "Branch" elige `main` y la carpeta `/ (root)`, y pulsa **Save**.
6. En uno o dos minutos tu página queda en `https://TU-USUARIO.github.io/mi-web/`.

Si antes subiste otros archivos (carpetas `css`, `js`, `assets`…), puedes dejarlos: ya no se usan.

## Qué funciona aquí

- ✅ Toda la página, animaciones, partículas, scroll y documentos legales. También con doble clic en tu computador.
- ✅ Banner de cookies (la decisión queda guardada en el navegador del visitante).
- ✅ Formulario de contacto: abre el correo del visitante con su mensaje y las casillas que marcó, listo para enviarte. **Guarda esos correos**: son tu prueba de las autorizaciones.
- ❌ No hay panel de admin ni registro automático de consentimientos con IP. Para eso se necesita la versión con servidor (carpeta `codex`, publicada en Render).

## Cambiar algo

No edites estos archivos a mano. Haz el cambio en la carpeta principal (`mi web/public` o `mi web/config.json`) y vuelve a generar estas páginas con:

```
node build-pages.js
```

Después sube de nuevo los 6 archivos a GitHub. GitHub te preguntará si quieres reemplazarlos: acepta.
