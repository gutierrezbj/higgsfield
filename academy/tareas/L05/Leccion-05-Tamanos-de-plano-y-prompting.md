# Lección 5 · Tamaños de plano y prompting

**Curso:** Creación con IA: primeros pasos (Higgsfield Academy)
**Fuente:** https://higgsfield.ai/es/academy/courses/ai-creation/shot-sizes-and-prompting
**Materiales (leídos enteros):** vídeo de 15:45 (por subtítulos) · guía "Tamaños de plano y prompting" (9 p.) · guía "Cámara: tamaños de plano, ángulos y movimiento" (20 p.)
**Instructor:** Adil

---

## 1. Qué vas a conseguir

Juntar los recursos de la lección 4 (personajes, localización, atrezo) en **una escena de vídeo con Seedance 2.5**, dirigiendo acción, cámara y actuación. Flujo: **describir → generar → revisar → corregir.**

Escena del demo: el motero entra en el bar con el maletín naranja, ve a su amigo, se sienta a su lado y le dice "What's up?". 4 planos, 16 s.

---

## 2. Preparar el espacio
1. Cinema Studio → el proyecto de la lección 4 → nueva carpeta **Generations**.
2. Pestaña **Video** → modelo **Seedance 2.5**.
3. **Elements** (guardar recursos con nombre para no adjuntarlos cada vez):
   - en la imagen, **tres puntos → Create Element → Image Element**;
   - **categoría** (Character, Location, Prop…), que añade el prefijo al ID automáticamente;
   - **nombre** sencillo (Biker).
   - En el prompt se llaman con **@** (@Biker).
   - *Un @ escrito a mano no adjunta nada*: hay que seleccionar el Element.
4. Ejercicio: preparar 4–5 Elements con nombres claros y distintos.

---

## 3. Seedance 2.5 (lo que dice la lección)
- **Multimodal**: texto, imagen, vídeo y audio juntos.
- Genera de **4 a 30 s con sonido**, en **una toma continua** o en **varios planos con cortes** (multi-shot). Seedance decide la estructura según el prompt:
  - para una toma continua, describe una sola toma;
  - para multi-shot, describe cada plano y dónde van los cortes.
- Hasta **30 imágenes, 10 vídeos y 10 audios** (50 referencias). **En su experiencia, hasta 12 imágenes es lo que mejor funciona.** El demo usa 5: dos personajes, un atrezo y dos vistas de la localización.
- **Ajustes:**
  - formato (21:9 para cine);
  - resolución;
  - duración: **igual al último código de tiempo del prompt**;
  - **audio activado**;
  - **1 generación**.
- **Modo borrador (Draft)**: vista previa a **480p** para probar con menos créditos; luego se convierte la toma elegida a **1080p**. Útil en escenas complejas que requieren varios intentos.

---

## 4. El prompt en 3 partes (+ detalles y sonido)

### 4.1 Contexto de la escena
La acción principal visible de todo el clip en 1–2 frases.
> *Biker enters a bar with a suitcase looking for his friend. They notice each other, and the biker walks over and sits next to him.*

### 4.2 Referencias: un trabajo para cada una
- *The biker, 100% as shown in the reference image.*
- *His friend, 100% as shown in the reference image. He is seated on a stool on the side of the bar counter, directly in front of the beer mug shown in location reference.*
- *The suitcase, 100% as shown in the reference image. It belongs to the biker, he carries it in his left hand.*
- *The bar interior, 100% as shown in the reference image. Use it for the light, color, location, and background people. The beer mug on the counter marks his friend's seat. Keep the mug in its reference position.*
- *The bar entrance, entrance of the same bar. Use it for the color and location, not for composition or framing.*

Regla: **la imagen da la apariencia; el prompt da propiedad, posición y acción.** Si solo quieres la cara de alguien, dilo. Se nombra a la persona antes de cada acción y se dice quién lleva o maneja el atrezo.

