# Lección 1 · Tu primer video

**Curso:** Creación con IA: primeros pasos (Higgsfield Academy)
**Fuente:** https://higgsfield.ai/es/academy/courses/ai-creation/your-first-video
**Materiales:** vídeo de 13:21 + guía visual en PDF (17 páginas, guardada en esta carpeta como `ai-creation__your-first-video__your-first-video.8965eff2.pdf`)
**Instructor:** Adil (creativo en Higgsfield, más de 500 vídeos; antes era camarero sin experiencia en contenido)

---

## 1. Qué vas a conseguir en esta lección

Hacer **tres vídeos** con la misma idea, con tres herramientas distintas, y entender por qué el resultado cambia tanto:

| # | Vídeo | Herramienta | Qué escribes |
|---|-------|-------------|--------------|
| 1 | "Prompt perezoso" | Seedance 2.5 en Cinema Studio | Una sola frase |
| 2 | La misma idea, desarrollada | SuperComputer | La misma frase, pero el agente la expande |
| 3 | Preset cinematográfico | Preset listo | Nada. Solo subes una foto tuya |

La regla del curso: **no veas la lección como una película.** El instructor hace algo, dice "pausa", tú abres la plataforma y lo repites. Tu resultado te enseña más que el suyo.

Dos miedos que el instructor despeja de entrada:

- **"Hay muchas palabras que no entiendo."** Cierto. Cada término se explica cuando aparece (ver glosario al final).
- **"Hay cien modelos, me voy a confundir."** Piensa en ellos como herramientas de un taller. Un martillo no compite con un destornillador. Cada vez que se usa uno, se dice cuál y por qué.

Aviso honesto: dos de los tres vídeos de hoy saldrán peor que el de la intro del curso. Es normal y es parte del plan. El tercero te lleva ahí.

---

## 2. Las tres herramientas

### Seedance 2.5
Modelo de vídeo. Genera metraje de los más realistas que existen, casi indistinguible de un rodaje real. Lo usan estudios grandes. Es el modelo con el que se hacen los vídeos 1 y 2.

### SuperComputer
El agente de IA de Higgsfield. No es un chatbot cualquiera: **conoce cómo funciona Seedance ahora mismo** y su trabajo es convertir la idea que tienes en la cabeza en un lenguaje que el modelo entienda. Combina criterio técnico con criterio creativo. Según el PDF, reúne modelos de lenguaje (GPT, Claude, Gemini) con las herramientas de generación de imagen y vídeo: los LLM conversan y planifican, las herramientas conectadas generan.

Imagínalo como alguien sentado a tu lado que ha hecho 10.000 vídeos y nunca se cansa.

### Preset
Una escena ya preparada por otra persona: cámara, luz, sonido, probado docenas de veces y empaquetado. Tú solo cambias una cosa: el protagonista, subiendo una imagen.

---

## 3. Vídeo 1 · El prompt perezoso (paso a paso)

**Objetivo:** ver qué hace el modelo solo, sin dirección, con una sola frase.

1. Entra en **Higgsfield.ai**. Al principio verás muchas pestañas; no te agobies.
2. Busca la pestaña **Cinema Studio**. Es el panel de control donde se generan imágenes y vídeos.
3. Cambia a la pestaña **Video**.
4. Selecciona el modelo **Seedance 2.5**.
5. Ajustes:

   | Ajuste | Valor | Por qué |
   |--------|-------|---------|
   | Aspect ratio | **21:9** | Se ve más cinematográfico |
   | Calidad | **720p** | Suficiente para probar. 1080p solo cuando confías en el prompt |
   | Duración | **15 s** | |
   | Nº de vídeos | **1** | No 4 a la vez |
   | Sonido | **Activado** | |

6. Escribe el prompt:

   ```
   Create a 15-second video of an epic sci-fi scene.
   ```

7. **Antes de pulsar Generate, comprueba el coste.** En la lección, un vídeo con esos ajustes costaba **98 créditos**. Es muy fácil marcar un ajuste equivocado y gastar más de la cuenta.
8. Pulsa **Generate**. Tarda entre **5 y 10 minutos**. El vídeo aparece en la misma pantalla.

> **Tu turno.** Pausa, repite los pasos con ese mismo prompt (o uno parecido igual de simple) y lanza la generación.

