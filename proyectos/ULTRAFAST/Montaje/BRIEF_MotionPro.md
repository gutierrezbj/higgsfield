# BRIEF PARA MOTION PRO · Corto "ULTRAFAST" (~1:45) · JRGB

Objetivo: montaje final de un cortometraje 16:9 para la web jrgblanco.com. Juan, ingeniero de campo, tiene que llegar a las 19:00 a un CPD caído; pulsa ⚡ULTRAFAST en su reloj y salta por 7 mundos, cada uno con un estilo visual distinto, hasta llegar destrozado al CPD, donde está Adri. Nivel entregable de agencia, no un corte básico.

Carpeta base: ~/Library/CloudStorage/OneDrive-Personal/Formacion/Higgsfiled/Retos/Corto-ULTRAFAST/
Referencia de orden ya aprobada: Montaje/ULTRAFAST-borrador-v3.mp4 (1:44; estructura buena, falta acabado).
Guion: Docs/Guion-v1.md · Tracker: Docs/PLAN-y-tracker.md

## Salida
- 1920x1080 (16:9), 24 fps, H.264, AAC 48 kHz. Los clips de origen son 854x480: escalar con la mejor calidad posible (lanczos + nitidez suave), sin deformar.
- Archivo: Montaje/ULTRAFAST_Final_JRGB.mp4. Además, una versión ligera para la web (≤ 15 MB) y una versión muda en bucle de 10–15 s para la cabecera (sin texto).
- NO alterar caras, voces ni el reloj. El audio original de cada clip (voces y efectos) es el único audio. **Sin música** (decisión de JuanCho).

## Orden y cortes (tiempos en el clip de origen)
| # | Archivo | Entrada-Salida | Contenido |
|---|---|---|---|
| 0 | E0/E0-toma1.mp4 | 0,0-7,0 | Intro: del suelo al portátil "CPD CAÍDO · 19:00", Juan dormido con el perro y el gato |
| 1 | E1/E1-toma1.mp4 | 0,0-12,0 | Despierta, se viste, reloj ⚡ULTRAFAST, "¿Ultrafast?… Dale.", se deshace en papel (opcional: recortar 5,0-6,0, el plano de la sudadera "sin cabeza") |
| T | Transiciones/tunel-toma1.mp4 | 0,0-5,0 | Túnel cuántico, "¡Coñoooo!" (SOLO esta vez) |
| 2 | E2/E2-toma1.mp4 | 0,0-11,0 | Novela gráfica: dron fumigador, "Recalculando ruta…" |
| 3 | E3/E3-toma1.mp4 | 0,0-13,0 | Chibi low-poly: servidores y robots |
| 4 | E4/E4-toma1.mp4 | 0,0-11,0 | Plastilina en Riad: bala a cámara lenta |
| 5 | E5/E5-toma2.mp4 | 0,0-12,0 | Manga en Caracas: "¡Coño! ¿En Caracas? ¡No me jodas!" (la toma 2; NO la toma1 ni la vozreal) |
| 6 | E6/E6-toma2.mp4 | 0,0-11,0 | Impresionista en París: la pintura se corre (la toma 2) |
| 7 | E7/E7-toma1.mp4 | 0,0-11,0 | 2D en el consejo de administración |
| 8 | E8/E8-toma1.mp4 | 0,0-11,0 | CPD real: "¿Tú también?", risas, relojes en el rack a las 19:00 |

## Efectos obligatorios
1. TÍTULO "ULTRAFAST" en E1, cuando el botón se enciende en el reloj (~8-9 s de origen): letras blancas gruesas con brillo azul eléctrico, entrada con glitch corto, 1,5 s, sin tapar la cara.
2. RÓTULO DE HORA Y LUGAR al inicio de cada mundo, esquina inferior izquierda, 1,5 s, estilo pantalla de reloj (fuente monoespaciada blanca con borde azul): E2 "18:18 · Campo" · E3 "18:26 · CPD" · E4 "18:34 · Riad" · E5 "18:41 · Caracas" · E6 "18:49 · París" · E7 "18:56 · Madrid" · E8 "19:00". (Corrige que en algunos clips el reloj marque 18:10.)
3. SUBTÍTULOS solo de las frases habladas, centrados abajo, blancos con borde, fuera de las caras: "¿Ultrafast?… Dale." · "Recalculando ruta…" · "¡Coño! ¿En Caracas? ¡No me jodas!" · "¿Era el de sistemas?" · "¿Tú también?"
4. CARTA FINAL (3 s, después del E8): fondo negro, "ULTRAFAST" y debajo "JRGB · jrgblanco.com", con un tic de reloj y una vibración suave.

## Transiciones (lo que hay que mejorar: cortes secos entre mundos)
- Entre mundos (E2→E3 … E7→E8): cada clip termina en la desaparición y el siguiente empieza en un flash blanco. Añadir en el empalme un destello blanco de 4-6 fotogramas con un "zap" eléctrico y que el aterrizaje ("¡bum!") quede reforzado con un sonido de impacto grave. Nada de fundidos a negro ni disolvencias largas.
- E0→E1: corte limpio cuando suena la alarma.
- E1→Túnel y Túnel→E2: directos (ya enlazan con flash).

## Sonido
- Sin música. Normalizar el corto a -16 LUFS sin aplastar los efectos. Igualar los volúmenes entre mundos (algunos clips vienen más bajos).
- Sonidos de Motion Pro solo en los empalmes (zap, impacto) y en los rótulos (tic de reloj suave).

## Control final antes de entregar
- Duración final y lista de efectos y transiciones aplicados (enseñársela a JuanCho ANTES de exportar).
- Mismas caras y mismas voces en todo; nada tapa caras ni el reloj.
- Ningún texto se sale de la zona segura 16:9.
