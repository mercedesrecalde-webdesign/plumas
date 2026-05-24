# El Almohadón de Plumas — Escape Room de Comprensión Lectora

Experiencia interactiva sobre el cuento de **Horacio Quiroga** (1907, dominio público).
Los estudiantes leen el cuento completo y luego deben escapar de la casa resolviendo
5 salas de comprensión sobre los personajes, sus emociones y la trama.

## 📁 Estructura del proyecto

```
/ (raíz del repositorio)
├── index.html        ← el sitio completo (no requiere instalar nada)
└── images/           ← las fotos de los personajes y escenarios
    ├── casa.png        (frente de la casa)
    ├── dormitorio.png  (habitación de Alicia)
    ├── alicia.png      (Alicia enferma en la cama)
    ├── jordan.png      (Jordán, el marido)
    ├── medico.png      (el médico)
    └── parasito.png    (el parásito del almohadón)
```

> **Importante:** si alguna imagen todavía no existe, el sitio muestra
> automáticamente una ilustración de respaldo, así que **nunca se rompe**.
> Podés ir agregando o reemplazando las fotos cuando quieras: solo respetá
> los nombres de archivo de la lista de arriba y ponelas dentro de `images/`.

## 🖼️ Cómo agregar tus propias fotos

1. Generá o conseguí la imagen (libre de derechos / generada por vos).
2. Guardala con el nombre exacto de la lista (por ejemplo `alicia.png`).
3. Colocala dentro de la carpeta `images/`.
4. Listo: al recargar la página aparece sola.

(Si querés cambiar los nombres o rutas, editá el bloque `IMGFILES` dentro de `index.html`.)

## 🚀 Deploy en GitHub + Cloudflare Pages

### 1) Subir a GitHub
1. Creá un repositorio nuevo en https://github.com (por ej. `almohadon-escape`).
2. Subí **`index.html`** y la **carpeta `images/`** (botón *Add file → Upload files*,
   arrastrás todo y *Commit changes*).

### 2) Publicar con Cloudflare Pages
1. Entrá a https://dash.cloudflare.com → **Workers & Pages** → **Create** → **Pages**
   → **Connect to Git**.
2. Autorizá GitHub y elegí tu repositorio `almohadon-escape`.
3. En la configuración de build dejá todo vacío:
   - **Framework preset:** *None*
   - **Build command:** *(vacío)*
   - **Build output directory:** `/`  (la raíz)
4. **Save and Deploy**.
5. En segundos tendrás una URL pública del tipo
   `https://almohadon-escape.pages.dev` para pegar en tu trabajo práctico.

### Alternativa rápida: GitHub Pages
1. En el repo: **Settings → Pages**.
2. *Source:* **Deploy from a branch**, rama `main`, carpeta `/root`.
3. Guardá: te da una URL `https://TU-USUARIO.github.io/almohadon-escape/`.

## 🎵 Sonido
La música y los efectos se generan en el navegador con Web Audio API
(ambiente, viento y un latido que se acelera). No usa archivos de audio:
es 100% libre de derechos. Se activa con el botón ♪ (arriba a la derecha).

## ⚖️ Derechos
- El cuento es de **dominio público** (Quiroga falleció en 1937).
- El sonido y las ilustraciones de respaldo son originales (generados por código).
- Las fotos que agregues deben ser de tu autoría, generadas por vos, o de uso libre.
