# Higgsfield Academy · Guías PDF de las lecciones 4 y 5 (leídas enteras)

Fuente: PDF oficiales descargados por Navegante el 7-11-2026 (carpeta Descargas/HF) y leídos completos:
- L4 "Create and Edit Assets" (31 p.)
- L5 "Shot Sizes & Prompting" (9 p.)
- L5 "Camera — Shot sizes, angles & movement" (20 p.)
La biblioteca de prompts de la L4 (27 p., 26 prompts completos: 6 Soul Cinema, 5 Seedream 5.0 Pro, 13 GPT 2.5 Sunburst, 2 Nano Banana Pro) va aparte en `Academy-L4-Biblioteca-prompts.md` (texto extraído tal cual del PDF).
Notas en castellano; los prompts y las cláusulas van literales en inglés porque son para pegar.

---

## L4 · Crea y edita recursos

### Glosario que usa el curso
Rango tonal · seguimiento del prompt · texto→imagen · imagen→imagen · "AI slop" (texturas raras, detalles repetidos, objetos sin sentido) · look CGI (puede ser un estilo buscado) · **ancla espacial** (objeto visible para situar la acción: "sienta al personaje junto a la jarra en el centro de la barra") · **contraplano / reverse angle** · profundidad de campo · bokeh.

### Qué revisar de cada modelo
| Modelo | Puntos fuertes | Qué comprobar |
|---|---|---|
| Soul Cinema | Luz fotográfica, piel y tela naturales, acabado de película, rango tonal amplio que aguanta en vídeo | La interpretación creativa mueve la composición; colocación de objetos; objetos pequeños rotos; detalle perdido en sombras de noche. Con imagen de entrada reinterpreta, no edita localmente |
| Seedream 5.0 Pro | Arquitectura, entornos grandes, color estilizado. **Edita imágenes enteras** (personas, objetos, ropa, fondos) conservando calidad y texturas | Briefs densos → look CGI; formas repetidas con mismo tamaño y espaciado |
| GPT 2.5 Sunburst | Sigue instrucciones al detalle, texto legible, tipografía, infografías, storyboards (lápiz, malla gris 3D, ilustrado) | Localizaciones sobrecargadas, sobre-nitidez y ruido; revisar el texto letra a letra y la continuidad entre viñetas |
| Nano Banana Pro | Generalista, sigue bien el brief | Acabado artificial por defecto, nitidez uniforme que aplana, reflejos llamativos, caras idealizadas parecidas |

### "Spot the slop": qué mirar ampliando la imagen
- Cielo: cantidad y reparto del grano o ruido (si lo pediste, no es error; si quieres limpio, cambia esa instrucción).
- Tejados y madera: bordes demasiado nítidos y detalle fino repetido = sensación de render.
- Césped: textura densa y repetida que aplana la profundidad.
- Patrones naturales (salinas): la repetición es normal; lo sospechoso es misma forma, tamaño y espaciado.
- Suelos mojados: reflejos que roban atención al sujeto.

### Personaje con AI Director (pasos de la guía)
1. Cinema Studio → AI Director (barra izquierda, Tools).
2. Skills → escribir "char" → Character Sheet.
3. Brief corto (papel, edad aproximada, ropa) → enviar → 5 castings → elegir → responder vestuario → hoja frente / espalda / retrato.
- Soul 2.0 hace los castings; Seedream construye la hoja.
- **Referencia preparada:** se tapa la cara pequeña para que no compita con el retrato grande. No cambia la cara del personaje.

**Prompt de hoja de personaje (desde una foto):**
```
Create a three-panel character sheet using the attached image as the identity and outfit reference: full-body front on the left, full-body back in the middle, and a three-quarter portrait from head to upper chest on the right. Preserve the person's face, age, build, haircut, black leather jacket, dark ribbed crew-neck top, silver hoop earring and other visible accessories. Keep the same identity, outfit and proportions across all panels. Complete the unseen lower outfit with full-length, straight-leg charcoal riding jeans and matte-black leather ankle-height motorcycle boots with rounded toes and low rubber soles. Match the jeans and boots in both full-body views. Use a seamless pure-white studio background with soft contact shadows. Remove the original environment and props. Show the full figure from head to shoes with space around it. Use a neutral stance, arms relaxed at the sides, empty hands and a calm, closed-mouth expression. The back view faces fully away; the portrait clearly shows the face. Use soft, even, neutral lighting, low contrast, subtle optical diffusion and natural skin and fabric texture. Preserve the outfit's colours.
```

**Edición de vestuario en Seedream 5.0 Pro:** adjuntar el original, describir el cambio y lo que se queda, **mismo aspecto y resolución que el original**. En una hoja multivista el cambio debe salir igual en todas las vistas.
```
Give him a silver wallet chain hanging off his jeans pocket. Replace the black t-shirt with a plain white ribbed cotton tank top, same tank top in all views
```