### 4.3 Planos (cada corte = nuevo número de plano con su tramo de tiempo)
- **Plano 1 (0–5 s):** plano medio corto, contrapicado, **jib shot** (la cámara sube para revelar su cara). Alguien cruza delante de cámara, el motero entra con el maletín en la mano izquierda y la cámara sube mientras busca a su amigo.
- **Plano 2 (5–8 s):** cámara quieta a la altura de los ojos; el amigo de cintura para arriba, de espaldas y un poco de lado, sentado ante la jarra. Al ver al motero se gira a medias y levanta la mano.
- **Plano 3 (8–11 s):** primer plano a la altura de los ojos, tres cuartos de frente; gente pasando delante de cámara; la cámara aguanta mientras lo reconoce y sonríe; sale de derecha a izquierda.
- **Plano 4 (11–16 s):** desde detrás de la barra, de frente, distancia media. El motero entra por la derecha, se sienta junto al amigo, deja el maletín en la barra con la mano izquierda diciendo **"What's up?"**, suelta el asa y se acomoda. **Un segundo de silencio.**

### 4.4 Detalles y sonido (para todo el clip)
- El amigo sigue sentado en el lado de los clientes, con la jarra delante y siempre en el mismo sitio.
- **Profundidad en cada plano**: algo cerca, algo en medio, algo al fondo.
- **Regla de los tercios.**
- El bar animado, como en la referencia.
- Sonido: *Natural bar ambience, footsteps, and clothing movement. No music.*
- Antes de generar, **leerlo entero**: si puedes imaginar la escena y sabes quién hace qué y quién lleva el maletín, está listo.

---

## 5. Revisar y corregir
Tres preguntas tras cada toma (PDF p. 8):
- **Acción**: ¿hizo la persona nombrada lo que tocaba?
- **Continuidad**: ¿se reconocen las personas, el atrezo y el sitio?
- **Cámara**: ¿el encuadre deja ver la acción importante?

Detecta dónde está el fallo y **corrige solo eso**. En el demo, la toma 1 dejó el maletín de pie y Adil lo quería tumbado. Cambios para la toma 2 (dos a la vez, aunque él aconseja uno cuando empiezas):
- en el contexto de la escena: *"lays the case flat as he sits down"*;
- plano 3: **un leve gesto con la cabeza** en vez de la sonrisa;
- plano 4: *"He lays the closed suitcase flat on the counter in front of him with his left hand, lid up, handle toward him, saying 'What's up?'"*.

Reglas de corrección:
- Acciones **en orden**: qué pasa primero y qué después.
- Movimiento de cámara: **dónde empieza y qué sigue**.
- Si un personaje, el atrezo o el sitio sale mal → revisa **su referencia y lo que pediste tomar de ella**. Si el detalle no deseado está en la imagen → **arregla el recurso antes de reutilizarlo**.
- **Si el que hace la acción es el que no toca, casi siempre es la redacción**: si en la frase no se sabe quién es, Seedance tampoco lo sabe.
- Atrezo: dónde lo pone el prompt, quién lo lleva y que se mantenga igual en toda la escena.
- Una toma nueva se mira **entera** otra vez: el cambio pedido y todo lo que ya gustaba.

**¿Qué arreglar? (PDF p. 8)**
- ¿El mismo error vuelve en varias tomas? → revisa el **prompt y los recursos**.
- El detalle está en la imagen → **arregla el recurso**.
- Actúa quien no toca, el atrezo está mal colocado o la cámara se contradice → **arregla el prompt**.
- Entradas claras y un fallo aislado → **otra toma**, guardando la original.

**Petición de reparación a un LLM (PDF p. 6):**
```
Revise the tested prompt below. What went wrong: [describe the errors]. What I want instead: [describe the intended result]. Keep the parts that already work. Update every affected line so the instructions agree. Return the full revised prompt, then list exactly what you changed or added and why.
Tested prompt: [paste the original prompt].
```

---

## 6. Plantilla de escena (PDF p. 7)
```
SCENE CONTEXT
@character_1 and @character_2 are in @location_1. Starting state: [positions and situation]. Action and ending: [what changes, in order, and the visible outcome].

REFERENCES
@character_1 and @character_2: identity and clothing. @prop_1: object appearance; carried by @character_1. @location_1: space, light and colour.

SHOTS
Shot 1, [start-end time]: [shot size and angle]. Camera: [static, or movement with a destination]. @character_1 [visible action].
Shot 2, [start-end time]: [next view and camera behaviour]. @character_2 [action or reaction]. @character_2 says: "[dialogue]".

CONTINUITY & SOUND
@prop_1: [position and orientation, if needed]. [Other details that must stay consistent]. [Ambience, action sounds and music instruction]. [Final hold, if needed].
```
Un plano por cada corte; un solo bloque si es una toma continua. Quitar referencias y secciones que no se usen. Que el contexto y los planos cuenten la misma secuencia. Antes de generar: **duración = último código de tiempo**, recursos adjuntos, encuadre, audio y coste.

