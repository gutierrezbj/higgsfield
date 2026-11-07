# Lección 4 · Crea y edita recursos

**Curso:** Creación con IA: primeros pasos (Higgsfield Academy)
**Fuente:** https://higgsfield.ai/es/academy/courses/ai-creation/create-and-edit-assets
**Materiales (leídos enteros):** vídeo de 26:43 (por subtítulos) · guía visual PDF de 31 páginas · Biblioteca de imágenes y prompts PDF de 27 páginas · `CINEIMAGE skill.zip` (solo trae `cineimage-soul/SKILL.md`, v2.7; el archivo de ejemplos que cita, `references/clean-midtones-examples.md`, no viene en el zip)
**Instructor:** Adil

---

## 1. Qué vas a conseguir

Preparar los **recursos de una escena** antes de generar vídeo: **personajes** (hoja de personaje), **localización** (generar y editar) y, si hace falta, **atrezo**. En la lección 5 esos recursos se combinan en vídeo con Seedance 2.5.

Idea central: *la diferencia entre un buen vídeo y uno mediocre empieza en las imágenes de referencia.* Seedance suaviza parte del "slop", pero no lo elimina: textura plástica, bordes raros o acabado artificial pasan al vídeo. Preparar los recursos es como elegir cámara, luz y estilo antes de rodar.

---

## 2. Los modelos de imagen (cuándo usar cada uno)

| Modelo | Fuerte en | Límites | Coste (vídeo) |
|--------|-----------|---------|---------------|
| **Soul Cinema** (Higgsfield) | Localizaciones con aspecto de película real: luz creíble, texturas naturales, gran rango tonal (bueno para vídeo), color | Solo texto→imagen o imagen→imagen **sin prompt**. Sigue peor las instrucciones (reinterpreta). Objetos rotos o desorden. De noche las sombras se van a negro y se pierde detalle que el vídeo no recupera | **0,125 cr** por imagen |
| **Soul 2.0** (Higgsfield) | **Casting**: caras distintas, reales, con imperfecciones. Es el motor de la skill Character Sheet | — | **0,125 cr** a 2K |
| **Seedream 5.0 Pro** | Mundos complejos, fantasía, ciencia ficción, arquitectura grande; estilos marcados; **edición** de imágenes conservando textura y cara | Con mucho detalle o mucha fantasía tiende a **look CGI**. **Repetición** de formas (helechos, costras de sal) | — |
| **GPT Image 2.5 Sunburst** | **Seguir instrucciones**: textos exactos, maquetación, infografías, **storyboards** | En localizaciones: exceso de detalle, sobre-nitidez, **ruido** en el cielo, poca profundidad, acabado pulido | — |
| **Nano Banana Pro** | Polivalente, sigue bien el prompt | Acabado "IA" por defecto; caras idealizadas y parecidas (en la prueba salieron "gemelos") | **3 cr** por imagen a 2K |

- Comparativa del vídeo: los mismos dos prompts de Seedance con recursos hechos en cuatro modelos. Los de Soul tienen "más alma" y aspecto de cine, y **cuestan 24 veces menos**.
- Higgsfield usa sobre todo **Soul y Seedream 5.0 Pro** para resultados de cine.
- Prueba de casting ("Portrait of a man in his mid thirties", 6 imágenes por modelo): Soul dio 6 caras distintas; Seedream y Nano Banana, 6 muy parecidas.

### Cómo detectar el "slop" (PDF p. 12–14)
Amplía y mira:
- **ruido o grano** donde la superficie debería ser lisa (cielo);
- **superficies demasiado nítidas** que dan sensación de render;
- **repetición** con misma forma, escala y espaciado (hierba, costras, helechos);
- **reflejos** que roban atención (baldosas mojadas);
- **falta de profundidad**;
- **el color**, que marca el look del vídeo final.

### Glosario (PDF p. 2–3)
Rango tonal · seguir el prompt · imagen→imagen · texto→imagen · AI slop · look CGI · **ancla espacial** (objeto visible para situar algo: "siéntalo junto a la jarra en el centro de la barra") · **plano inverso** (la escena vista desde la dirección contraria) · profundidad de campo · bokeh.

---

## 3. Preparar el espacio de trabajo (Cinema Studio)

1. Abre **Cinema Studio** en Higgsfield. Organiza las generaciones en **proyectos y carpetas**, con "me gusta" y filtros.
2. **New Project** → "Lesson 4" → Create. Debajo del nombre están las herramientas **Elements, Canvas y AI Director**.
3. **Add Folder**: una carpeta "Characters" y otra "Location" (y "Model testing" si comparas modelos).
4. Abajo, el **panel de generación** con dos pestañas: **Image** y **Video**. Pulsando el nombre del modelo se abre la lista.

---

## 4. Personajes