**Personaje con tu cara + ropa de otra imagen (roles por imagen):**
```
Create a three-panel character sheet: full-body front on the left, full-body back in the middle, and a three-quarter portrait from head to upper chest on the right.
Use @Image1 only for identity. Preserve Adil's face, age, build, short dark curls, moustache, small goatee, earrings and fine necklace. Use @Image2 only for clothing; do not transfer that person's face or identity.
Replace Adil's black T-shirt with the outfit from @Image2 : a black armored leather motorcycle jacket with ribbed shoulders, reinforced arms and elbows, a snap-tab stand collar, asymmetric chest panels and an open front zipper; a slate-gray crew-neck T-shirt; and gray jeans. Complete the jeans as full-length, straight-leg riding jeans over matte-black leather ankle boots with rounded toes and low rubber soles. Keep the clothing, proportions and jewelry consistent across all views, including the jacket's back.
Use a seamless pure-white studio background, soft contact shadows and no reference-scene objects. Keep the full-body figures visible from head to shoes, with relaxed arms, empty hands and a neutral, closed-mouth expression. Use soft, even, neutral lighting, low contrast, subtle optical diffusion and natural skin and fabric texture. Preserve the clothing colours.
```

### Localización
- Base en Soul Cinema con el sitio vacío (así se juzga mejor la arquitectura y el espacio útil). Se elige la que sirve a la escena, no la más elaborada.
- Ediciones sobre la misma imagen base (Seedream 5.0 Pro):
```
Add eight dive bar regulars - a mix of men and women. Some are playing pool, others are sitting at tables. Keep all bar stools empty, and place a single mug of beer in the middle of the bar counter.
```
```
Use the attached image as the reference. Show the same bar from the opposite end, looking back towards the entrance. Make the entrance door clearly visible. Keep the existing chairs and bar stools, preserving their designs and positions within the room. Maintain the bar's layout, furniture, materials, lighting and atmosphere. Change only the camera viewpoint.
```
- Comprobar el número de personas y su sitio; en el contraplano, la continuidad (puerta, barra, taburetes). Lo nuevo que invente no estaba necesariamente en la sala original.

### Técnica secreta: de referencia a Soul Cinema
1. Componer la escena con un modelo obediente (en la guía, **GPT 2.5 Sunburst** con prompts muy detallados de salón y biblioteca).
2. Soul Cinema → arrastrar esa imagen al cuadro de prompt (el texto queda bloqueado) → Generate.
3. Soul Cinema hace variaciones del mismo concepto y arquitectura con texturas naturales, luz expresiva y profundidad fotográfica. Detalles y encuadre pueden cambiar. La guía enseña 6 resultados por imagen fuente.
Los dos prompts fuente completos (salón soleado y biblioteca nocturna) están en la biblioteca.

### Fórmula de prompt para Seedream 5.0 Pro (6 pasos, 60–90 palabras orientativas)
1. **Nombra la imagen y el sitio:** empezar con "An empty photographic view of…" + 2–3 elementos concretos y sus materiales.
2. **Para qué es el espacio:** "ample dry open floor for fifteen dancers", "central open standing space allowing circular camera movement" (le dice dónde dejar espacio útil).
3. **Cámara concreta:** posición, altura, dirección y lente ("centered at the near threshold, 1.4 m high, frontal view, 24 mm spherical lens"). Una sola configuración.
4. **De dónde viene la luz:** fuente y dirección, y la zona de sombra si importa. Nada de "cinematic lighting".
5. **Acabado y material:** paleta corta, grano si se quiere, una o dos texturas tangibles. Mejor que "beautiful, ultra-detailed, 8K".
6. **Exclusiones relevantes al final:** "No people, water, writing or logos." Aspecto y resolución en los controles, no en el texto.
Ejercicio: mismo sitio y propósito, cambiar solo la altura de cámara y comparar.
```
An empty photographic view of a dense green woodland clearing: tall straight trunks and layered leaves, overcast daylight filtering from above. Low close camera at 0.6m looking toward central open standing space, near foliage encircling frame edges and allowing circular camera movement. 24mm spherical lens, rich natural greens, neutral midtones, mild analog grain, tactile bark and leaf veins. No people, writing or logos.
```

### CINEIMAGE: instalación según la guía
- Claude: Customize → Skills → Add → Upload skill → arrastrar `cineimage-soul.zip` → Upload. Se llama con `/cineimage` → cineimage-soul.
- Supercomputer: Skills (barra izquierda) → Create new → Upload a skill → arrastrar el zip → revisar nombre → Save. Se llama con `/cineimage`.
- Uso: "An empty neighbourhood cafe just before opening, viewed from the entrance. Warm side light, worn wood and a clear path to the counter." Con referencia: "Keep this room's architecture and camera angle; make the light feel like early morning."

