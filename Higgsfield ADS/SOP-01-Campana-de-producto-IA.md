# SOP-01 · Campaña de producto con IA (de una foto a fotos + vídeos)

**Versión:** 1.0 · 25-10-2026
**Origen:** Higgsfield Academy, Lección 3 (método de Adil) + dos ejecuciones reales: gafas de ciclismo en Cádiz (25-10) y gafas geek con Adri en París (25-10).
**Herramienta probada:** Higgsfield SuperComputer. **El método es independiente de la herramienta**: cada paso dice *qué* hay que conseguir; el modelo es intercambiable.
**Siguiente evolución:** convertir cada fase en una skill (.md) propia y cargarla en Picasso.

---

## 0. Principio

**Primero se fijan los activos y después se produce.** Un modelo combina bien lo que está fijado y se inventa lo que no. Hay tres activos fijos:

| Activo | Qué es | Sin él… |
|--------|--------|---------|
| **PRODUCTO** | La foto fiel del objeto | El producto cambia de forma o de color |
| **CREADOR** | La hoja de personaje | La persona cambia de cara entre piezas |
| **LOCALIZACIÓN** | Una imagen del sitio, vacía | Cada pieza parece de una campaña distinta |

Bucle de trabajo en cada paso: **idea → prompt → resultado → ajuste.** Se queda lo que funciona y se cambia **una sola cosa** por vuelta.

---

## 1. Antes de empezar

**Entradas:** el objeto físico (o su foto), el público al que va el anuncio y una idea de look.

**Chat nuevo** para cada campaña, y todo en el mismo chat de principio a fin (mismo trabajo, mismo chat). Modelo de conversación en **Auto** (gratis) y **"Preguntar antes de generar"** activado.

**Reglas de la casa:** se pegan en el primer mensaje.
```
House rules for this chat:
- Always show me the plan, references, model, settings and cost before any generation. Never generate without my approval.
- Drafts first: videos at 480p, images at 1K unless I ask for more.
- No automatic extra passes: no storyboards, no cleanup passes, no refinement passes, no upscales unless I ask.
- One output per request unless I ask for variations.
- Pass references separately with their roles; never composite them.
- Change only what I name in a correction; keep everything else verbatim.
```

**Nunca pulsar "Permitir siempre"** en las tarjetas de aprobación.

---

## FASE A · Fijar los activos

### A1. Producto
1. **Foto:** objeto entero, luz de ventana de frente, fondo liso y claro, bordes y detalles visibles (bisagras, puente, logos). Móvil a la altura del objeto, sin gran angular.
2. **Limpieza:** recortar el fondo **sin redibujar**. Si ofrece varias opciones, elegir la de recorte, que no toca los píxeles del producto.
   ```
   The attached photo is our PRODUCT, [describe it]. Remove the background and put it on a plain light background. Keep it exactly as it is: same shape, colour and details. No redesign.
   ```
3. **Comprobar** con el original: contorno, color y detalles, y que no queden restos del fondo.
4. **Ficha de producto:** apuntar sus **comportamientos conocidos** (p. ej. "el cristal pasa de rojo a naranja con sol directo"). Una sola foto no lo cuenta todo, y el revisor no debe marcar como error lo que es una característica.
5. **Aviso:** las marcas registradas (logos) pueden activar el control de propiedad intelectual. Sirven para practicar; no se publican como anuncio de esa marca.

Coste de referencia: ~1 crédito.

### A2. Creador (opcional: solo si la idea necesita persona)
**Opción 1 · Casting nuevo:** skill **Character Sheet** (/character), con **3 variantes** para empezar.
```
Use Soul 2.0. Make 3 different [persona: edad, estilo, rasgos]. Outfit: [ropa de la campaña]. No eyewear/props, the product will be added later. Full body on the left, face on the right, 16:9.
```
- **Pedir el modelo por su nombre.** Sin indicarlo, la skill usó un modelo de 2,5 cr por hoja; con Soul 2.0, 0,125 cr.

**Opción 2 · Persona real (o personaje existente):** subir su foto u hoja y pedir **una** hoja en formato estándar con un modelo que conserve la identidad (Seedream 5.0 Pro o Nano Banana), a 2K, porque es la semilla.
```
Use the attached reference: this is [nombre], our CREATOR. Keep her/his exact face, skin, hair and build. Make ONE character sheet: full body on the left, face on the right, 16:9, plain light background. Outfit: [ropa de la campaña]. No eyewear, the product will be added later. Use the model that best preserves identity and show me the model and cost before generating.
```
- **Consentimiento:** si es una persona real, que esté de acuerdo.
- Marcas de agua o textos en la referencia: quitarlas antes con una edición local ("remove only… keep everything else identical") y comprobar que la cara no cambia.

