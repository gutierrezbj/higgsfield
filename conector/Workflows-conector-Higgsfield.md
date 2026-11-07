# Conector de Higgsfield en Claude · qué trae (comprobado 7-11-2026)

En los chats de este Project, Claude tiene el conector de Higgsfield activo: genera imagen, vídeo y audio, edita, crea proyectos y Elements en Higgsfield, y consulta saldo (plan Plus). Además del generador directo, el conector trae **flujos de trabajo empaquetados** (cada uno es un SKILL.md que Claude carga antes de producir).

## Flujos de trabajo del conector
| Flujo | Para qué |
|---|---|
| product-photoshoot | Fotos de producto: packshot de estudio, lifestyle, producto con persona, pin de Pinterest, banner hero, carrusel, pack de anuncios estáticos, prueba virtual con modelo, conceptual/CGI, restyle |
| brand-asset-creation | Logos, identidad visual, kit de marca, mockups, merch, packaging, rótulos, brandbook, decks, gráficos sociales, carteles; también recolorear y exportar un logo oficial |
| ads-studio | Anuncios estáticos con copy e imagen (Meta, Instagram…) desde web de marca, foto de producto, enlace o solo un prompt |
| ugc-video | Vídeo UGC terminado: reseña de creador, producto con voz en off, unboxing, try-on, tutorial, tour de una web |
| ad-multiplier | Versiones de un anuncio de 4–30 s: cambiar personas, producto, fondo o rehacerlo para otro mercado o idioma |
| character-sheet | Hojas de personaje consistentes (fotorreal, editorial, anime, 3D, concept de juego) |
| thumbnail-generation | Miniaturas de YouTube e Instagram |
| faceless-video | Vídeo narrado sin presentador (explicativo, historia, infantil, cuento) con voz y subtítulos |
| narration | Voz en off ajustada a tiempos, o tu foto como narrador sobre un vídeo |
| video-montage | Montar clips, música, subtítulos quemados |
| video-editing | Edición y motion graphics sobre material existente |
| microdrama-ads | Microdrama publicitario con personajes que actúan y hablan |
| katana | Remix de vídeo a partir de una referencia |
| website-builder-flow | Webs, apps y juegos de navegador alojados en Higgsfield |
| reel-effects, color-grade, manga-engine, shorts-studio | Efectos de reel, etalonaje, manga, shorts (por comando) |

## CLI + skills de Higgsfield (`@higgsfield/cli` y `higgsfield-ai/skills`)
- Es para agentes de terminal (**Claude Code** en el Mac, Cursor, Codex), que no tienen el conector. Repositorio revisado: versión 0.14, 9 skills (generate, brandkit, product-photoshoot, soul-id, youtube-thumbnail, marketplace-cards, faceless-video, video-explainer, websites).
- En este chat **no hace falta**: el conector cubre lo mismo.
- Se instala solo si vamos a producir desde Claude Code (archivos en disco, tandas grandes). Órdenes: `npm i -g @higgsfield/cli` → `higgsfield auth login` (abre el navegador, lo hace Navegante) → `npx skills add higgsfield-ai/skills`.
- Regla acordada: cuando algo necesite ejecutarse en Claude Code, Claude avisa a Navegante con las órdenes exactas.
