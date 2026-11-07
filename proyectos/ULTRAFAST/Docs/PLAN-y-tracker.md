# Corto "ULTRAFAST" — 8 mundos (método Adil, vídeo B) · destino: web jrgblanco.com
Fuente del método: ../Metodo-Adil-cortometrajes.md (parte B) + librería de prompts de las 8 escenas (Notion).

## Logline (borrador v0)
Juan, ingeniero de campo, tiene que estar a las 19:00 en un centro de datos caído. El reloj de su dron le ofrece una tercera ruta: ⚡ ULTRAFAST. La pulsa… y cada salto lo lanza a un mundo con un estilo visual distinto, cada uno peor que el anterior.

## Escenas (borrador v0, pendiente de que JuanCho lo valide)
| # | Mundo / estilo | Qué pasa | Sale con |
|---|---|---|---|
| 1 | Casa · papel recortado / anime | Alarma: "CPD caído, 19:00". Se viste a la carrera. El reloj ofrece Larga / Corta / ⚡ULTRAFAST | Pulsa → flash blanco |
| 2 | Campo agrícola · novela gráfica Moebius | Cae sobre un dron fumigador gigante en pleno vuelo | Pulsa |
| 3 | Sala de servidores · chibi low-poly | Sus manos son bloques y no atina con el reloj | Pulsa al cuarto intento |
| 4 | **Riad** · plastilina a cámara lenta | Azotea frente a las torres de Riad, tormenta de arena; un dron de seguridad le dispara a cámara lenta | Pulsa a 1 cm |
| 5 | Caracas · manga en blanco y negro | Lo persiguen motorizados por las escaleras de un barrio | Pulsa desde un poste |
| 6 | **París** · pintura impresionista (acuarela/óleo) | Cae dentro de un cuadro junto al Sena con la Torre Eiffel; un pintor lo pinta y la lluvia empieza a correr la pintura de su cuerpo | Pulsa mientras se destiñe |
| 7 | Reunión de directivos · dibujo 2D en imagen real | Cae en mitad de un consejo de administración | Saluda incómodo y pulsa |
| 8 | Centro de datos · imagen real | Llega destrozado a las 19:00 en punto. Adri ya está allí, igual de destrozada y con el mismo reloj. Se ríen y dejan los relojes en el rack | Fin |

## Cambios v1 (26-10)
- Añadidos París y Riad (JuanCho). Salen la azotea cyberpunk (→ Riad) y el infierno (→ París).

## Decisiones técnicas propuestas
- Formato 16:9 (pensado para la cabecera de la web; Adil usó 2.35:1).
- 8 escenas × 10–12 s = ~1:30 total.
- Seedance 2.5 a 480p para iterar; la final a 1080p.
- Encadenado: cada escena = fotograma clave del mundo + prompt anterior + "Extend @video1, continue from the white flash".
- Objeto conductor: el reloj del dron (hoja de atrezo con vistas ortográficas).

## Tracker
| # | Paso | Coste | Estado |
|---|---|---|---|
| 0 | Validar historia y mundos | 0 | ⬜ |
| 1 | Guion por entrevista (Claude) | 0 | ⬜ |
| 2 | Hoja de atrezo: reloj con el botón ULTRAFAST (Nano Banana Pro) | ~3 | ⬜ |
| 3 | Fotograma clave del mundo 1 (Soul Cinema + enhancer) | ~0,5–2 | ⬜ |
| 4 | Escena 1 (Seedance) | ~45/tanda | ⬜ |
| 5–11 | Mundos 2–8: fotograma clave + escena encadenada | ~50 c/u | ⬜ |
| 12 | Montaje + música (postproducción) | 0 | ⬜ |
| 13 | Versión final para la web | ? | ⬜ |

## Cerrado (26-10): 8 mundos v1 (con París y Riad, sin infierno).