---

## L5 · Tamaños de plano y prompting

### Glosario
Movimiento de cámara · scene context · **toma (take)** = una generación de la escena, puede tener varios planos · ángulo · tamaño de plano · continuidad · **Element** (asset guardado que se llama con @) · **plano (shot)** = vista continua entre cortes.

### Encuadre
- Plano general = sitio; plano medio = deja sitio al gesto; MCU = cabeza y pecho; primer plano = la cara manda.
- Profundidad en 3 capas (en el bar: taburetes cerca, gente en medio, billar al fondo). La regla de tercios es guía, no obligación.

### Roles de las referencias
- Persona: identidad y ropa; nombrar quién hace cada acción.
- Atrezo: forma, color, detalles; de quién es y cómo está orientado.
- Sitio: espacio, luz y color; el encuadre se especifica aparte.
- **Escribir "@algo" no adjunta nada:** hay que seleccionar el Element.
- "La imagen da el aspecto; el prompt da la propiedad, la posición y la acción."
```
@character_1 and @character_2 are the two people. @prop_1 is the object carried by @character_1. @location_1 defines the setting. Keep each person and the object consistent with their references.
```

### Planos y tiempos (4 pasos)
1. Definir la acción: estado inicial, cambios visibles y final, en orden y con quién actúa.
2. Elegir la vista por beat: manos y objetos visibles en una interacción; más cerca cuando manda la reacción.
3. Cortes y movimiento: cada corte, número de plano nuevo; dentro del plano, cámara fija o movimiento con destino.
4. Tiempo: inicio y fin por plano, contando acción, diálogo y pausa final. El último tiempo = la duración elegida.
Tamaño, ángulo y movimiento son tres decisiones separadas.

### Plantilla de escena (copiar y adaptar)
```
SCENE CONTEXT
@character_1 and @character_2 are in @location_1. Starting state: [positions and situation]. Action and ending: [what changes, in order, and the visible outcome].

REFERENCES
@character_1 and @character_2: identity and clothing. @prop_1: object appearance; carried by @character_1. @location_1: space, light and colour.

SHOTS
Shot 1, [start-end time]: [shot size and angle]. Camera: [static, or movement with a destination]. @character_1 [visible action]. Shot 2, [start-end time]: [next view and camera behaviour]. @character_2 [action or reaction]. @character_2 says: "[dialogue]".

CONTINUITY & SOUND
@prop_1: [position and orientation, if needed]. [Other details that must stay consistent]. [Ambience, action sounds and music instruction]. [Final hold, if needed].
```
Antes de generar: duración = último tiempo; revisar assets, encuadre, audio y coste. Plano nuevo solo si quieres corte; quitar referencias y secciones que no se usan; scene context y planos deben contar la misma secuencia.

### Pedir a un LLM que repare el prompt
```
Revise the tested prompt below. What went wrong: [describe the errors]. What I want instead: [describe the intended result]. Keep the parts that already work. Update every affected line so the instructions agree. Return the full revised prompt, then list exactly what you changed or added and why.
Tested prompt: [paste the original prompt].
```
Vale con Claude, ChatGPT, Gemini o AI Director. Luego leer el prompt y la lista de cambios (que no meta acciones ni movimientos no pedidos) y ver la toma nueva entera con sonido.

### Qué arreglar (árbol de decisión)
Revisar 3 cosas: acción (¿la persona correcta hizo lo previsto?), continuidad (¿se reconocen personas, atrezo y sitio?), cámara (¿el encuadre deja ver la acción?). ¿El error se repite en varias tomas?
- **Sí → mirar prompt y assets primero.**
  - 01 Arreglar el asset: el defecto ya está en la referencia. Corregir esa imagen; no intentar borrarlo con palabras.
  - 02 Arreglar el prompt: actúa quien no es, el atrezo está mal o la cámara tiene órdenes contradictorias. Nombrar al actor, fijar el orden, que las líneas cuadren.
- **No → 03 Generar otra toma:** entradas claras pero un defecto aislado (o quieres otra puesta en escena). Quedarse el original y comparar el clip nuevo entero.

---

## L5 · Cámara: tamaños, ángulos y movimiento (cláusulas listas)