### Qué acabas de hacer
No has dicho nada del protagonista, del mundo, del lugar ni del movimiento de cámara. Solo un formato y un ambiente. Eso es un **prompt perezoso**: te pone en marcha sin obligarte a escribir el brief perfecto.

**La trampa:** todo lo que no especificas, lo decide el modelo. A veces te sorprende para bien; otras crea algo precioso que no tiene nada que ver con lo que imaginabas.

### Resultado del instructor
La explosión se veía bien y la nave pequeña pasando junto a la enorme daba sensación de escala. Pero el láser era confuso: en un plano parecía que atacaba la nave grande, en el siguiente no se sabía de dónde salía el rayo, y luego explotaba todo. Quería ver a una nave burlar a la otra y en cambio intentaba entender qué había pasado.

Para una frase escrita en segundos, no está mal. **Pero no es la escena que quería.** Esa sensación de "no, eso no es" se convierte en la herramienta más útil de la lección.

---

## 4. Mientras esperas: créditos y cómo no desperdiciarlos

- Antes de generar, siempre ves **cuánto va a costar**. Ahí mismo está tu saldo restante y la opción de comprar más. Todo en una pantalla, sin sorpresas.
- **Un intento malo también gasta créditos.** Pagas por la generación, no por si te gusta el resultado. Es como un rodaje real: una vez grabada la toma, el tiempo y los recursos están gastados aunque no llegue al montaje final.
- Si una generación aparece como **Failed** o **NSFW**, puede ser un fallo técnico, un filtro de seguridad o una **comprobación de propiedad intelectual** (busca personajes y franquicias protegidas). Tu prompt o el propio vídeo pueden disparar el bloqueo aunque nunca hayas pedido un personaje famoso. En esos casos **los créditos se devuelven automáticamente** (el PDF matiza: algunos modelos tienen excepciones; si falta un reembolso, contacta con soporte).
- **El mismo prompt puede dar un vídeo distinto.** No estás pidiendo una pizza, estás tirando un dado, pero tú diseñas las caras. Cuanto mejor el prompt, más caras te gustarán.

---

## 5. Vídeo 2 · La misma idea con SuperComputer

1. En Higgsfield, pulsa **SuperComputer** en el menú superior.
2. Escribe exactamente lo mismo que antes y envíalo:

   ```
   Create a 15-second video of an epic sci-fi scene
   ```

3. A veces SuperComputer te hace una o dos preguntas primero (¿qué tipo de batalla? ¿qué época? ¿qué tono?). **Responde en lenguaje normal.**
4. Espera la generación.

> **Tu turno.** Pausa y repite.

### Resultado del instructor
Se ve al piloto, la nave pequeña lanza un misil y se ve dónde impacta en la nave grande. Ya no son solo naves y explosiones: hay **progresión**. Amenaza, piloto, contraataque, recompensa. Pedí una batalla espacial épica y el agente resolvió cómo mostrarla.

### Comparativa (la lección entera en un fotograma)

| Izquierda: prompt de una línea | Derecha: misma idea vía SuperComputer |
|---|---|
| Cinematográfico, pero el láser confunde | Se ve al piloto, el lanzamiento, el impacto |
| La nave grande explota sin saber quién disparó | La acción se sigue sin esfuerzo |

**No es talento ni años de experiencia. Es un prompt más claro.**

### Qué hizo SuperComputer por detrás (del PDF)
La petición corta solo daba duración y género. El prompt expandido especificó dos naves, un piloto y la secuencia ataque, evasión y contraataque. Las claves del prompt que generó:

- **Roles distintos.** Una nave pequeña con forma de cuña (30 m, negra mate) y un leviatán de 4 km con forma de manta raya. La "trinchera" de armas del leviatán, que brilla naranja, es a la vez la fuente del peligro y el objetivo del contraataque. El piloto da foco humano.
- **Causa y consecuencia.** La grande dispara, la pequeña esquiva, el piloto lanza el misil, el misil impacta en la trinchera, la explosión sigue a un impacto identificable. Cada plano empuja hacia ese desenlace.
- **Continuidad visual y de cámara.** Dirección de pantalla (la cuña siempre vuela de izquierda a derecha, el leviatán ocupa la derecha profunda), posiciones, persecución del misil. Nubes pasando y cambio de tamaño de las naves dan pistas de velocidad y distancia. Paleta, luces y materiales compartidos unen los planos.
- **Restricciones concretas.** Exactamente dos naves, un piloto visible (solo en el plano 3), un misil, un disparo de rayo, cuatro cortes duros a 3.0 s, 5.5 s, 9.0 s y 11.0 s. Sonido solo diegético (motores, rayo, nubes, impactos, respiración del piloto en cabina). Sin música, sin subtítulos.
- **Planos con tiempos.** 5 planos: Ataque (0-3 s), Evasión (3-5.5 s), El piloto decide (5.5-9 s, interior de cabina cámara en mano), Lanzamiento (9-11 s), Impacto y recompensa (11-15 s).
- **Tratamiento de color.** Suavidad fílmica pictórica, bajo contraste en la neblina, sombras levantadas a ciruela, paleta rosa / ciruela / verde mar / coral / carbón. El rayo del arma es el único rojo saturado del encuadre.

