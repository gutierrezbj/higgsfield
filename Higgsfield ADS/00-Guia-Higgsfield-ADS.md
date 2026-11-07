# Higgsfield ADS · Guía de producción

Método: "Animals" de Adil (falso documental: entrevista + su día), adaptado a anuncios para clientes.
Fuente leída entera el 7-11-2026: blog de Adil en Higgsfield "How To Save AI Credits With Higgsfield + Claude" (enlazado desde higgsfield.ai/s/animalsbreakdown-higgsfieldai-dzKYAp) + vídeo youtube.com/watch?v=sCukTWZEt7Q.
Archivos de esta carpeta:
- `00-Guia-Higgsfield-ADS.md` → esta guía (el paso a paso).
- `01-Plantillas-prompts.md` → los prompts base, listos para rellenar.
- `02-Ficha-cliente.md` → el brief que se rellena por cada anuncio ANTES de abrir Higgsfield.
- `skills/higgsfield-acting-skill/SKILL.md` → la skill de actuación original (Tigran/Adil), sin traducir.

Lo marcado **[adaptación JRGB]** no sale de la fuente: es cómo lo llevamos a anuncios. Lo demás es literal del método.

---

## 0. Qué es el formato y por qué sirve para ads

- **A-roll = entrevista.** El personaje sentado en una silla, en el centro, hablándole a un entrevistador que nunca se ve ni se oye (está justo a la derecha del objetivo).
- **B-roll = su día.** Escenas de lo que hace, que se intercalan con la entrevista en el montaje.
- **Siempre se hace primero el A-roll**: así se sabe exactamente dónde entra cada plano del B-roll.
- **[adaptación JRGB]** En un anuncio, la entrevista es el testimonio y el B-roll enseña el problema y el producto en uso. Lo que vende es la actuación (lo que el personaje quiere y le cuesta), no un spot plano.

Herramientas (las mismas de Adil):
| Qué | Modelo | Ajustes |
|---|---|---|
| Hojas de personaje, ropa, producto | Seedream 5.0 Pro | 16:9, 2K |
| Locaciones (sets) | Soul Cinema | 16:9, 1080p |
| Ediciones puntuales y recolor | Seedream 5.0 Pro (modo edición, imagen adjunta) | 16:9, 2K |
| Vídeo | Seedance 2.5 | Draft 480p para probar → 1080p la toma buena. Planos de 14 s |
| Prompts | Claude, con la acting skill activada | — |
| Voz | Voice Change de Seed Audio, al final | voces predeterminadas |

---

## 1. Preparación única (se hace una vez)

1. **Instalar la acting skill en Claude.** En claude.ai: Customize → Skills → **+** → subir `higgsfield-acting-skill.zip`. Después **abrir un chat nuevo** (la skill solo se activa en chats nuevos).
2. **Comprobar:** en el chat nuevo, escribir "¿tienes la higgsfield-acting-skill activa?". Debe responder que sí.
3. Esta carpeta `Higgsfield ADS` en el Project de Claude es la referencia. Cada cliente nuevo arranca rellenando `02-Ficha-cliente.md`.

---

## 2. Por cada cliente: ficha antes que nada

1. Copiar `02-Ficha-cliente.md`, guardarla como `clientes/<cliente>-<campaña>.md` en este Project y rellenarla entera.
2. Sin ficha completa no se genera nada. Los campos que más pesan:
   - **Dolor del cliente final** → será el OBSTACLE de la actuación.
   - **Colores de marca en HEX** → serán la palette card.
   - **Formato y plataforma** → decide la relación de aspecto de todo (ver paso 6).
   - **La frase del personaje** → corta. 14 s dan para unas 2–3 frases con pausas.

---

## 3. Proyecto en Higgsfield (Cinema Studio)