### Tamaños de plano
| Plano | Para qué | Cláusula |
|---|---|---|
| Extreme wide / EWS | El sitio manda, persona diminuta; geografía, aislamiento | `Extreme wide shot; keep the subject small within the surrounding environment.` |
| Wide / WS-LS | Persona entera con aire; entradas, movimiento, relaciones | `Wide shot; full figure with open space around them.` |
| Full shot / FS | De cabeza a pies; presentar personaje, postura, andar, baile | `Full-body shot; keep the head and feet inside the frame.` |
| Medium long / MLS | De cabeza a rodillas; diálogo de pie, gesto de manos y piernas | `Medium long shot; frame the person from head to knees.` |
| Cowboy | Cabeza a medio muslo; manos y cadera visibles, alcance, duelo | `Cowboy shot; head to mid-thigh, hands visible.` |
| Medium / MS | Cintura arriba; diálogo y acciones simples | `Medium shot; waist-up, camera at eye level.` |
| Medium close-up / MCU | Cabeza, hombros y pecho; diálogo íntimo | `Medium close-up; head and shoulders, chest at the lower edge.` |
| Close-up / CU | La cara domina; reacción, reconocimiento | `Close-up of the face; blurred background.` |
| Extreme close-up / ECU | Un detalle: ojo, dedo, pieza clave | `Extreme close-up of the key detail; exclude the surrounding context.` |
Ojo: el tamaño de plano no es la lente. Primero el límite del encuadre; la lente después.

### Ángulos
| Ángulo | Efecto | Cláusula |
|---|---|---|
| Eye level | Encuentro directo; base para diálogo | `Eye-level camera; lens at the subject's eye height.` |
| High angle | Más suelo; persona pequeña o expuesta | `Camera above the subject, looking down.` |
| Low angle | Figura o edificio imponente | `Low camera position, looking upward.` |
| Overhead / top-down | Mapa de posiciones y rutas; puede ser fijo | `Directly overhead; camera looking straight down.` |
| Dutch angle | Horizonte en diagonal; inquietud | `Dutch angle; a clearly diagonal horizon.` |
Ángulo y movimiento son decisiones separadas.

### Movimientos
| Movimiento | Qué hace | Cláusula |
|---|---|---|
| Pan | Gira en horizontal desde un punto fijo (desplazarse de lado sería truck) | `Pan right at an even pace from a fixed position; keep the horizon level and settle on the new view.` |
| Tilt | Gira en vertical sin subir la cámara | `Tilt smoothly upward from a fixed position; keep the camera at the same height and stop on the upper subject.` |
| Rise (pedestal/boom) | Cambia la altura; revela lo que tapaba el primer término | `Raise the camera vertically at an even pace; keep the lens level and finish on a higher view.` |
| Dolly in / out | Se acerca o aleja físicamente (cambia la relación primer término-fondo; el zoom no) | `Dolly slowly forward to a closer view; keep focal length and camera height fixed, with the subject near centre.` |
| Truck | Lateral; paralaje que revela | — |
| Tracking | Viaja con el sujeto a su ritmo | `Track parallel to the moving subject at a matching pace; keep a steady distance and consistent framing.` |
| Arc | Rodea al sujeto (que no gire él en la primera prueba) | `Arc from a side view to a frontal view at a steady distance; the subject stays still.` |
| Zoom | Cambia el campo de visión desde el mismo sitio | `Increase focal length smoothly from a fixed camera position; finish on a tighter frame of the subject.` |
| Dolly zoom | Retrocede y hace zoom: el sujeto igual, el fondo crece | `Move the camera backwards while zooming in; keep the subject the same size in frame.` |
| Static | Encuadre fijo, la acción cambia | `Locked-off camera; keep the composition fixed while the action unfolds.` |
| Handheld | Sensación física | `Restrained handheld drift; keep the subject clearly framed.` |
| Roll | Gira sobre el eje de la lente | `Slow clockwise camera roll from a level frame.` |
| Whip pan | Giro rápido con desenfoque | `Whip pan right with brief motion blur; settle on a sharp, readable final frame.` |

### Ponerlo en palabras
- Imagen fija: encuadre primero, luego ángulo. Ej.: `Medium close-up, eye-level camera. Keep the main subject clearly separated from the background.`
- Plano en movimiento: recorrido, ritmo, qué se mantiene y composición final. Ej.: `Begin with a medium shot. Slowly dolly in to a close-up, keeping the subject in the same frame position.`
- Secuencia de 3 planos: Wide (establece sujeto y espacio) → Medium (gesto legible) → Close-up (termina en la reacción).
- Cambiar una decisión de cámara cada vez en las pruebas.

### Soul Directory (el "cheat code")
**soul-directory.higgsfield.app** · biblioteca interactiva con 33 estilos, 46 movimientos de cámara y 24 montajes de luz, cada uno con ejemplo visual y prompt copiable. Tiene Shot Builder (movimiento + estilo + luz + tu escena → un prompt, con botón para pasar a vídeo en Higgsfield) y un simulador de luz 3D que escribe el prompt de iluminación. Ejercicio: misma escena, comparar dolly frente a zoom.