El prompt completo ocupa las páginas 8 a 14 del PDF. Merece leerse una vez entero para ver hasta dónde llega el nivel de detalle que un modelo de vídeo puede aprovechar.

---

## 6. Truco para ahorrar créditos: Seedance 2.5 Draft

Cuando quieres clavar una escena concreta o probar una idea con varias versiones:

1. Selecciona el modelo **Seedance 2.5 Draft**.
2. Déjalo en **480p**.
3. Mismo prompt, pero genera **4 versiones en un lote**.
4. Compara y elige la que tenga la acción y el movimiento de cámara que te gustan. Si ninguna sirve, ajusta el prompt y lanza otro lote.
5. Con la toma elegida, pulsa **Generate en 1080p**: te da un resultado idéntico a mayor resolución.

Cuentas de la lección (créditos):

| Opción | Coste |
|--------|-------|
| 1 borrador de 15 s en 480p | 45 |
| 4 borradores | 180 |
| Subir el favorito a 1080p | 180 |
| **Total: 4 borradores + 1 final** | **360** |
| 4 vídeos directos en 1080p | 720 |

La mitad. **Prueba la idea primero. Gasta en calidad final solo cuando ya tienes el plano que quieres.**

---

## 7. Vídeo 3 · El preset con tu foto

Esta vez no escribes **ni una palabra**.

1. Abre el preset (el que muestra el instructor en la lección; en la página de la lección hay un enlace "Abre Supercomputer" bajo "Práctica opcional").
2. Sube una imagen tuya o de tu personaje.
3. Comprueba que **la cara se ve con claridad**.
4. Pulsa **Generate**.

> **Tu turno.** Pausa, elige cualquier imagen y usa el preset.

Hace diez minutos no sabías qué era un prompt. Ahora tienes un vídeo cinematográfico contigo de protagonista.

---

## 8. Tarea de la lección

Sube en la ventana de la lección **tres vídeos**:

1. Uno con un prompt simple.
2. Uno con SuperComputer, **con la misma idea** que el primero.
3. Uno usando un preset **con tu propia foto**.

Condiciones de la plataforma: deben ser generaciones tuyas de los **últimos 3 días** y cada generación solo se puede enviar una vez. Las lecciones 4 a 7 aparecen bloqueadas hasta avanzar.

---

## 9. Lo que añade el PDF: cómo estructurar un prompt tú mismo

Una petición corta deja muchas decisiones al modelo. Describe los detalles que te importan y agrúpalos en **cinco partes**:

| Parte | Qué incluir |
|-------|-------------|
| **1. Sujeto** | La persona u objeto principal y sus rasgos visuales importantes |
| **2. Lugar** | El sitio, el entorno y la hora del día |
| **3. Eventos** | Las acciones en orden, incluido cómo termina la escena |
| **4. Cámara** | Qué se mantiene en cuadro, el punto de vista y el movimiento |
| **5. Luz + sonido** | La fuente de luz, su dirección y los sonidos que quieres |

Ejemplo del PDF:

```
A cyclist in a yellow jacket rides along a quiet city street at sunrise. She slows down
and stops outside a cafe. Keep the bicycle and rider fully in frame as the camera
follows from the side. Use soft morning light and natural street sounds.
```

La chaqueta amarilla identifica al sujeto. "Frena y se detiene" ordena los eventos. "Sigue desde el lado" describe la cámara mientras ocurre la acción. Puedes cambiar el orden o dejar una decisión abierta cuando no te importa.

**Haz específica la decisión visual.** "Dramático" sugiere un ambiente; para describir una iluminación concreta, nombra fuente y dirección:

```
Light from a window on the left side of the face, with the other side in shadow.
```

### Desarrollar una escena con SuperComputer en varios mensajes

En vez de pedir el vídeo de golpe, trabaja en tres pasos:

1. **Pide una descripción o un borrador de prompt, sin generar todavía.**
   ```
   I want a video of a cyclist in a yellow jacket arriving at a cafe. Describe the scene
   in plain language first. Do not generate a video yet.
   ```
   Si ya tienes clara la escena: "Write the prompt first so I can review it before generation."

2. **Discute y refina.**
   ```
   Make the street quiet and set the scene at sunrise. Follow the cyclist from the side
   and end when she stops outside the cafe. Show me the revised prompt before generating.
   ```

3. **Aprueba y genera.** Revisa el prompt, los ajustes, el número de salidas y el coste.
   ```
   That is the scene I want. Use this approved prompt and the agreed settings to
   generate one video.
   ```

**Guarda el prompt aprobado junto al resultado.** El mismo prompt puede producir otro vídeo distinto más adelante.

### Checklist antes de pulsar Generate

- [ ] ¿La escena propuesta coincide con mi idea?
- [ ] Modelo, formato de cuadro, resolución, duración, sonido y nº de salidas correctos
- [ ] He leído el presupuesto en vivo (créditos) de esta generación
- [ ] Voy a guardar una copia del prompt con el vídeo final
- [ ] Para practicar, ¿he comparado el precio de 480p u otras resoluciones bajas?

---

## 10. Glosario (del PDF)

| Término | Significado |
|---------|-------------|
| **Modelo** | Sistema de IA entrenado para generar contenido a partir de tus entradas. De imagen: Nano Banana, Seedream, Soul Cinema. De vídeo: Kling, Seedance |
| **Prompt** | Tus instrucciones escritas. Un "prompt perezoso" es una petición breve que deja muchas decisiones al modelo |
| **SuperComputer** | Agente de IA de Higgsfield: LLM (GPT, Claude, Gemini) + herramientas de generación |
| **Preset** | Escena ya preparada: cámara, luz y sonido diseñados; tú aportas la imagen del protagonista |
| **Aspect ratio** | Forma del cuadro, ancho:alto. 21:9 es más ancho en proporción que 16:9 |
| **Resolución** | Dimensiones en píxeles. El aspect ratio da la forma; la resolución, cuántos píxeles la componen |
| **Créditos** | Unidad que se cobra por generación. Un resultado terminado gasta créditos aunque no te guste |
| **Failed / NSFW** | Failed: la generación no se completó. NSFW: marca de seguridad de contenido. Los fallos técnicos y los controles de PI también detienen generaciones. Suelen devolverse los créditos |

---

## 11. Ideas clave para llevarte a futuros proyectos

1. **Empieza perezoso, luego dirige.** Una frase para ver qué hace el modelo; después la misma idea con detalle.
2. **Lo que no dices, lo decide el modelo.** Si algo te importa, escríbelo.
3. **Estructura en cinco partes:** sujeto, lugar, eventos, cámara, luz + sonido.
4. **Causa y consecuencia.** Una escena se sigue cuando cada acción lleva a la siguiente y el final es identificable.
5. **Restricciones explícitas** (cuántas naves, cuántos cortes, qué sonido) reducen la aleatoriedad.
6. **Borradores en 480p, final en 1080p.** La mitad de créditos para el mismo resultado.
7. **Lee siempre el coste antes de generar.** Y guarda el prompt aprobado con el vídeo.
8. **SuperComputer en tres mensajes:** describe sin generar, refina, aprueba y genera.

---

## 12. Enlaces útiles de la lección

- Getting Started with Seedance (Higgsfield Help Center): cómo lanzar una generación, añadir referencias y elegir ajustes básicos.
- Higgsfield Plans & Credits (Pricing): planes, créditos incluidos y límites.
- Troubleshooting Failed Generations (Help Center): qué hacer cuando una generación se queda parada o falla, y dónde comprobar reembolsos.
- Model directory, Soul Cinema, About SuperComputer, NSFW, IP checks (referenciados en la página 16 del PDF).

**Siguiente lección:** Lección 2 · Segundo cerebro. "No es una metáfora: es una herramienta real que cambiará por completo cómo trabajas con la plataforma."