1. Entrar en Cinema Studio → **nuevo proyecto**. Nombre: `ADS · <Cliente> · <Campaña>`.
2. Crear **4 carpetas**: `CHAR` (personajes), `PROPS` (ropa y producto), `LOCATION` (sets), `SCENES` (vídeos).
3. **Regla de nombres:** cada recurso se guarda como Element con un nombre corto y **el mismo nombre en Claude y en Higgsfield**. Así los prompts que escribe Claude funcionan tal cual.
   - **[adaptación JRGB]** Con varios clientes, prefijo de cliente en todos: `@dd_maestro`, `@dd_showroom`, `@dd_uniforme`. Nunca dos clientes con el mismo nombre de Element.

---

## 4. Paso 1 · El personaje (CHAR)

**Qué se pide a Claude:** en palabras normales, qué personaje es y qué cara debe tener. Ejemplo literal de Adil: "Write me an image prompt. I need a brown bear for this film. Make him look like a bear from a movie…". Claude escribe el prompt largo.

**Qué tiene que llevar el prompt (lo comprueba uno antes de pegarlo):**
- Dos fotos lado a lado sobre **gris medio liso**: sin textura, sin ventanas, sin objetos.
- "El mismo individuo en las dos fotos": misma cara, mismos colores, misma complexión.
- **Izquierda:** retrato de cabeza y hombros, de frente, mirando a cámara.
- **Derecha:** cuerpo entero de frente **cortado justo bajo la barbilla, con la cabeza fuera de cuadro**. Brazos relajados a los lados, manos abiertas y vacías.
- Luz suave principal desde la izquierda, lado en sombra a la derecha, sin retoque.
- Negativos: no CGI, no render 3D, no plástico, no caricatura, no persona disfrazada. Sin texto ni logos.
- Color natural: sin etalonaje, sin tinte, sin dominante verde.

**Dónde:** Imagen → Seedream 5.0 Pro, 16:9, 2K → pegar el prompt → Generar.
**Revisar:** cara clara, cuerpo entero con manos y pies, fondo gris limpio. Si vale: guardar como Element en `CHAR` con su nombre (`@<cli>_<personaje>`).
**Si falla un detalle:** no se regenera, se edita (ver paso 7).

Plantilla: `01-Plantillas-prompts.md` → P1.

---

## 5. Paso 2 · Ropa y producto (PROPS)

Regla de Adil: **la ropa va aparte del personaje.** Así se cambia el vestuario sin rehacer el personaje (es uno de los tres ahorros).

1. Pedir a Claude la ropa en palabras sencillas ("haz un uniforme básico de camarero en blanco y rojo, que destaque").
2. El prompt debe pedir un **flat-lay cenital sobre gris medio liso**: sin persona, sin maniquí, prendas en orden de uso y bien separadas, con los colores en HEX, tela real con pliegues y algo de uso, sin texto ni logos.
3. **El conjunto tiene que salir entero.** Si sale cortado (en el ejemplo del ciervo el pantalón salía cortado), se corrige con una edición: "Show the whole pair of pants. Keep the clothes the same."
4. Si aparece algo que sobra (en el uniforme salió una bandeja con comida), también se edita: "Keep only the clothes. Remove the tray… No person, no text."
5. Guardar cada conjunto como Element en `PROPS`: `@<cli>_<personaje>_<uso>`.

**[adaptación JRGB] El producto del cliente va aquí, en su propia hoja**, con la misma lógica: fondo gris, producto entero, sin texto inventado. Si el producto lleva logo o etiqueta real, se usa la foto real del cliente como referencia; no se le pide al modelo que invente el logo.

Plantillas: P2 (ropa), P3 (producto).

---

## 6. Paso 3 · Locaciones (LOCATION)

### 6.1 Palette card (una por cliente)
- Adil usa una tarjeta con los HEX que comparten todas las locaciones, y la adjunta a Claude cada vez que pide una locación. Así los colores vuelven como HEX dentro del prompt.
- **[adaptación JRGB]** Construirla con los colores de marca de la ficha + neutros. Guardarla en `LOCATION` como `@<cli>_paleta`.

