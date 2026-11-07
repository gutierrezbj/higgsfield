# Lección 6 · Dirige tu propia escena (Seedance 2.5, 2.ª parte)

Fuentes leídas enteras: subtítulos del vídeo (15 min), PDF "Dirige tu propia escena" (13 páginas), Seedance Prompter.md (skill cinedance-lite v3.0).

## Idea central
"Dejo de describir y empiezo a mostrar". Lo que cuesta poner en palabras se le enseña con una referencia:
| Lo difícil | Referencia | Qué se toma de ella | Qué define el prompt |
|---|---|---|---|
| Apariencia | Imagen (Elements) | Identidad, objeto, sitio, luz y color | Quién actúa y qué cambia |
| Movimiento | Vídeo del móvil | Recorrido de cámara, encuadre, velocidad, tiempos de la acción | Personajes, sitio, lo que cambia |
| Voz | Audio corto | Tono y acento | Quién habla y su diálogo (no tiene que repetir la grabación) |
No hace falta usar todos los tipos: solo los que resuelvan un problema de tu escena.

## 1. Referencia de vídeo ("doble candado": vídeo + prompt)
- Se graba con el móvil, sin perfección, con dobles (stand-ins): personas u objetos que representan a los personajes. El maletín de Adil era imaginario: lo mimaron y el maletín real lo pone la imagen.
- Del clip se toma la ruta de cámara, el encuadre, la velocidad y los tiempos de la acción. Las imágenes siguen mandando en personajes, atrezo y bar.
- Demo de Adil (3 tiempos): 1) cerca del que habla; 2) baja para enseñar la acción (abrir el maletín); 3) vuelve a los dos para la reacción.
- Línea de la referencia de vídeo: *"Use this video for the camera movement, framing, speed and action timing. The man on the left asking the question represents [friend]; the man on the right answering 'yeah' and miming the opening represents [biker]. Keep their positions and use the image references for the characters' appearance, the suitcase and the bar."*
- Se puede usar solo el arranque del clip (PDF p. 4): *"Use only 00:00-00:03 of @Video1 for the opening camera move and framing. After that, stop following its action and camera path. Continue with [new action and camera], ending on [final view]."*
- **Duración = la del clip del móvil.**

## 2. Referencia de voz
- Una grabación corta con tu voz (Adil: "Hey, I'm Adil, I'm 23 years old").
- Línea: *"This belongs to [personaje]. Use this audio as [personaje]'s voice reference. Match its vocal tone and accent. Apply it only to [personaje]."*
- El diálogo se escribe aparte en el prompt; no tiene que coincidir con lo grabado.
- Para nosotros: resuelve el acento caraqueño desde la raíz (ya no hay que describirlo).

## 3. AI Director con Astra 6 para escribir el prompt
- Cinema Studio → AI Director → modelo **Astra 6** ("el más potente; puede ver el vídeo") → **Apply Prompt Box** (trae el prompt y las referencias de la caja) → comprobar que están imágenes, clip y voz.
- Pedido de Adil: *"Help me write a Seedance 2.5 prompt using these references. Use the phone video for the camera movement, framing and timing. The man on the left becomes the friend… The audio is the friend's voice only. [Situación inicial]. [Diálogo]. [Acción]. [Cámara]. One continuous 15-second shot. Natural bar sounds, no music. Use this structure: Scene context, references, shot, audio. Keep the prompt clear and concise. Write the prompt only."*
- Corrigió la posición de cámara con un segundo mensaje y *"Keep everything else unchanged. Write the prompt only."*
- **Use** → manda el prompt al panel de vídeo. Comprobar que cada etiqueta apunta al elemento correcto y que el audio es solo del personaje que toca.
- Comparar el resultado con el clip: misma ruta y ritmo de cámara, mismo encuadre, cada persona en su sitio, voz parecida.
- ⚠️ Pendiente: ver cuánto cuesta Astra 6 antes de usarlo (en SuperComputer, los modelos que no son Auto pueden costar).

## 4. Seedance 2.5 Edit (cambiar un detalle sin regenerar)
- Panel de vídeo → Referencias → **Editar video** → el modelo pasa a Seedance 2.5 Edit → **Video to edit** → elegir la toma.
- Prompt: qué añadir o cambiar + dónde en el encuadre + cuándo empieza y termina + qué se mantiene. Ejemplo de Adil: *"When the camera returns to both men at the end, a man walks by behind them, giving them a strange look. Keep everything else unchanged, including the camera movement and audio."*
- Una edición, verla entera con sonido al lado de la original. Si cambia lo que no toca → nombrar el objeto con más claridad y su sitio, y repetir **desde la original**. Si rompe algo grande → quedarse con la original. **Nunca editar encima de una edición fallida.**
- Edit sirve para cambios locales. Si hace falta otra puesta en escena u otra secuencia de acciones → nueva toma.