---

## 7. Cámara: guía rápida (PDF de 20 p.)

**Tamaños de plano**

| Plano | Qué muestra | Cláusula |
|-------|-------------|----------|
| Gran plano general (EWS) | El sitio manda, la persona muy pequeña | *Extreme wide shot; keep the subject small within the surrounding environment.* |
| Plano general (WS/LS) | Persona entera con mucho espacio | *Wide shot; full figure with open space around them.* |
| Plano entero (FS) | De la cabeza a los pies | *Full-body shot; keep the head and feet inside the frame.* |
| Plano americano largo (MLS) | Hasta las rodillas | *Medium long shot; frame the person from head to knees.* |
| Cowboy | Hasta medio muslo, con las manos | *Cowboy shot; head to mid-thigh, hands visible.* |
| Plano medio (MS) | De cintura para arriba | *Medium shot; waist-up, camera at eye level.* |
| Plano medio corto (MCU) | Cabeza, hombros y pecho | *Medium close-up; head and shoulders, chest at the lower edge.* |
| Primer plano (CU) | La cara | *Close-up of the face; blurred background.* |
| Plano detalle (ECU) | Un detalle | *Extreme close-up of the key detail; exclude the surrounding context.* |

El tamaño de plano **no es la lente**: "primer plano" describe el encuadre; la focal y la distancia son decisiones aparte.

**Ángulos:**
- a la altura de los ojos: *lens at the subject's eye height*;
- picado: *camera above the subject, looking down*;
- contrapicado: *low camera position, looking upward*;
- cenital: *directly overhead*;
- holandés: *a clearly diagonal horizon*.

**Movimientos:**
- **Pan**: gira en el sitio (*Pan right at an even pace from a fixed position; keep the horizon level and settle on the new view*).
- **Tilt**: mira arriba o abajo sin subir.
- **Pedestal o grúa**: la cámara sube o baja.
- **Dolly in/out**: se acerca o se aleja (*Dolly slowly forward to a closer view; keep focal length and camera height fixed*).
- **Truck**: se mueve en lateral, con paralaje.
- **Tracking**: viaja con el sujeto (*Track parallel to the moving subject at a matching pace*).
- **Arco**: rodea al sujeto.
- **Zoom**: cambia el campo de visión sin moverse.
- **Dolly zoom**: retrocede mientras hace zoom.
- **Estática**: *Locked-off camera*.
- **Cámara en mano**: *Restrained handheld drift*.
- **Roll** y **whip pan**.

Para describir un movimiento en vídeo: **recorrido, ritmo, qué se mantiene fijo y composición final**. En la primera prueba, **cambia una sola decisión de cámara**.

Ejercicio de tres planos: **general** (sitio) → **medio** (gesto) → **primer plano** (reacción).

**Truco: Soul Directory**, en `soul-directory.higgsfield.app`:
- 33 estilos, 46 movimientos de cámara y 24 esquemas de luz, cada uno con su prompt copiable;
- **Shot Builder**;
- simulador de luz en 3D.

---

## 8. Tarea de la lección
En la plataforma: **"Crea una escena, cambia una cosa en el prompt y genérala de nuevo. Añade ambos videos: antes y después del cambio."** → **0/2 vídeos**. Desbloquea la lección 6.
- Toma 1 y su prompt → lista de fallos → corregir las instrucciones → toma 2 → comparar las dos con sonido.
- Subir las **dos tomas con sus prompts**.

**Siguiente lección (6):** usar un vídeo del móvil para el movimiento de cámara y la voz propia para un personaje.

---

## 9. Ideas clave
1. **Elements** con nombres claros = referencias reutilizables con @.
2. **Cada referencia tiene un trabajo**; la imagen da la apariencia y el prompt la acción, la propiedad y la posición.
3. **Contexto → referencias → planos con tiempos → detalles y sonido.**
4. **Nombrar a quién actúa en cada frase**; si no se entiende quién, Seedance tampoco.
5. **Duración = último código de tiempo.** Dejar un segundo de silencio al final.
6. **Profundidad y regla de los tercios** en cada plano.
7. **Borrador a 480p** para probar; 1080p solo para la toma buena.
8. **Revisar acción, continuidad y cámara**; corregir lo que falla y mirar la toma nueva entera.
9. Error repetido → recurso o prompt; error aislado → otra toma.
