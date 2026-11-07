# Qué podemos generar desde aquí (curso Academy + este Project)

Comprobado el 7-11-2026. Cuenta Higgsfield conectada a Claude: plan **Plus**, **1.004 créditos** en ese momento (el saldo cambia; se consulta antes de cada encargo).

## Dos formas de producir
1. **En la web de Higgsfield** (como en el curso): Cinema Studio (proyectos, carpetas, Elements con @, AI Director, Seedance 2.5 Draft y "Generate in 1080p", Seedance 2.5 Edit) y Supercomputer (skills integradas /character sheet y /product, subir skills .md al chat).
2. **Desde un chat de este Project**, con el conector de Higgsfield: Claude escribe el prompt con las skills de `academy/skills/` y lanza la generación directamente (imagen, vídeo, audio, ediciones), guarda en proyectos y carpetas de Higgsfield y crea elementos de referencia. Cada generación pide aprobación y enseña el coste antes.
   - Seedance 2.5 está disponible por conector con resolución 480p / 720p / 1080p, 4–30 s, modos texto→vídeo, referencias (imagen, vídeo, audio), edición de vídeo y extensión de vídeo. El botón "Seedance 2.5 Draft" + "Generate in 1080p" del curso es de la web; por conector el borrador es pedir 480p (el precio exacto se ve en la aprobación).
   - Soul 2.0, Soul Cinema (incluye 21:9), Seedream 5.0 Pro (con modo edición), GPT Image 2/2.5/2.6, Nano Banana Pro también están en el conector.

## Catálogo de entregables
Cada fila: qué es, con qué se hace y qué lección/skill lo respalda.

| # | Entregable | Cómo | Modelo | Skill / fuente | Coste orientativo (curso) |
|---|---|---|---|---|---|
| 1 | **Clip rápido de idea** (15 s) | Prompt perezoso → mismo idea con entrevista previa | Seedance 2.5 | L1, L2 | 98 cr a 720p/15 s; 45 cr draft 480p |
| 2 | **Vídeo con preset** con la cara de alguien | Foto + preset | Presets de Higgsfield | L1 | según preset |
| 3 | **Foto de producto limpia** | Foto real → quitar fondo / fondo liso conservando el objeto | Edición (Seedream 5.0 Pro / GPT Image) o quitar fondo | L3 | bajo |
| 4 | **Casting de personajes** (muchas caras) | Descripción simple, lotes de 10–20 | Soul 2.0 | L3, L4 | 1,25 cr por 10 |
| 5 | **Hoja de personaje** (frente, espalda, retrato) + versión sin la cara pequeña | Casting elegido → hoja → edición puntual | Soul 2.0 + Seedream 5.0 Pro | L4 (/character sheet) + `metodo/` de Adil | bajo |
| 6 | **Personaje con cara real** (tuya o de un cliente) | Foto de cara + foto de vestuario | Seedream 5.0 Pro | L4 | bajo |
| 7 | **Localización cinematográfica** | Prompt con mapa izquierda→centro→derecha, sin gente | Soul Cinema | `cineimage-soul` (L4) | 0,125 cr/imagen |
| 8 | **Localización editada** (gente, ancla espacial, contraplano) | Imagen base + cambio + lo que se queda | Seedream 5.0 Pro | L4, `cineimage-soul` modo Edit | bajo |
| 9 | **Hoja de atrezo / producto** | Vista 3/4 sobre fondo neutro; varias vistas si es complejo | Soul / Seedream / GPT Image | L4 + `Higgsfield ADS/01` P3 | bajo |
| 10 | **Sesión de fotos de campaña** (con modelo y solo producto, 9:16) | Personaje + 3 localizaciones + producto | Imagen (Supercomputer /product) | L3 | bajo |
| 11 | **Vídeo UGC** (creador hablando del producto, vertical) | Referencias separadas: personaje, producto, localización | Seedance 2.5 | `ugc-video-creator` (L3) | según duración |
| 12 | **Anuncio cinematográfico de producto** | Assets generados + Cinema Studio | Cinema Studio / Seedance 2.5 | L3 | según duración |
| 13 | **Escena multiplano con diálogo** (2 personajes, atrezo, localización) | Elements @ + prompt Scene context / References / Shots | Seedance 2.5 | L5 + `cinedance-lite` modo A | 4–30 s |
| 14 | **Escena guiada por vídeo del móvil** (doble candado) | Clip de móvil para cámara y tiempos + imágenes | Seedance 2.5 referencias | L6 | duración del clip |
| 15 | **Voz de un personaje** a partir de una grabación | Audio de referencia asignado a un solo personaje | Seedance 2.5 / Voice Change | L6, `metodo/` Animals | — |
| 16 | **Arreglo de una toma ya buena** (añadir o cambiar un detalle) | Edición de vídeo sobre el clip original | Seedance 2.5 Edit | L6 | según duración del clip |
| 17 | **Corto con historia** (inicio, cambio, final) | Estructura de historia → assets → escenas | Todo lo anterior | L6, L7 + `metodo/Metodo-Adil-cortometrajes.md` | según escenas |
| 18 | **Exploración visual aleatoria** de un estilo ("lowkey neo noir") | Frase de ambiente; 3 tiradas baratas, se elige una | Seedance 2.5 | `cinedance-lite` modo B | 3 × 480p + 1 final |
| 19 | **Anuncio falso documental** (entrevista + su día) | Método Animals | Seedream 5.0 Pro, Soul Cinema, Seedance 2.5 | `Higgsfield ADS/` + `higgsfield-acting-skill` | ver guía ADS |

## Reglas que se aplican a todo (del curso)
- **Bucle:** idea → prompt → resultado → un ajuste. Un cambio por iteración cuando se está aprendiendo.
- **Borrador antes que final:** todo vídeo se prueba a 480p; solo la toma buena va a 1080p.
- **Assets primero:** si el material se ve mal en la imagen, se arregla la imagen, no el prompt de vídeo.
- **Una referencia, un trabajo:** cara, atrezo, sitio, cámara (vídeo), voz (audio). Hasta 12 imágenes es lo que mejor funciona.
- **Una sola cara por personaje** en la referencia del vídeo.
- **Anclas espaciales** (un objeto concreto en el set) para colocar la acción con una frase.
- **Duración = donde acaba el último plano.**
- **Dos chats:** uno para imágenes, otro para prompts de vídeo; un asset o una escena cada vez.
- **Un trabajo, un chat**; la entrevista antes del prompt.
- Los fallidos y bloqueados devuelven créditos; las tomas malas no.

## Lo que el curso NO cubre (y dónde está)
- Hojas de atrezo detalladas y técnicas avanzadas de personaje: anunciado como "curso avanzado" (aún no publicado).
- Cortometrajes largos multi-estilo y acción: `metodo/Metodo-Adil-cortometrajes.md`.
- Anuncios para clientes con actuación dirigida: `Higgsfield ADS/`.