## Herramientas por paso (lo que Adil no tenía cuando hizo este corto)
| Paso | Herramienta | Por qué |
|---|---|---|
| Guion por entrevista | Claude (aquí) | Método Adil: preguntas → guion, nunca "escríbeme un guion" |
| Juan en cada estilo | **Character Sheet** (skill preinstalada / AI Director) | Hoja con una sola cara por estilo, a partir de @juancho_V1.0 |
| Reloj ULTRAFAST | Claude → prompt de hoja de atrezo → Nano Banana Pro / GPT Image 2 | Vistas ortográficas para la consistencia |
| Fotograma clave por mundo | Soul Cinema + enhancer; Cineimage Soul si hace falta | Tandas baratas, variedad |
| Prompt de cada escena | **AI Director con Astra 6** (DE PAGO, ~1–8 cr por paso; usar solo si compensa) + Seedance Prompter / CINEDANCE | Encadenado: prompt anterior + vídeo anterior + fotograma clave |
| Revisión | Astra 6 compara prompt y resultado; checklist acción/continuidad/cámara/audio | Ciclo Describe → Generate → Review → Refine |
| Retoques locales | Seedance 2.5 Edit | Solo si compensa frente a una toma nueva |

## Ejecución según SOP-01 (decisión 26-10: "sticky to the plan")
**FASE A · Fijar los activos**
- A1 · Producto = **reloj de JuanCho**:
  - fotos (frente, laterales, 3/4, en la muñeca izquierda);
  - recorte de fondo sin redibujar (~1 cr);
  - ficha de comportamientos: la pantalla muestra la interfaz ULTRAFAST y la hora; al pulsar, flash blanco con fragmentos azul eléctrico;
  - de ahí sale la hoja del reloj con la pantalla ULTRAFAST.
- A2 · Creador = @juancho_V1.0 → versión de una sola cara con fondo gris (método Adil). @adri_Adri_V1.0 para la escena 8. Hojas por estilo con Character Sheet, cuando toque cada mundo.
- A3 · Localización = fotograma clave por mundo (Soul Cinema + enhancer), vacío o con la acción según el método B de Adil.
**FASE B · Producir** = escenas en Cinema Studio (Seedance), encadenadas con AI Director/Astra 6.
**FASE C · Revisar y entregar** = checklist del SOP + carpeta final con prompts y activos.

## Estado 26-10 (cierre)
- ✅ Proyecto ULTRAFAST con carpetas (00-Activos/Reloj, Juan, Adri; E1–E8).
- ✅ Reloj: recorte front_1K.png (SuperComputer) → pantalla ULTRAFAST con GPT Image 2.5 (AI Director, 2,75 cr). Elemento `reloj_ultrafast` (categoría Prop, v1), pendiente de confirmar que se creó.
- Lección aprendida: un paso = una pantalla, una foto, una frase (como las gafas de la L03). Chat siempre en Auto/Free; GPT 6 Astra cobra cada mensaje.
- Siguiente: hoja de Juan con una sola cara → fotograma clave del mundo 1.

## Estado 27-10
- ✅ Activos fijos en 00-Activos: `reloj_ultrafast` (Prop v1), `juancho_v2` (una cara, fondo gris), `adri_v2` (una cara, fondo gris).
- ✅ E1-Casa: fotograma clave `E1-keyframe.png` (papel recortado, con perro y gato) → subido a la carpeta E1-Casa.
- Receta que funcionó (E1, todo en ChatGPT):
  1. imagen de estilo;
  2. cambiar la cara por la de la hoja, poner el reloj y pasar a 16:9;
  3. redibujar la cara en el mismo estilo.
- Pendiente: fotogramas clave E2–E8.

- **Decisión 27-10 (JuanCho):** los fotogramas clave de los 8 mundos se hacen en **un mismo chat de ChatGPT**, que guarda el contexto (cara, reloj, mochila) y da continuidad entre mundos. Higgsfield queda para los elementos, el almacenamiento por carpetas y los vídeos (Seedance). Regla: un solo chat de ChatGPT para todo el corto; cada imagen buena se descarga y se sube a su carpeta E#.

