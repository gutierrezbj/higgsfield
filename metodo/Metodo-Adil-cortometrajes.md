# Método de Adil para cortometrajes (fuentes leídas enteras el 26-10-2026; vídeo A revisado de nuevo el 7-11-2026)
- Vídeo A: "I Made a Viral AI Short Film From Scratch — Full Workflow (Seedance 4K)", 39 min, transcripción completa: https://www.youtube.com/watch?v=CHHH8tNioSc. Proyecto: higgsfield.ai/@adilinthewild/projects/4k-blockbuster-breakdown (13.491 generaciones, 937.489 créditos, 3:22 min).
- Vídeo B: "How To Make an AI Animated Short Film (Full Workflow)", 15 min, transcripción completa. Librería de prompts de las 8 escenas: higgsfield-ai.notion.site/Short-film-prompt-library-all-8-scenes-33dea9455d118096af4cec86fc6d15e0
- Skills: Blockbuster → enlace en la descripción (higgsfield.ai/s/blockbuster-4k-higgsfieldai-hDUIci); 8 escenas → "Seedance-2-Skill.md" (Dropbox, en la descripción del vídeo B). Complemento: skill de actuación de "Animals" (ver metodo/Adil-ahorro-creditos-Animals.md).

## A · Blockbuster (acción en imagen real, 4 mundos)
1. **Guion con Claude por entrevista**, nunca "escríbeme un guion": idea → preguntas (duración, ambientes, giros) → guion. "Nada bueno sale de una petición perezosa."
2. **Cinema Studio → proyecto → carpeta por escena con subcarpetas por recurso.** "Dentro de 400 generaciones lo agradecerás." El **lienzo (canvas)** es el espacio de trabajo: ahí van todos los recursos finales, a la vista.
3. **Hoja de personaje:** cuerpo entero de frente y de espaldas + primer plano, **fondo gris** (más tomas válidas). El primer plano da la cara exacta y el cuerpo entero da la altura. GPT Image 2 para hojas fotorrealistas y ediciones. **Borrar la cara del panel de cuerpo entero → una sola cara** (si no, la identidad se desvía en cada escena).
4. **Localizaciones:** "si el set parece barato, cada plano también". Claude mejora el prompt; Soul Cinema en tandas (8 imágenes = 1 cr); **pedir ángulo de 3/4** (da profundidad a la cámara); fuentes de luz motivadas (farol + rayos de luz). Elegir la versión donde el elemento clave (el mapa) se lee bien.
5. **Atrezo:** pasada en bruto con Soul Cinema → edición con GPT Image 2 (velas negras, logo…).
6. **Nombrar cada recurso igual en Claude y en Elements** → los prompts se emparejan solos.
7. **Escenas:** skill de Claude (constructor de prompts) + recursos + guion + qué pasa → Seedance: 21:9, 4K, 15 s, **4 tandas**. Se revisa, se le dan los comentarios concretos a Claude y se repite. **En el montaje se cogen los mejores segundos de cada tanda.**
8. Trucos:
   - **dibujar un boceto** de la geometría ("un dibujo dice lo que 10 frases no"); cada tanda fallida que evitas ahorra créditos;
   - **localización aparte** para un sitio concreto (el oasis);
   - si cambia el vestuario a mitad de historia → **nueva hoja con la ropa rota**;
   - si un recurso queda caricaturesco → cambiarlo (mandriles → macacos); tener variantes preparadas;
   - un plano que falla en multiplano → hacerlo como toma continua sola (el POV del despertar);
   - **diálogo:** plano y contraplano del mismo sitio, cámara fija, regla de 180°, contraplano sobre el hombro izquierdo, tono de cada frase escrito; **referencias de las dos caras de la habitación** para que el fondo no salte entre cortes; fijar el tamaño de los objetos clave;
   - transiciones entre mundos escondidas en polvo o en un blanco; dejar **un respiro al inicio del plano** para que el corte desde la escena anterior funcione;
   - que el personaje **reaccione** a lo que pasa a su alrededor (la escena se siente real); el humor está en los cortes (multiplano para comedia).
9. Prefijo de estilo fijo (copiado de la ficha del proyecto): anamórfico 21:9, imagen real fotorrealista, ópticas de cine de aventuras (crash zoom, seguir proyectiles, tomas únicas, POV), una fuente de luz motivada, grade apagado por mundo + un acento saturado, piel a nivel de poro, actuación a nivel muscular, física respetada, continuidad fijada, solo SFX y diálogo, sin música (la música se pone en postproducción). "Candados positivos": número de personas, geografía de pantalla, estado del atrezo y eje de 180° escritos en cada prompt.

## B · 8 escenas, 8 estilos (animación)
1. Personaje: Soul Cinema con un prompt mínimo + **enhancer activado** ("se vuelve creativo"). Si algo no encaja → Nano Banana Pro cambia solo eso.
2. Objeto conductor (reloj): Claude → prompt de hoja de atrezo (vistas ortográficas, despiece) → Nano Banana Pro. Varias vistas = consistencia en todas las escenas.
3. Escena 1: fotograma clave + hoja del objeto → Claude con la skill → prompt por planos de ≤15 s → Seedance 2.0.
4. **Clave del encadenado:** en cada escena nueva se le da a Claude el fotograma clave nuevo + **el prompt de la escena anterior**, y a Seedance el prompt + el fotograma clave (referencia de estilo) + **el vídeo anterior** ("Extend @video1. Continue exactly from the white flash of the last frame").
5. Un estilo por escena = una generación de ≤15 s (montaje fácil). Cada escena termina en el teletransporte (flash blanco).
6. La escena final, sin fotograma clave: hoja del objeto + primer vídeo + descripción. Seedance inventó a Anna y mantuvo el estilo.
7. En la imagen de estilo: "DO NOT use the character from @image; create a NEW original character in the same style".