### 6.2 Set de entrevista (la regla fija)
Pedido a Claude, del estilo de: "Haz [lugar del cliente] para una entrevista. Una silla en el centro, cámara de frente."
El prompt tiene que llevar:
- **Encuadre perfectamente simétrico**, punto de fuga central, cámara a la altura de los ojos de alguien sentado.
- **Una silla vacía en el centro**, mirando a cámara, a unos pasos del fondo.
- **Luz principal suave desde fuera de cuadro a la izquierda, ~45° hacia la silla**: quien se siente es lo más iluminado del cuadro.
- **Fondo 1–2 pasos más oscuro**, con prácticos cálidos (lámparas ámbar) para separar al personaje del fondo.
- Primer término desenfocado y simétrico en las dos esquinas de abajo.
- Paleta en HEX, película 35 mm, grano fino, anamórfico sutil sin flares.
- Sin texto ni logos.
- **Alrededor de la silla, espacio limpio**: si hay trastos pegados al personaje, al moverse se funden.

**Dónde:** Imagen → Soul Cinema, 16:9, 1080p. Guardar como `@<cli>_set`.

### 6.3 Locaciones del B-roll
- Mismo sistema: Claude escribe el prompt y Soul Cinema lo genera.
- Pensar la acción: Adil puso el baño portátil mirando a cámara y con espacio delante "para verle intentar entrar".
- Un mismo sitio puede dar dos sets: la obra (`@site`) y la obra preparada como entrevista (`@site_interview`).
- Si una locación no existe como imagen, se puede describir solo con palabras en el prompt del vídeo.

### 6.4 Formato **[adaptación JRGB]**
- Adil trabaja en horizontal (sets a 16:9 con look 2.39:1 y vídeo 21:9).
- Para Reels/TikTok/Stories: **generar los sets ya en 9:16** y quitar "2.39:1" del prompt. El set simétrico con la silla en el centro funciona igual en vertical.
- Probar primero en Draft 480p (paso 8) antes de dar por bueno el formato.

---

## 7. Ediciones en vez de regenerar (ahorro)

- Se adjunta la imagen y se le dice a Seedream **qué cambia y qué se queda**. Ejemplos literales: "replace the monitors with modern ones"; "remove the text on the toilet, replace it with WC".
- **Recolor:** cuando el encuadre gusta pero el color no (la calle salía demasiado verde), Claude convierte los colores en HEX y Seedream cambia **solo el grade**: "Do not add, remove or move anything."
- Antes de cada intento, decidir qué se va a cambiar: cada generación extra cuesta créditos.

Plantillas: P5 (edición), P6 (recolor).

---

## 8. Paso 4 · Escenas (SCENES) con Seedance 2.5

### 8.1 Orden
1. **A-roll (entrevista) primero.**
2. Luego el B-roll, que se coloca donde la entrevista lo pide.

### 8.2 Cómo se le pide a Claude (dos mensajes, en un chat con la acting skill activa)
1. **Qué pasa**, con los Elements adjuntos: "Haz una entrevista corta con @X en @set. Lleva @ropa y se sienta en una silla demasiado pequeña. Dice: «…». Luego escucha la siguiente pregunta y pregunta: «…»."
2. **Qué está haciendo de verdad** (esto es lo que activa la actuación): "Intenta convencer al entrevistador de que le va bien, pero ni él se lo cree. Que se revuelva en la silla y mire la cara del entrevistador entre frase y frase. Antes de «…» mira abajo, pausa y vuelve a subir la mirada. Usa la acting skill para meterlo en el prompt."

### 8.3 Estructura del prompt que debe devolver Claude (revisar que esté todo)
1. **ELEMENTS:** cada imagen con **lo único que define**. Por ejemplo: "Bear: cara, pelo y complexión; el fondo, la maqueta y la pose de la hoja NO se heredan"; "Outfit: solo la ropa"; "Set: lugar, silla, luz y paleta".
2. **STYLE / LIGHTING / COLOR:** el color con los HEX del set.
3. **CAMERA:** duración y planos con cortes en segundos exactos. Ejemplo: "14 s, tres planos fijos frontales con cortes secos en 6 s y 10 s, cámara a la altura del sentado, sin movimiento".
4. **PHYSICS:** cómo pesa y se mueve el personaje de verdad (piel, pelo, respiración, la silla que cede, la ropa que tira).
5. **RULES numeradas:** los candados. No se levanta. Lleva la ropa en todos los planos. El entrevistador no se ve ni se oye. Sin lágrimas.
6. **CHARACTERS:** postura.
7. **ACTING TASK:** SCENE DIRECTION, MOTIVE, GOAL, OBSTACLE, TACTIC + **momento a momento con tiempos** + la línea de seguridad contra la mirada vidriosa.