## ✅ FASE A COMPLETA (27-10, 19:17)
Fotogramas clave aprobados, uno por mundo:
- E1 papel recortado, con perro y gato.
- E2 novela gráfica, dron fumigador en el viñedo.
- E3 chibi low-poly en el CPD con robots.
- E4 plastilina en Riad, con tormenta de arena y dron (pendiente opcional: pantalla del reloj encendida).
- E5 manga en Caracas, con el Ávila y los motorizados.
- E6 impresionista en París, con el pintor retratándolo.
- E7 2D sobre imagen real en el consejo (Cuatro Torres).
- E8 CPD real con Juan y Adri destrozados.
Herramientas: E1–E7 en ChatGPT (un solo chat); E8 en Higgsfield con Nano Banana y @juancho_v2 + @adri_v2 + @reloj_ultrafast.
Antes de la FASE B: grabar 3 frases con la voz de JuanCho, con la intención: E1 "¿Ultrafast?… Dale." · E5 "¡Coño! ¿En Caracas? ¡No me jodas!" · E8 "¿Tú también?".

## FASE B · vídeos (27-10)
- ✅ E1-toma1 (12 s, 36 cr): aprobada. Pendiente opcional: recortar el plano de la sudadera "sin cabeza" (5,0–6,0 s) en el montaje.
- ✅ E2-toma1 (11 s): aprobada, con el gag "Recalculando ruta…" funcionando.
- Herramientas del visor de Higgsfield: Recortar (para el montaje), Extender (encadenar), Editar (IA, 90 cr en 12 s: evitar).
- Transición: un clip de túnel cuántico reutilizable con la voz "¡Coñoooo!" (voz/tunel_cono.m4a) → carpeta Transiciones/.
- ✅ Transiciones/tunel-toma1 (5 s, ~15 cr): aprobado. Se reutiliza entre todas las escenas (versión normal y en espejo).
- E3-toma1: generado a 13 s (el prompt llega al 11 s): revisar los 2 s finales.
- E5-toma1 generado SIN audio de referencia: si la voz no vale → 1) cambio de voz de HF (mirar coste) · 2) superponer voz/E5_caracas.m4a en el montaje (gratis).
- ✅ E3-toma1 (13 s), E4-toma1 (11 s), E5-toma1 (11 s, sin referencia de audio: revisar la voz; si no vale → cambio de voz de Higgsfield o la grabación real en el montaje), E7-toma1 (11 s), E8-toma1 (11 s): aprobadas.
- E6: toma1 descartada (Juan sale fotográfico en un mundo pintado) → toma2 con el prompt reescrito y el estilo fijado (en el horno, 27-10 22:19).
- Pendiente: el reloj marca 18:10 en E3/E4 (en el montaje casi no se nota). Desde E5 la hora va en el prompt.
- Próxima sesión: revisar E6-toma2 → montaje (E1 → túnel → … → E8, recortar el plano de la sudadera del E1) → música → versión web.
- ✅ E6-toma2: aprobada (Juan pintado e integrado en el cuadro). La toma1 se queda como descarte.
- **Fase B completa:** E1–E8 + túnel. Siguiente: montaje.
- ✅ Montaje/ULTRAFAST-borrador-v1.mp4 (2:07, sin música): E1→túnel→E2→túnel espejo→E3→…→E8. El túnel completo (5 s) aparece 7 veces = 35 s.
- Próxima sesión: (1) acortar el túnel a ~2–3 s a partir de la segunda vez; (2) recortar la sudadera sin cabeza del E1; (3) decidir la voz del E5; (4) música; (5) versión final para la web (¿1080p?).
- 28-10: ✅ E0-toma1 (intro: del suelo al portátil "CPD CAÍDO · 19:00" y a Juan dormido) · ✅ E5-toma2 (con @Audio1, la voz real) · Montaje v3 = E0→E1→túnel (una sola vez)→E2…E8, 1:44, sin música.
- Siguiente: música con Higgsfield (Audio) → versión final para la web.
