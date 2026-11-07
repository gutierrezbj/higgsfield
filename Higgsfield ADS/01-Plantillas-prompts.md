# Higgsfield ADS · Plantillas de prompts

Estas plantillas salen de los prompts reales de Adil ("Animals"), con huecos `[...]` para rellenar. Van en inglés porque así están en la fuente y así responden los modelos.
**Uso normal:** no se rellenan a mano. Se le dan a Claude junto con la ficha del cliente, y Claude devuelve el prompt completo. Sirven para comprobar que no falte ningún bloque.

---

## P1 · Hoja de personaje — Seedream 5.0 Pro, 16:9, 2K

```
Photorealistic character sheet: two photographs side by side on a plain, neutral mid-grey studio backdrop — no texture, no windows, no objects, no room. The same [character] in both photos.

Character: one [character], the exact same individual in both photos: the same face, the same [skin/fur/hair], the same colors and the same build. [Who he/she is, age, build — "indistinguishable from a real [person/animal] photographed on set". For animals: "standing upright on his hind legs like a person".]

[FACE: detailed description — skin, eyes and gaze, nose, mouth closed, ears, hair.]
[BODY: build, hands/feet, colors of each zone.]

Left photo: head-and-shoulders portrait, front view, looking straight into the camera; [what must be visible]. The backdrop behind him is an even, neutral mid-grey.

Right photo: full-length front view cropped at the neck — the top edge of the photo cuts just below the chin, the head is completely out of frame. [Body, arms, hands and feet fully visible], standing upright with a soft contact shadow. Both arms hang relaxed at his sides, hands open and empty. The backdrop is the same neutral grey, slightly lighter toward the floor.

Soft diffused key light from the left, gentle shadow side on the right, no retouching. Not CGI, not a 3D render: no plastic look, no over-sharpening, no glossy render shine. Not cartoon, not a person in a costume. No text, labels, watermarks or logos anywhere.

Natural, true-to-life color: neutral white balance — no color grading, no tint, no desaturation, no green or olive cast. Soft contrast, sharp detail, very fine film grain. Naturalistic, documentary-like realism.
```

---

## P2 · Ropa (flat-lay) — Seedream 5.0 Pro, 16:9, 2K

```
Photorealistic flat-lay photograph of [a complete outfit / uniform] for [type of wearer, e.g. "a very large, heavy-set wearer"], shot from directly above on a solid, flat, uniform mid-grey background — plain seamless grey with no texture, no gradient, no objects. No person, no mannequin, no animal. The pieces are laid out as one outfit, in the order they are worn, neatly and clearly separated:
- At the top: [headwear or top piece, color with HEX].
- In the middle: [jacket/shirt, color with HEX, details].
- Below: [trousers, color, details — shown in full, both hems visible].
- On either side / at the bottom: [gloves, shoes, accessories].
Real fabric texture: creases, pilling, [level of wear]. The colors stay strong and true.

Crisp soft light from the top left with gentle natural shadows under each piece, rich contrast, vivid saturated true-to-life color, sharp focus across the whole layout, no retouching. Not CGI, not a 3D render, not an illustration. No text, labels, brand names or logos anywhere.
```

---

## P3 · Hoja de producto — Seedream 5.0 Pro, 16:9, 2K  [adaptación JRGB]

Misma lógica que la ropa. Si el producto tiene logo o etiqueta real, **se adjunta la foto real del cliente** y se pide conservarla; no se deja que el modelo invente el logo.

```
Photorealistic product sheet of [product], on a plain, neutral mid-grey studio background — no texture, no objects. [Front view on the left, three-quarter view on the right / or the views needed]. The whole product inside the frame, nothing cropped. [Materials, colors with HEX, size reference.] [If a real photo is attached: "Keep the product exactly as in the attached photo: shape, colors, label and logo unchanged."]
Soft diffused key light from the left, gentle natural contact shadow. Not CGI, not a 3D render. No invented text or logos.
```

---

## P4 · Set de entrevista — Soul Cinema, 16:9, 1080p

(Para vertical: generar en 9:16 y quitar "2.39:1".)