**Criterios de una buena semilla:** cámara a la altura de los ojos, sin gran angular, **expresión neutra**, varias vistas (frente, tres cuartos, perfil, cuerpo entero), sin reflejos que tapen los ojos, cada vista en un archivo o en la hoja estándar, **sin collages con texto**.
**Vestuario:** se decide aquí y debe pegar con el producto. La ropa sobria deja que el producto sea la nota llamativa.

Costes de referencia: 3 caras en Soul 2.0 ≈ 0,4 cr · hoja de identidad en Seedream 2K = 2,5 cr.

### A3. Localización
Pedir **un lote** en 9:16 con un modelo barato (Soul 2.0 / Soul Cinema). Cada opción lleva su propio prompt para que haya variedad.
```
Use Soul 2.0. I need [5–10] Instagram/Pinterest locations in [ciudad / zona] that I can use for UGC content: [rasgos]. Golden hour, warm low sunlight with long shadows and rich, vivid colours. No people, no cars in the foreground, no readable text or logos. Vertical 9:16.
```
- **Pedir desde el principio la luz dorada y los colores vivos.** "Luz suave y natural" sale plana y sosa.
- **Revisar en grande**, no la miniatura, que recorta.
- Si nada convence: otra ronda con **un** cambio.

**Criterios para elegir:**
1. Encaja con el producto y con el público.
2. El producto contrasta con el fondo.
3. Hay espacio para la acción (el creador de pie, moviéndose, alguien grabando).
4. La luz cuadra con el resto de la campaña.
5. Está limpia: sin gente, textos, logos ni mobiliario que distraiga.
6. Hay varias opciones para comparar.

Costes de referencia: ~0,125 cr por imagen.

**Fin de la fase A:** tres activos descargados y revisados, con su papel claro.

---

## FASE B · Producir

### Cómo pasar los activos (en todos los pasos)
Adjuntar **en el mensaje, en este orden** y diciendo el papel de cada uno:
```
Use these three attached references: image 1 = PRODUCT ([descripción]), image 2 = CREATOR ([nombre / descripción]), image 3 = LOCATION ([descripción]).
```
- Una descripción del tipo "la de las pecas" no es una referencia; hay que adjuntar la imagen exacta.
- Comprobación final: en la tarjeta de aprobación tienen que aparecer **las miniaturas correctas**.

### B1. Fotos de campaña · skill Product Photographer (/product)
```
[Bloque de referencias]
Make a photoshoot for [producto] with [creador] in this location for [público], style: [look]. [Nº] vertical 9:16 photos: [N] with the creator using/wearing it and [N] of just the product. Keep the product exactly the same in every photo: [forma, color, detalles]. Same light direction across the whole set. Show me the shots and settings before generating.
```
- **Mínimo de la lección:** tres vistas útiles, que son primer plano, producto entero y producto en uso.
- **Revisar el plan antes de aprobar:** la mezcla de planos, las referencias de cada foto, **la misma dirección de luz en toda la serie** y que no haya "segundo pase" automático.
- **Comparar precios:** si 1K y 2K cuestan igual, generar a 2K.
- **Revisar la serie:** producto reconocible en todas, creador consistente, misma localización y luz.

Costes de referencia: ~2 cr por foto a 2K (Nano Banana 2.1).

### B2. Vídeo UGC · skill UGC (archivo .md adjunto)
1. Adjuntar el **.md de la skill UGC** + los tres activos por separado. **La localización es la imagen vacía**, no una foto de campaña.
2. Escribir la acción (una cosa sencilla con el producto: enseñarlo, probarlo, usarlo) y las frases exactas.
```
Use the attached UGC skill. [Bloque de referencias] Make a 15-second vertical 9:16 UGC video, 480p draft, one continuous handheld take. Her/his friend is filming with a phone. [Acción paso a paso, terminando en un momento claro]. Outfit: [si cambia respecto a la hoja]. She/he speaks [idioma y acento]. Have her/him say these exact lines, in order: "[…]" "[…]" "[…]". No storyboard, no extra passes. Show me the proposed action, the lines and the settings before generating.
```
**Frases:**
- 15 s dan para 4–6 frases cortas, con una palabra en MAYÚSCULAS por frase y cada frase pegada a una acción visible.
- **Sin inventar características** que no estén en la referencia del producto.
- La primera palabra es el gancho: nada de "vale" ni "hola".

**Acento:** describir **cómo suena** (p. ej. caraqueño: seseo, s final aspirada, ritmo caribeño, entonación de las preguntas) y listar los acentos que **no** se quieren. Nombrarlo solo no basta. Si el agente adapta el texto al acento, debe **avisar y pedir validación**.

**Revisar el plan antes de aprobar:**
- Sin storyboard.
- Tres referencias separadas.
- Una sola toma.
- Duración, formato y 480p.

**En la tarjeta:** las tres miniaturas y que el prompt empiece con "TECHNICAL AND WORLD RULES".