Plantilla completa: P7.

### 8.4 Generar
1. Vídeo → Seedance 2.5 → adjuntar los Elements → pegar el prompt.
2. **Primero Draft a 480p.** Se revisan acción, ángulo y actuación.
3. Si falla: decir a Claude qué falla en concreto, corregir el prompt y repetir en 480p.
4. Solo cuando la actuación y el plano gustan → **la misma versión en 1080p**.
5. Guardar en `SCENES`.

### 8.5 Probar variantes baratas
- **Object Swap** (tip del vídeo): para probar otro personaje u otro producto, se cambia el objeto sobre una toma ya hecha antes de pagar una escena nueva.
- **[adaptación JRGB]** Útil para versiones del mismo anuncio por público o por producto.

---

## 9. Montaje y voz

- Se intercala A-roll y B-roll según lo que pide la entrevista.
- **La voz va al final:** primero se dirige la actuación y luego se elige la voz. Voice Change de Seed Audio con voces predeterminadas; es barato y se prueban varias para la misma línea.
- **[adaptación JRGB]** Rótulo final y CTA del cliente en el montaje, no dentro de la generación.

---

## 10. Los ahorros (resumen para tenerlo delante)

1. Todo en Draft 480p; a 1080p solo la toma que se queda.
2. Editar detalles en vez de regenerar la imagen entera.
3. Ropa (y producto) separados del personaje: cambiar de vestuario nunca obliga a un personaje nuevo.
4. La acting skill da una toma buena antes, con lo que se pagan menos reintentos.
5. Decidir qué se cambia antes de cada nuevo intento.

---

## 11. Cómo se adapta a clientes distintos **[adaptación JRGB]**

| Tipo de cliente | Personaje (CHAR) | Set entrevista | B-roll | OBSTACLE típico |
|---|---|---|---|---|
| Producto físico / tienda | cliente tipo o mascota de marca | su casa o la tienda | el problema sin producto → con producto | lo que le frustra sin el producto |
| Restaurante / comida | cocinero, camarero o cliente habitual | la cocina o el comedor vacío | servicio, plato saliendo | prisa, competencia, el plato que nadie conoce |
| Servicio técnico / B2B / industrial | técnico u operario | el taller, la obra, la nave | intervención en campo | la avería, el cliente esperando |
| Software / app | usuario (autónomo, gestor…) | su oficina o despacho | su día con el lío → con la app | papeleo, errores, falta de tiempo |
| Servicio local (reformas, etc.) | el maestro o el cliente que reformó | la obra a medias o el showroom | antes / durante / después | obra que se alarga, presupuesto que no cuadra |

Animal o persona: el método funciona igual. El animal llama más la atención; la persona da más credibilidad en B2B. Se decide en la ficha.

---

## 12. Checklist de entrega por anuncio

- [ ] Ficha de cliente rellena y guardada en `clientes/`.
- [ ] Proyecto Cinema Studio con las 4 carpetas y Elements con prefijo de cliente.
- [ ] Personaje: dos paneles, una sola cara, fondo gris.
- [ ] Ropa y producto en hojas aparte, completos en cuadro.
- [ ] Palette card de marca aplicada a todas las locaciones.
- [ ] Set de entrevista con la regla: simétrico, silla centrada, luz izquierda 45°, fondo más oscuro.
- [ ] A-roll aprobado en 480p → 1080p.
- [ ] B-roll aprobado en 480p → 1080p.
- [ ] Voz elegida al final.
- [ ] Montaje con CTA y rótulos del cliente.
- [ ] Créditos gastados anotados en la ficha (para presupuestar el siguiente).
