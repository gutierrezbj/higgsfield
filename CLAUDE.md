# CLAUDE.md · repo higgsfield

Centro de producción de imagen y vídeo con IA de JRGB (Navegante). Este repo es la copia versionada del Project "Higgsfield" de claude.ai: método, guías, plantillas y skills. No hay código de aplicación.

## Cómo trabajar aquí
- Responder en español, directo y sin rodeos. Los prompts para los modelos van en inglés.
- Antes de guiar una producción, leer las fuentes del repo (`academy/`, `metodo/`, `Higgsfield ADS/`) y aplicar lo aprendido sin que Navegante tenga que recordarlo.
- Seguir el método acordado; no proponer atajos que se salgan de él.
- Bucle de producción: idea → prompt → draft 480p → un ajuste → 1080p solo la toma buena.
- No inventar: si algo no está en las fuentes, decirlo.

## Skills (en `.claude/skills/`, enlazadas a su carpeta real)
- `cineimage-soul` — prompts de imagen fija y localizaciones (Soul Cinema primero).
- `cinedance-lite` — prompts de vídeo para Seedance 2.5 (modo escritor y modo aleatorio).
- `ugc-video-creator` — vídeos UGC de creador con producto.
- `higgsfield-acting-skill` — bloque ACTING TASK para dirigir la actuación.
- `higgsfield-seedance-prompt` — prompts de Seedance del corto Blockbuster (bloques, FOV en grados, candados).
Nota: CINEIMAGE pone "Seedream 4.5 Edit" para editar; en el curso se edita con Seedream 5.0 Pro. Se sigue el curso.

## Generar desde aquí
En Claude Desktop (pestaña Code) el conector de Higgsfield ya viene: se genera sin instalar nada. Claude Code en terminal (otra máquina) no lo tiene; ahí hace falta la herramienta oficial (ver `conector/Workflows-conector-Higgsfield.md`): `npm i -g @higgsfield/cli`, `higgsfield auth login` (lo hace Navegante en el navegador) y `npx skills add higgsfield-ai/skills`. No instalar sin que Navegante lo pida.

## Archivos pesados
PDF, imágenes y vídeos van a Google Drive (carpeta Higgsfield), no al repo. Estructura en `00-Infraestructura.md`.

## Sincronía con el Project de claude.ai
El Project es la fuente de los chats. Si se cambia un documento aquí, avisar a Navegante para actualizarlo también en el Project (y al revés).