Costes de referencia: ~45 cr por 15 s a 480p (Seedance 2.5).

### B3. Anuncio de moda / cine · Cinema Studio
```
Generate a video in Cinema Studio using these images: [bloque de referencias]. Create a viral cinematic reels commercial for [producto]. [Vestuario si cambia]. [Duración] seconds, vertical 9:16, draft resolution. Keep the product identical to image 1 in every frame. No dialogue. Show me the settings and cost before generating.
```
- La petición corta de Adil **no fija la duración**; ponerla siempre.
- **Audio:** música de fondo más el ambiente si el vídeo es la pieza final; mudo si se va a montar después.
- **Cinema Studio es el estudio; el modelo puede ser Seedance 2.5 o Cinema Studio 4.0.** Mirar en la tarjeta cuál y cuánto cuesta.
- "Más dinámico" no garantiza mejorar: a Adil le deformó caras y le metió un segundo actor. Mejor una nota concreta.

Costes de referencia: 12 s a 480p con Seedance = 36 cr · Cinema Studio 4.0 a 720p = 98 cr (15 s, lección 1).

---

## FASE C · Revisar y entregar

### Checklist (PDF de la lección + experiencia)
- [ ] **Producto reconocible** en fotos y vídeos: forma, color y detalles. También cuando las manos lo tocan.
- [ ] **Las tres fotos** dan vistas útiles con un look coherente.
- [ ] **Creador y escenario consistentes** con la hoja y la localización.
- [ ] **Acción, cámara y final claros.** La última frase o acción termina antes del corte.
- [ ] **El sonido acompaña.** El habla es clara, en el idioma y acento pedidos, y encaja con lo que se ve.
- [ ] **No hay elementos de más:** ni segundo móvil, ni segundo actor, ni objetos inventados.
- [ ] **Lo que dice el agente coincide con los parámetros reales del trabajo** (formato, resolución, prompt enviado).
- [ ] La elección creativa encaja con el público y el producto sigue siendo el foco.

**Revisar siempre:** el vídeo entero y con sonido, y las imágenes en grande.
**Un borrador que funciona es suficiente.** Si algo distrae, se guarda esta versión y se elige **un** arreglo concreto.

### Entrega
Se guardan juntos en la carpeta de la campaña:
- la foto original del producto,
- los tres activos fijos (producto limpio, hoja del creador y localización),
- las fotos elegidas,
- los vídeos,
- los prompts exactos (campo Prompt de cada trabajo),
- dos frases: para quién es y por qué ese look y ese formato.

---

## Fallos conocidos y su prevención

| Fallo observado | Prevención |
|-----------------|------------|
| Generó sin pedir aprobación aunque el modo estaba activado | Reglas de la casa + revisar siempre la tarjeta; nunca "Permitir siempre" |
| Envió un prompt distinto del aprobado (callejón en vez de parking) | Leer el inicio del prompt en la tarjeta; si el chat da respuestas incoherentes, chat nuevo |
| Dijo un formato o resolución que no era el real | Fiarse de la tarjeta y de los parámetros del trabajo, no del texto del chat |
| Storyboard y "segundo pase" automáticos (más gasto) | Reglas de la casa; la skill UGC prohíbe el storyboard |
| La localización se quedaba fuera del vídeo | Pedir las tres referencias por separado y comprobarlo en el plan |
| Protagonista de espaldas todo el vídeo | Pedir explícitamente que se le vea la cara (ángulo y momento) |
| Elementos inventados (papel volando, cortinas) | Restricción "no other moving elements" y revisar el prompt antes de pagar |
| Luz de lado contrario entre fotos de la serie | Exigir la misma dirección de luz en toda la serie |
| Modelo caro por defecto en el casting | Pedir el modelo por su nombre |
| El archivo de skill adjuntado pero sin enviar | Comprobar que el .md sale en el mensaje enviado, no solo en la caja |

---

## Decisiones de modelo (referencia, 25-10-2026)

| Necesidad | Modelo usado | Por qué |
|-----------|--------------|---------|
| Explorar caras o localizaciones baratas | Soul 2.0 / Soul Cinema | ~0,125 cr por imagen |
| Conservar una cara real | Seedream 5.0 Pro | Elegido por el agente para identidad |
| Fotos de campaña con producto y persona | Nano Banana 2.1 | Admite varias referencias y respeta el producto |
| Vídeo UGC y anuncio | Seedance 2.5 | Referencias separadas, audio y voz en el idioma pedido |

Los precios y modelos cambian: se confirman siempre en la tarjeta. La comparación detallada de modelos de imagen va en la Lección 4.

| Necesidad | Herramienta | Por qué |
|---|---|---|
| Fotogramas clave con el mismo personaje en varios estilos | ChatGPT (un solo chat) | Guarda el contexto y da continuidad al personaje; luego se sube a Higgsfield |