### 4.1 Con AI Director + Character Sheet (método del vídeo)
**AI Director** es un SuperComputer configurado para Cinema Studio (menú izquierdo → Tools; el chat se abre a la derecha).
1. Escribe el brief en lenguaje normal: *"a main character for a biker road movie, 25 years old, in modern clothing"*.
2. Escribe **char** → selecciona **Character Sheet** (comprueba que el chip de la skill está adjunto) → enviar.
3. Prepara **5 opciones de casting** con Soul 2.0: **0,625 cr** las cinco. Apruebas.
4. Eliges un candidato (Adil: el n.º 5, "the quiet outsider") y respondes las **preguntas de vestuario** (vaqueros rectos y botas de moto).
5. Prepara una **hoja de tres vistas en Seedream 5.0 Pro**: frente, espalda y retrato grande. Comprueba que cara, pelo, chaqueta y proporciones coinciden en las vistas.
6. Genera también **una versión con la cara pequeña tapada**. Truco: si las dos caras de la hoja (la del cuerpo entero y la del retrato) difieren un poco, el modelo de vídeo recibe señales contradictorias y la cara puede cambiar entre planos generales y primeros planos.

### 4.2 Editar el personaje (Seedream 5.0 Pro)
- Arrastra la hoja al campo de entrada y describe el cambio diciendo qué se mantiene. Usa el **mismo formato y la misma resolución** que la imagen original.
  ```
  Give him a silver wallet chain hanging off his jeans pocket. Replace the black t-shirt with a plain white ribbed cotton tank top. Same tank top in all views
  ```
- Compara con el original: cara, chaqueta y texturas iguales; solo cambian la cadena y la camiseta.

### 4.3 Tu cara + ropa de otro personaje
En el mismo chat de AI Director: *"one more character sheet using the face from the first image and the outfit from the second image"*. Adjunta **tu foto primero** y la del outfit después.
- Si la ropa de la referencia está cortada, el Director **pregunta cómo completarla** (vaqueros grises y botines).
- **Revisa el primer resultado:** el Director detectó que los vaqueros iban metidos en botas altas y propuso corregirlo. Solo se repite la parte baja; cara, chaqueta y composición se quedan.
- Prompt del PDF (p. 18): *"Use @Image1 only for identity… Use @Image2 only for clothing; do not transfer that person's face or identity."*

---

## 5. Localización

### 5.1 Generar (Soul Cinema)
- Carpeta "Location" → **Soul Cinema** → formato **21:9** (más espacio y aspecto de cine).
- "American bar" ya daría resultados, pero con una idea clara se escribe más concreto:
  ```
  Create an empty American dive bar. Place a dark wooden bar counter on the right, with leather stools and illuminated bottles behind it. Add a few neon signs, booths along the left wall, and a pool table at the far end beneath a hanging lamp. Frame the shot from the doorway.
  ```
- **4 generaciones** y comparar: la 1 demasiado granulada (parece de los 90), la 2 demasiado vacía, **la 3 es la más cercana** → base para editar. *Se elige por lo que necesita la escena, no por la más elaborada.*
- Empezar con la sala **vacía** permite juzgar la arquitectura y el espacio útil.

### 5.2 Editar (Seedream 5.0 Pro): gente + ancla espacial
- Arrastra la localización al campo de entrada; para ediciones sencillas basta lenguaje normal. Mismo formato, 4 variaciones:
  ```
  Add eight dive bar regulars - a mix of men and women. Some are playing pool, others are sitting at tables. Keep all bar stools empty, and place a single mug of beer in the middle of the bar counter.
  ```
- **La jarra es un ancla espacial**: en el prompt de vídeo basta con decir "se sienta en el taburete junto a la jarra del centro de la barra". Añadir anclas visuales a una localización es buena costumbre: ahorra tiempo, quita ambigüedad y sube las probabilidades de éxito en el vídeo.
- Comprueba el **número de personas** y su colocación; no des por hecho que siguió cada instrucción.

### 5.3 Plano inverso
Chat nuevo en AI Director: Seedream 5.0, cámara dentro del bar mirando hacia la puerta, plano más cerrado cerca de la entrada, con la puerta y un par de taburetes. Adjunta el bar como referencia.
- Prompt del PDF (p. 20): *"Use the attached image as the reference. Show the same bar from the opposite end, looking back towards the entrance… Keep the existing chairs and bar stools, preserving their designs and positions… Change only the camera viewpoint."*
- Revisa la continuidad: puerta, barra, taburetes. El modelo puede inventar cosas que no estaban (apareció una jukebox).

---

## 6. Atrezo (props)
- Mismo prompt en los cuatro modelos para comparar:
  ```
  A slim orange hard shell briefcase with a ribbed molded lid, rounded corners, a black top handle, and two metal latches. White background, soft studio light, no logos or text.
  ```
- Color llamativo (naranja) → punto focal y curiosidad.
- Mejor en **ángulo de tres cuartos**: da información del frente y del lateral, Seedance interpreta menos y el objeto se mantiene igual entre planos.
- Objetos complejos (detalles distintos en frente, espalda y lados) → **hoja de atrezo** con todos los ángulos (curso avanzado).

