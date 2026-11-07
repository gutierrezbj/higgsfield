# Higgsfield Academy · material del curso en este Project

Curso: **"Creación con IA: primeros pasos"** (Higgsfield Academy, higgsfield.ai/es/academy). Es el único curso publicado a 7-11-2026: introducción + 7 lecciones, 1 h 42 min, profesor Adil. Navegante lo tiene completado (certificado, logro "Foundation", Creator Drop). La Academy anuncia cursos avanzados "en preparación".

## Qué hay en `academy/`
| Archivo | Para qué |
|---|---|
| `00-LEEME-Academy.md` | Este índice y cómo arrancar el chat del curso |
| `01-Leccion-por-leccion.md` | El método de cada lección (de la transcripción completa), ajustes, costes, tareas, y el estado de los PDF |
| `02-Entregables.md` | Qué podemos producir, con qué modelo y qué skill, y las reglas comunes |
| `03-Guias-PDF-L4-L5.md` | Las guías PDF de L4 y L5: modelos, "spot the slop", prompts de hoja de personaje y ediciones, técnica GPT→Soul Cinema, fórmula Seedream, plantilla de escena, reparación de prompts y todas las cláusulas de cámara |
| `Academy-L4-Biblioteca-prompts.md` | Los 26 prompts completos de la biblioteca de imágenes de la L4, texto exacto extraído del PDF |
| `skills/cineimage-soul/SKILL.md` | Skill CINEIMAGE v2.7 (L4): prompts de imagen fija, sobre todo localizaciones, con Soul primero |
| `skills/cinedance-lite/SKILL.md` | Skill "Seedance Prompter" = CINEDANCE LITE v3.0 (L6): prompts de vídeo para Seedance 2.5 (modo A escritor, modo B aleatorio) |
| `skills/ugc-video-creator/SKILL.md` | Skill UGC Video Creator (L3): vídeos de creador con producto, grabados con móvil |

Las tres skills están copiadas **sin cambios** de los archivos oficiales de la lección (comprobado byte a byte); solo se añadió una línea de comentario con la fuente debajo de la cabecera.

## Cómo encaja con lo que ya había en el Project
- `metodo/Metodo-Adil-cortometrajes.md` → cortos (Blockbuster 4K y 8 escenas/8 estilos).
- `metodo/Adil-ahorro-creditos-Animals.md` y `Higgsfield ADS/` → anuncios tipo falso documental, skill de actuación.
- `Higgsfield ADS/skills/higgsfield-seedance-prompt/SKILL.md` → skill de prompts de Seedance del corto Blockbuster (más técnica: FOV en grados, bloques, candados). La del curso (`cinedance-lite`) es la versión de principiante; para escenas con referencias y planos se puede usar cualquiera de las dos, sin mezclar estructuras en el mismo prompt.
- Diferencia a tener presente: CINEIMAGE pone "Seedream 4.5 Edit" en su orden de modelos para editar, pero en la lección 4 Adil edita con **Seedream 5.0 Pro**. Seguimos la lección.

## Cómo usar las skills en un chat de este Project
- Como instrucciones: adjuntar o citar el `SKILL.md` y decir "usa CINEIMAGE / Seedance Prompter / UGC Video Creator".
- Instaladas en Claude (para que salten solas): Customize → Skills → + → subir el `SKILL.md` (o un zip con la carpeta). En Supercomputer de Higgsfield: + → Attach file → subir el `.md`.

## Arranque del chat del curso (pegar como primer mensaje)
> Este chat es el taller del curso de Higgsfield Academy. Lee `academy/00-LEEME-Academy.md`, `academy/01-Leccion-por-leccion.md` y `academy/02-Entregables.md`, y usa las skills de `academy/skills/` según toque (CINEIMAGE para imágenes de localización, Seedance Prompter para vídeo, UGC Video Creator para anuncios de creador). Sigue el bucle del curso: idea → prompt → draft 480p → un ajuste → 1080p. Primer encargo: [qué quieres hacer].