```
Cinematic interior shot, photorealistic, 35mm anamorphic film still. [The place] set up for a documentary interview, no people. Perfectly symmetrical frame: the camera stands at seated eye level, facing [the back wall] straight on, one-point perspective. A single [chair type] stands exactly in the center, empty and facing the camera, a few steps in front of [the back wall]. Behind it, [what is behind, mirrored on both sides]. [Materials and colors with HEX from the palette card]. Worn and lived-in. No text or logos anywhere.

In the soft out-of-focus foreground, [two matching objects] close to the lens frame the lower left and lower right corners symmetrically. Shallow depth of field with the empty chair in sharp focus; the background melts softly.

Lighting built for the interview: a soft key from a large off-screen window at front left, about 45 degrees to the chair, falls directly onto it, so whoever sits there is the brightest thing in the frame, with a gentle shadow side on the right. The room behind sits a stop or two darker: [cool practical] and [warm amber practical lamps], separating the sitter from the background.

SUBTLE anamorphic lens character: horizontal squeeze and compression, oval elliptical bokeh, horizontally stretched highlights, curved barrel edge distortion, chromatic aberration toward the edges. NO lens flares, NO light streaks, NO floating bokeh circles. 2.39:1.

Shot on 35mm film. [Palette with HEX codes: highlights, midtones, shadows, one accent.] Soft diffused light, low contrast, visible fine film grain. Warm amber only in practical lamps. Naturalistic, documentary-like realism. Seated eye-level, medium-wide framing.
```

Regla: alrededor de la silla, espacio limpio.

---

## P5 · Edición puntual — Seedream 5.0 Pro (imagen adjunta)

```
Edit the attached image. [Change: exactly what changes]. Keep [everything else / list what must stay] exactly the same. No person, no text.
```
Ejemplos reales: "replace the monitors with modern ones" · "remove the text on the toilet, replace it with WC" · "Show the whole pair of pants. Keep the clothes the same."

---

## P6 · Recolor — Seedream 5.0 Pro (imagen adjunta)

```
Recolor this image only — keep everything else exactly as it is: the same composition, framing, people, faces, clothes, objects, textures, lighting direction and every detail. Change only the color grade to [look]:
- highlights [tone, HEX];
- midtones [tone, HEX];
- shadows [tone, HEX];
- overall saturation [level], small accents keep their color [which, HEX];
- skin tones natural and warm;
- [contrast], fine film grain.
Do not add, remove or move anything. No text, no logos.
```

---

## P7 · A-roll (entrevista) — Seedance 2.5, plano de 14 s

Esta es la estructura del prompt del oso. La parte ACTING TASK la construye Claude con la acting skill.

```
ELEMENTS
@[set] = Set — defines the interview location: [place], the chair and its position, materials, light and palette only. [Which shot uses its exact framing.]
@[character] = [Name] — defines the [character]'s face, [skin/fur] and build only. Sheet background, layout and pose are not inherited.
@[outfit] = Outfit — defines the clothes [Name] wears only; he wears exactly this outfit.
[@[product] = Product — defines the product only; shape, colors and label unchanged.]

STYLE: photorealistic documentary interview, restrained and naturalistic, 35mm film, subtle anamorphic lens character, fine film grain, no lens flares.

LIGHTING: [Name] is lit softly from the front left; the room stays a step darker behind him in every shot.

COLOR: grade matches @[set]: [saturation], highlights (#...), midtones (#...), shadows (#...).

CAMERA: 14 seconds, [number] locked-off frontal shots joined by hard cuts at [Xs] and [Ys], camera at seated eye level, no camera movement inside any shot.

PHYSICS — [real weight and behavior: how the mouth shapes the words, skin/fur/clothes moving, breathing, the chair reacting to his weight, everything settling in the pauses].

RULES
1. [He sits on the chair for the whole 14 seconds and never stands up.]
2. He wears the outfit from @[outfit] in every shot.
3. The interviewer stays off-screen, just right of the lens, and is never seen or heard.
4. [What must NOT happen — e.g. no tears; the feeling lives in his eyes, breath and voice.]

CHARACTERS
[Name] — [posture].

ACTING TASK — [NAME] (he is fully invested in his tactic; the work happens in his eyes):
SCENE DIRECTION (shared, unspoken): [one line]
MOTIVE (his fuel): [...]
GOAL: [...]
OBSTACLE: [...]
TACTIC: [...]
Moment to moment:
— (0-0.8s, silence) — [...]
— "[line]" — [verb at the interviewer + what the eyes check]
— (pause) — [...]
— "[line]" — [...]
— ([X-Ys], listening) — [...]
— "[line]" — [...]
— ([end], silence) — [...]
(Safety: gaze always engaged in the task — never a frozen, glassy, unfocused stare; natural blink cadence.)
```