## 5. Seedance Prompter skill (cinedance-lite v3.0)
- Se sube como en la L04 (ZIP → Save → elegirla en el chat).
- Modo A · Writer: con escena concreta (sitio, personaje, acción o duración). Estructura de 7 partes: SPINE, PLATE, CHARACTERS, SHOTS (con "Hard cut." entre planos), CAMERA LAW (óptica, movimiento, altura, motion blur, formato, un "anti-default"), GRADE AND AUDIO, CONSTRAINTS (contadores "Count of X: N" en vez de "No X").
- Modo B · Cinematic Random: solo un mood o género. Tira al azar formato, óptica, altura, movimiento, composición y número de planos. El contenido lo inventa el modelo.
- Encabezados que pide la lección (PDF p. 10): SCENE CONTEXT · REFERENCES · SHOTS · CAMERA LAW · GRADE AND AUDIO · CONSTRAINTS.
- Pedido recomendado (PDF p. 9): *"Use Seedance Prompter Skill to turn my brief into a clear video prompt. Preserve my scene, actions and camera choices. Use the actual attachment mentions. Do not add events or change the staging. If essential information is missing, ask me before writing the prompt."*
- Leer el prompt antes de generar: orden de la acción, cámara, menciones, cortes o diálogo de más. Ajustes = prompt.

## 6. Antes de escribir: intención (PDF p. 3)
- ¿Qué tiene que entender el espectador? ¿Qué tiene que pasar en pantalla? ¿Qué puede decidir el modelo?
- **Esencial** vs **abierto a interpretación** (gestos pequeños, fondo). Si no te importa un detalle, no lo describas: deja improvisar.
- AI Director para explorar (PDF p. 7): *"Review my scene idea and the attached assets. Identify missing information or conflicting instructions. Suggest two ways to stage the action and explain the trade-offs. Keep my essential requirements and flag any new creative choices you introduce. Wait for my choice before writing the final prompt."* · Con la guía de cámara de la L05: *"suggest three combinations of shot size, angle and movement…"*

## 7. Revisar (PDF p. 11)
1. Nombrar el error visible (qué, cuándo y qué querías). 2. Buscar la instrucción (contexto y planos; para apariencia o voz, también referencias y audio). 3. Comparar: si el texto pide lo que no quieres, lo deja abierto o se contradice → corregir; si la instrucción ya era clara, puede ser fallo de la toma, no del prompt. 4. Corregir a mano o con un LLM:
*"Compare this tested prompt with the attached result or my error description. Find wording that could explain the mismatch. If the instruction is already clear, say so. Revise only what needs changing, preserve the rest of my scene, and explain exactly what you changed and why."*

## Regla de Adil
"Cada línea extra tiene que ser algo que de verdad quiero ver u oír." · "Tu primera historia no tiene que ser perfecta; tiene que estar terminada."

## TAREA
Un vídeo corto que cuente una historia propia: **inicio, cambio y final**. Calidad borrador vale. Generaciones de los **últimos 3 días**; cada una solo se puede enviar una vez. Envío → desbloquea la lección 7 (cierre del curso).
Tras verlo: ¿se entiende sin explicarlo? ¿El final cierra la idea? Guardar la toma elegida con su prompt y sus referencias.

## Diario de la práctica (26-10)
- Clip 1 vertical → repetido en horizontal (16:9). Dobles: cojín = Juan, maleta con chaqueta naranja = Adri, maleta rígida = bolsa.
- Generación 1 (Video1.mp4, 51 cr): la cámara copia el recorrido del clip; inicio, cambio y final se entienden. Fallos: dos manos abren la bolsa desde el lado de la cámara (el clip lo enseñaba así: **el vídeo manda sobre el prompt**), "paña" en vez de "pana", entonación plana.
- Edit evaluado: 60 cr frente a 51 de una toma nueva; descartado porque las manos son un problema de puesta en escena.
- Clip 2: mano desde el lado de Juan; 4 s muertos recortados → Toma2_recortada.mp4 (14,8 s). Se sigue el clip hasta 00:13 y después dirige el prompt.
- Astra 6 (DE PAGO: ~1–8 cr por paso) revisó el prompt viendo el clip. Primero analizó el clip equivocado → chat nuevo + caja limpia.
- Diálogo con intención (tono, susurro, pausa) + notas de jerga en cada frase.