---

## 7. Técnicas extra

- **Elementos desenfocados en primer plano** → profundidad y simulación de diafragma abierto en el vídeo.
- **"shot on an anamorphic lens"** en Soul Cinema → bokeh y desenfoque anamórficos.
- **Técnica secreta Soul Cinema** (PDF p. 21–23): genera primero la composición en un modelo que sigue bien las instrucciones (**GPT 2.5 Sunburst**), luego arrastra esa imagen a **Soul Cinema sin texto** (al soltar la imagen la caja de texto se bloquea) → Generate. Soul Cinema mantiene el concepto y la arquitectura y le da luz, textura y profundidad de cine. Cada resultado varía detalles.
- **Prompt de Seedream para localizaciones** (PDF p. 24), 60–90 palabras, en este orden:
  1. "An empty photographic view of…" + el sitio + 2–3 elementos concretos con material;
  2. **para qué es el espacio** ("central open standing space allowing circular camera movement");
  3. **cámara**: posición, altura, dirección y lente;
  4. **de dónde viene la luz** (no "cinematic lighting");
  5. **acabado**: paleta corta, grano, 1–2 texturas;
  6. **exclusiones** cortas ("No people, writing or logos.").
  Ejercicio: fija sitio y propósito y cambia solo la altura de cámara.

---

## 8. Skill CINEIMAGE (cineimage-soul v2.7)

- Convierte una idea o una imagen de referencia en un prompt de imagen fija de cine, pensado sobre todo para **Soul / Soul Cinema**.
- Regla central: **controla la lógica, el contenido y la cámara; dirige la luz; no simules el render.**
- Reglas fijas:
  - **localización = vacía** salvo que pidas gente, con frase obligatoria de "no people… reflections…";
  - **lente**: posición, altura, dirección, focal, FOV y distorsión desactivada (sin anamórfico salvo que se pida);
  - **un solo estilo** (por defecto *cinematic editorial realism*);
  - **texto exacto** solo en objetos que llevan texto;
  - **base tonal neutra**, con el color de cada fuente contenido cerca de ella y sin tinte global.
- Flujo interno: modo (generar / editar / referencia / limpiar / diagnosticar) → reglas fijas → intención → jerarquía (sujeto o localización) → **mapa de localización izquierda/centro/derecha × primer plano/medio/fondo** → ficha de escena → completar características → lógica física → color → estilo → prompt en prosa → **verificación de 23 puntos**.
- Orden de modelos: Soul / Soul Cinema → Seedream (edición) → Nano Banana Pro → GPT Image.
- **Instalar en SuperComputer:** Skills (barra lateral) → Create new → Upload a skill → arrastrar `cineimage-soul.zip` → Save. **En Claude:** Customize → Skills → Add → Upload skill.
- **Usarla:** escribir **/cineimage** y elegir *cineimage-soul*. Ejemplo: *"An empty neighbourhood cafe just before opening, viewed from the entrance. Warm side light, worn wood and a clear path to the counter."*; con referencia: *"Keep this room's architecture and camera angle; make the light feel like early morning."*

---

## 9. Tarea de la lección

En la plataforma: **"Crea una hoja de personaje y luego genera y edita una ubicación. Añade la hoja de personaje y la ubicación antes y después de tu edición."** → **0/3 imágenes**. Desbloquea la lección 5.

Según el vídeo:
- **uno o dos personajes**, cada uno con su hoja;
- **una localización** donde ocurre tu escena;
- **unas cuantas ediciones deliberadas**: añadir gente, cambiar un objeto o meter un detalle con el que interactúe el personaje, al servicio de lo que pasa en la escena;
- subir las hojas + la localización **antes y después**;
- **una descripción corta de la escena y qué cambiaste**.

Estos recursos se usan en la **lección 5** (vídeo con Seedance 2.5).

---

## 10. Ideas clave para futuros proyectos

1. **Los recursos deciden el vídeo**: lo que tenga la imagen (plástico, bordes raros, color) pasa al vídeo.
2. **Soul para caras y localizaciones de cine (0,125 cr); Seedream 5.0 Pro para editar y mundos complejos; GPT para texto y storyboards.**
3. **Luz legible**: la dirección de la luz en la imagen se mantiene en el vídeo.
4. **De noche, cuidado con los negros**: el detalle perdido no vuelve.
5. **Hoja de personaje sin la cara pequeña** para que el vídeo no reciba señales contradictorias.
6. **Anclas espaciales** en la localización para dirigir la acción con una frase.
7. **Localización vacía primero**, luego editar.
8. **Atrezo en tres cuartos** y con color que destaque; hoja de atrezo si es complejo.
9. **Organizar en proyecto y carpetas** desde el principio.
10. **Elegir por lo que pide la escena**, no por la imagen más espectacular.

**Siguiente lección:** Lección 5 · Tamaños de plano y prompting (personajes en la localización, Seedance 2.5 a fondo, dirigir acción y cámara).
