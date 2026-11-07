# Centro de producción Higgsfield · dónde vive cada cosa (7-11-2026)

| Qué | Dónde | Para quién |
|---|---|---|
| Método, guías, skills, plantillas de prompts (texto) | Este Project de claude.ai (`academy/`, `Higgsfield ADS/`, `metodo/`, `conector/`) | Los chats de Claude |
| Lo mismo, versionado | Repo privado GitHub **gutierrezbj/higgsfield** (rama `main`, con CLAUDE.md y las 5 skills enlazadas en `.claude/skills/`) | Claude Code en cualquier máquina: `git clone https://github.com/gutierrezbj/higgsfield.git` |
| Material pesado: PDF, imágenes, vídeos, recursos de clientes, entregas | Google Drive (5 TB) · carpeta **Higgsfield** | Todo el equipo y todas las máquinas |

## Google Drive · Higgsfield
https://drive.google.com/drive/folders/1lgs-_HykJb3aS_wImMDzn97dqfMbju5P

```
Higgsfield/
├── 00_Academy/              material del curso (PDF, zip L3, biblioteca de prompts)
├── 01_Cortos-y-Series/      un subproyecto por corto o serie
├── 02_ADS-Clientes/         un subproyecto por <cliente>-<campaña>
├── 03_Biblioteca/           personajes, localizaciones y referencias reutilizables
│   └── skills/              instaladores .zip de las skills (para subirlas a claude.ai)
└── 99_Plantilla-proyecto/   copiar para cada proyecto nuevo
    ├── CHAR/      hojas de personaje
    ├── PROPS/     vestuario, atrezo, producto
    ├── LOCATION/  sets y paleta
    ├── SCENES/    vídeos generados (draft y final)
    ├── EDIT/      montaje, voz, música
    └── ENTREGA/   lo que se entrega
```
CHAR / PROPS / LOCATION / SCENES son las mismas carpetas del proyecto en Cinema Studio (método de Adil). Los nombres de archivo siguen la regla de Elements: mismo nombre en Claude, en Higgsfield y en Drive (con prefijo de cliente en ADS).

## Pendiente
- Hecho (7-11-2026): repo creado y con todo el contenido del Project. Si se cambia un documento en un sitio, se actualiza en el otro.
- Navegante: arrastrar a `00_Academy` los 5 archivos grandes de Descargas/HF (4 PDF y el zip de la L3). La conexión de Drive desde Claude no sube archivos de más de ~3 MB.
