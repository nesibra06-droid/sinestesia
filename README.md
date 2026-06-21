# Sinestesia

Un sentimiento, leído por la ciencia, traducido a sonido y luz.

Escribes un sentimiento, un momento o un lugar ("nostalgia de domingo por la tarde",
"euforia de neón en la ciudad") y Sinestesia genera una pieza audiovisual en tiempo
real: un paisaje sonoro que evoluciona y un campo de luz que reacciona a la música.

## Cómo funciona

El texto pasa por un motor que **mide el afecto** (valencia y activación, el modelo
circumplejo de Russell) y de ahí deriva, con mapeos basados en investigación, el
modo musical, el tempo, la articulación y la paleta de color, además del tipo de
visual (lluvia, brasas, aurora, escarcha, pulso, olas…).

Todo ocurre en el navegador, en un solo archivo. Una capa de IA opcional añade el
título y la descripción poéticos cuando está disponible.

## Probarlo

Abre `sinestesia.html` en el navegador, o sírvelo localmente:

```
python3 -m http.server 8000
# http://localhost:8000/sinestesia.html
```

El audio arranca con el primer clic (los navegadores lo exigen).

## Publicarlo

Ver `PUBLISH.md`. La forma más rápida sin configurar nada: arrastrar el archivo a
netlify.com/drop. Para algo permanente y editable: GitHub Pages, Netlify o Vercel.

## Créditos científicos (referencias del mapeo)

- Russell (1980), modelo circumplejo del afecto — valencia × activación.
- Juslin & Västfjäll; Hevner — emoción ↔ rasgos musicales (modo, tempo, articulación).
- Valdez & Mehrabian (1994) — emoción ↔ color (matiz, saturación, luminosidad).
- Spence (2011); Marks — correspondencias crossmodales (tono↔brillo, tempo↔movimiento).
