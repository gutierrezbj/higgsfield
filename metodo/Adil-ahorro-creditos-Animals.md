# Adil · "Animals": cómo ahorrar créditos (3 tips)

Fuentes:
- Vídeo de Higgsfield AI, "You Will Stop Burning Your AI Credits After Watching This (3 Tips)": https://www.youtube.com/watch?v=sCukTWZEt7Q
- Blog con todos los prompts: https://higgsfield.ai/es/@adilinthewildtempo/blogs/how-to-save-ai-credits-with-higgsfield-claude
- Prompts y activos: https://higgsfield.ai/s/animalsbreakdown-higgsfieldai-dzKYAp

Resumido el 7-11-2026 para la serie VIAJEROS (nombre provisional anterior: HUELLAS).

## Flujo
1. **Proyecto en Cinema Studio** con 4 carpetas: CHAR (personajes), PROPS (outfits y objetos), LOCATION (sets) y SCENES (vídeos). Todo es Element con nombre (@bear), y se usan los mismos nombres en Claude y en Higgsfield para que los prompts de Claude funcionen tal cual.
2. **Ficha de personaje**: cara a la izquierda y cuerpo del cuello hacia abajo a la derecha, sobre gris liso, generada con **Seedream 5.0 Pro**, 4 versiones; se elige una. Claude escribe el prompt a partir de una descripción en palabras simples.
3. **Outfits separados del personaje**, en flat-lay sobre gris y completos en el cuadro, para que el modelo no invente.
4. **Locaciones** con Soul Cinema y arreglos con Seedream 5.0 Pro. Regla de entrevista: encuadre simétrico, silla en el centro, luz sobre ella y fondo un paso más oscuro. Espacio limpio alrededor del personaje, porque si hay mucho objeto, al moverse se funde.
5. **Tarjeta de paleta**: se adjunta a Claude en cada petición de locación, y los colores vuelven como códigos HEX dentro del prompt. Así todos los sets tienen el mismo look.
6. **Ediciones en vez de regenerar**: letrero ilegible, monitores viejos, copiar colores de otra imagen. Decir qué cambia y qué NO.
7. **Vídeo con Seedance 2.5**, usando el skill de actuación de Claude.
8. **Primero la entrevista (A-roll) y luego el día (B-roll)**, para saber dónde va cada cosa en el montaje.
9. **Voz al final** con Voice Change de Seed Audio: es barato y se prueban varias voces para la misma línea.
10. Una locación sin imagen se describe con palabras en el prompt del vídeo.

## Los 3 tips de ahorro
1. **Borrador a 480p primero** para acción y ángulo; solo la toma buena se termina a 1080p.
2. **Arreglar en vez de regenerar**, y decidir qué cambiar antes de cada intento.
3. **Probar personajes nuevos con un cambio de objeto** (Object Swap) sobre una toma existente, antes de pagar la escena completa.

Extra: el skill de actuación da una buena toma antes, con lo que se pagan menos reintentos. Primero la actuación, luego la voz.

## El skill de actuación (higgsfield-acting-skill.zip, en el blog)
Convierte una nota simple sobre el personaje en un bloque **ACTING TASK** dentro del prompt de vídeo:
- **SCENE DIRECTION**: lo que pide la escena, compartido y nunca dicho.
- **MOTIVE**: por qué lo quiere (su combustible).
- **GOAL**: qué quiere conseguir.
- **OBSTACLE**: qué se lo impide.
- **TACTIC**: cómo intenta conseguirlo. "El trabajo ocurre en los ojos".
- **Momento a momento**: cada línea o silencio con su intención (por ejemplo, "comprueba los ojos del entrevistador: ¿le cree?").
- **Safety**: la mirada siempre ocupada en la tarea, nunca fija ni vidriosa; parpadeo natural.

Instalación según Adil: en Claude, Customize → Skills → + → subir el zip, y abrir un chat nuevo.

## Estructura del prompt de vídeo de Adil (Seedance 2.5)
1. **ELEMENTS**: qué define cada referencia y qué NO hereda. Ejemplo: "@Bear = define cara, pelaje y complexión; el fondo, la maqueta y la pose de la ficha NO se heredan". Y de una locación: "NO es fotograma clave; el encuadre sale de este prompt".
2. **STYLE / LIGHTING / COLOR**, con HEX de la paleta.
3. **CAMERA**: duración, número de planos, cortes en segundos exactos, movimiento o cámara fija.
4. **PHYSICS**: cómo se mueve el cuerpo real (pelo, piel, peso, la silla que cede, la respiración). Ejemplo: "un oso real, no una persona disfrazada ni un CGI rígido; boca de oso, nunca boca humana".
5. **RULES**: numeradas, las cosas que no pueden pasar.
6. **CHARACTERS** y **ACTING TASK** (lo de arriba).
7. **ACTION TIMING**: plano por plano con tiempos y un **END STATE** al final de cada plano.
8. **AUDIO**: "solo sonido directo de producción", con tiempos exactos de diálogo y SFX. Sin música ni subtítulos.
9. **HOLD FOR THE FULL TIMELINE**: lo que debe mantenerse en todo el clip (identidad, vestuario, set).

## Aplicación a VIAJEROS
- Proyecto con carpetas CHAR / PROPS / LOCATION / SCENES; Elements con el mismo nombre en Claude y en Higgsfield (@lucas, @sofia, @aurora, @elias, @kai, @remi…; nombres definitivos pendientes al crear los Elements).
- Fichas de producción con Seedream 5.0 Pro (cara y cuerpo sobre gris, una sola cara), sacadas de las fichas de presentación ya hechas, en estilo B (3D cálido).
- Tarjeta de paleta única de la serie, adjunta a toda petición de locación.
- Si Kai y Remi no hablan (pendiente de decidir en la biblia v0.2): su ACTING TASK es puro ojos y cuerpo, y el bloque PHYSICS es clave (un perro y un gato reales).
- Todo en borrador de 480p hasta aprobar la actuación; el final, a 1080p.
