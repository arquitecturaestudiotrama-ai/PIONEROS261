# Barrio Pioneros — Lote 261 · DFS Studio

Presentación web del proyecto de vivienda en Barrio Pioneros, Pinamar.

## Archivos

| Archivo | Qué es |
|---|---|
| `index.html` | Versión completa (computadora y tablet). |
| `celular.html` | Versión optimizada para celular. Se ve en `/celular`. |
| `favicon.svg` | Ícono de la pestaña (isotipo de DFS). |
| `vercel.json` | Configuración de Vercel (direcciones sin `.html`). |

Las imágenes, los planos y la tipografía están embebidos en cada HTML: no hay carpetas extra ni hace falta instalar nada.

## Cambio automático de versión

- Si alguien abre la dirección principal desde un celular, pasa solo a `/celular`.
- Si abre `/celular` desde una computadora, vuelve a la versión completa.
- Para forzar una versión: `?completa` (ej. `tusitio.vercel.app/?completa`) o `?celular` (ej. `tusitio.vercel.app/celular?celular`).

## Publicar

### 1. GitHub
1. Entrá a github.com → **New repository** → nombre, por ejemplo `pioneros-lote-261` → **Create repository**.
2. En la página del repositorio vacío, hacé clic en **uploading an existing file**.
3. Arrastrá **los 5 archivos** de esta carpeta (no la carpeta ni el .zip) → **Commit changes**.

### 2. Vercel
1. Entrá a vercel.com con tu cuenta de GitHub → **Add New… → Project**.
2. Elegí el repositorio `pioneros-lote-261` → **Import**.
3. Framework Preset: **Other**. No cambies nada más → **Deploy**.
4. En menos de un minuto tenés el link (`pioneros-lote-261.vercel.app`). Desde **Settings → Domains** podés ponerle un dominio propio.

Cada vez que subas un cambio al repositorio, Vercel actualiza el sitio solo.

## Editar datos de contacto

Abrí `index.html` y `celular.html` con un editor de texto, buscá `const CONTACT` y completá los valores:

```js
const CONTACT = [
  { label: "Mail", value: "estudio@ejemplo.com" },
  { label: "Instagram", value: "@usuario" },
  { label: "Teléfono", value: "+54 9 223 000 0000" }
];
```

Si un valor queda vacío, la página muestra "A completar".
