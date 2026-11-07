# ULTRAFAST · Guía paso a paso — FASE A (activos)
Basada en: SOP-01, lecciones 3–6 y método de Adil (Blockbuster + 8 escenas). Cada paso: dónde, qué pulsar, qué pegar, qué comprobar, coste.
Regla de siempre: **nunca generar sin mirar el coste en el botón; nunca "Permitir siempre"; una cosa cada vez.**

---
## A0 · Proyecto y carpetas (Cinema Studio) — 0 cr
Ya hecho: proyecto **ULTRAFAST** y carpeta **00-Activos**.
1. En la barra izquierda del proyecto, pasa el ratón por **00-Activos** → aparece un **+** a la derecha → púlsalo → escribe `Reloj` → Enter.
2. Repite el **+** en 00-Activos para crear `Juan` y `Adri`.
3. Pulsa **Añadir carpeta** (debajo de "Todos los recursos") y crea, una a una: `E1-Casa`, `E2-Campo`, `E3-Servidores`, `E4-Riad`, `E5-Caracas`, `E6-Paris`, `E7-Consejo`, `E8-CPD`.
✔ Comprobar: 00-Activos con 3 subcarpetas + 8 carpetas de escena.

---
## A1 · PRODUCTO = tu reloj
### A1.1 Fotos (móvil) — 0 cr
- Fondo: un folio blanco o la mesa despejada. Luz: de frente a la ventana, de día, sin sol directo (evita reflejos en el cristal).
- Móvil a la altura del reloj, sin gran angular (zoom 1x, a unos 30 cm), en horizontal.
- 5 fotos, **una vista por foto**:
  1. de frente (pantalla mirando a cámara);
  2. lateral derecho (corona y botón);
  3. lateral izquierdo;
  4. en 3/4;
  5. **puesto en la muñeca izquierda** (manga recogida, brazo apoyado en la mesa).
- Pantalla: apagada o encendida, da igual (la cambiamos).
- Guárdalas en `Retos/Corto-ULTRAFAST/reloj/` como `reloj_1_frente.jpg` … `reloj_5_muneca.jpg` y avisa: **"A1.1 listo"**. Las reviso antes de seguir.

### A1.2 Quitar el fondo sin redibujar (SuperComputer) — ~1 cr por foto
1. Menú superior → **Supercomputer** → barra izquierda → **Nuevo chat**.
2. Abajo, junto a la flecha de enviar: modelo **Auto · Gratis** y el desplegable **Preguntar ⌄** → **Preguntar antes de generar**.
3. Primer mensaje (pega las reglas de la casa del SOP y envía):
```
House rules for this chat:
- Always show me the plan, references, model, settings and cost before any generation. Never generate without my approval.
- Drafts first: images at 1K unless I ask for more.
- No automatic extra passes, no upscales unless I ask.
- One output per request unless I ask for variations.
- Change only what I name in a correction; keep everything else verbatim.
```
4. Segundo mensaje: **+** → Attach file → **Upload media** → `reloj_1_frente.jpg`, y escribe:
```
The attached photo is our PRODUCT, my smartwatch: rounded-square case, digital crown and side button on the right, sport band. Remove the background and put it on a plain light grey background. Keep it exactly as it is: same shape, colour, band and details. No redesign.
```
5. Tarjeta de aprobación: miniatura = tu foto ✔, coste ≈1 ✔ → **Aprobar** (nunca "Permitir siempre").
6. Comprueba contra el original: contorno, color, correa, corona; sin restos de fondo. Descarga → `reloj/limpio_frente.png`.
7. Repite los pasos 4–6 con `reloj_4_34.jpg` → `limpio_34.png`.

