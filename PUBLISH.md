# Publicar Sinestesia

Tres caminos, de más rápido a más completo. En todos, conviene que la raíz del
sitio sirva un `index.html`. Lo más simple: renombra el archivo.

```
# desde la carpeta del proyecto
cp sinestesia.html index.html      # o: mv sinestesia.html index.html
```

(Si lo renombras a `index.html`, actualiza también este documento mentalmente: el
archivo a servir es ese.)

---

## 1) Netlify Drop — sin terminal, en segundos

1. Entra a https://app.netlify.com/drop
2. Arrastra el archivo `index.html` (o toda la carpeta) a la página.
3. Te da una URL pública al instante. Listo.

Bueno para enseñarlo ya. Para un dominio bonito y actualizaciones, usa la opción 2 o 3.

---

## 2) GitHub Pages — gratis y permanente

Requiere una cuenta de GitHub. Desde la carpeta del proyecto:

```
git init
git add .
git commit -m "Sinestesia: primera publicación"
# crea un repo vacío en github.com (ej. tu-usuario/sinestesia) y luego:
git remote add origin https://github.com/TU-USUARIO/sinestesia.git
git branch -M main
git push -u origin main
```

Después, en GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a
branch → Branch: main / root → Save.**

En 1-2 minutos tu sitio queda en `https://TU-USUARIO.github.io/sinestesia/`.

> Pídele a Claude Code: *"sube esto a un repo de GitHub y activa GitHub Pages, dame la URL"*.

---

## 3) Vercel — rápido, con dominio y futuros backends

```
npm i -g vercel      # si no lo tienes
vercel               # sigue las preguntas; acepta los valores por defecto
vercel --prod        # publica a producción
```

Vercel es buena opción si más adelante añades una **función serverless** para activar
la IA garantizada (guardando `ANTHROPIC_API_KEY` como variable de entorno en el panel
de Vercel, nunca en el cliente). Ver `CLAUDE.md` → "Limitación conocida".

---

## Después de publicar

- Abre la URL y prueba **copiar enlace**: debe reconstruir tu pieza al abrirlo.
- Prueba **guardar pieza** y recargar: si el entorno persiste, la galería sigue ahí.
- Comparte el enlace o el PNG de **guardar imagen**.