### A1.3 Hoja del reloj con la pantalla ULTRAFAST (Cinema Studio) — ~2,5–3 cr
1. Cinema Studio → proyecto ULTRAFAST → carpeta **00-Activos / Reloj** seleccionada (para que el resultado se guarde ahí).
2. Panel de abajo, a la izquierda: pestaña **Imagen** (no Video).
3. Selector de modelo → **GPT Image 2.5 Sunburst** (el que mejor escribe texto, y la pantalla lleva texto). Si el coste no te cuadra, el plan B es **Seedream 5.0 Pro**.
4. Ajustes: formato **16:9**, resolución **2K**, cantidad **1/4 → 1**.
5. **+** → sube `limpio_frente.png`, `limpio_34.png` y `reloj_5_muneca.jpg`.
6. Pega:
```
The attached photos show our PRODUCT: my real smartwatch (image 1 front, image 2 three-quarter, image 3 on my left wrist for scale). Keep the case shape, colour, crown, button and band exactly as in the photos.
Make one prop sheet on a plain neutral grey background, clean design-sheet layout: front view, left side, right side, back, three-quarter view, and one close-up of the screen.
Replace only the screen content, in every view where the screen is visible: an original navigation interface (not Apple's) with the time "18:10" at the top and three stacked buttons: "Ruta larga · 45 min", "Ruta corta · 25 min" and a third glowing electric-blue button "⚡ ULTRAFAST · NUEVO". No logos, no brand names. Photoreal product render, soft studio light, consistent proportions in every view.
```
7. Antes de **Generar**: 3 miniaturas correctas, modelo, 2K, 1 imagen, coste en el botón.
8. Revisión (en grande): ¿es TU reloj (forma, color, correa)?; ¿sin logos delante?; ¿se lee "ULTRAFAST"?; ¿las vistas son coherentes entre sí? Si falla algo → corregimos **una** cosa.

### A1.4 Crear el elemento del reloj — 0 cr
1. Barra izquierda del proyecto → **Elementos** → crear elemento → **Image Element**.
2. Imagen: la hoja buena de A1.3. Nombre: `reloj_ULTRAFAST`. Categoría: **Prop / atrezo**.
3. Comprueba: escribiendo **@** en la caja de abajo aparece `reloj_ULTRAFAST`.

### A1.5 Ficha de comportamientos (en este archivo, para la revisión)
- La pantalla siempre muestra la interfaz ULTRAFAST y la hora de cada escena (18:10 → 19:00).
- Al pulsar: flash blanco + fragmentos de luz azul eléctrico. Es una característica, no un error.

---
## A2 · CREADOR = Juan (y Adri)
### A2.1 Hoja de Juan con una sola cara (Cinema Studio) — ~2,5 cr
Motivo (Adil): si la hoja tiene caras en el cuerpo entero y en el primer plano, Seedance duda cuál copiar y la cara se desvía escena a escena.
1. Carpeta **00-Activos / Juan** seleccionada → pestaña **Imagen** → modelo **Seedream 5.0 Pro** → 16:9, 2K, 1 imagen.
2. **@** → `juancho_V1.0` (que salga como chip amarillo, no escrito a mano).
3. Pega:
```
Edit the attached character sheet of Juan. Keep his face, hair, glasses, build and clothing exactly the same. Remove the face from the full-body figure: hide it naturally (head turned away, or the face left blank and smooth) so the ONLY visible face in the whole sheet is the close-up. Replace the background with plain neutral grey. Keep the layout: full-body front, full-body back, face close-up. No text, no labels.
```
4. Revisión: cara del primer plano idéntica a la tuya (ojos marrones, gafas), cuerpo entero sin cara, fondo gris.
5. Elementos → nuevo Image Element `juancho_V2.0`, categoría **Character**.

### A2.2 Adri — 0 cr por ahora
Se usa `adri_Adri_V1.0` en la escena 8. Si en las pruebas se desvía, le hacemos lo mismo que a Juan.

---
## A3 · Fotogramas clave de cada mundo
Se hacen escena a escena al empezar la FASE B (guía aparte, con los prompts de cada mundo).
