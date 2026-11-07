# Lección 5 · Tomas 3 y 4 (prompt calcado del método de Adil)

- Toma 3: job 8ba4e90a-fade-4fc1-9ffb-8ad800421ba1 · archivo hf_20261026_131624_8ba4e90a...mp4 · seed 1414455451
- Toma 4: job 0367c5d4-b8c1-4e90-8ea3-511bfcc253b7 · archivo Los_chorros_JRyAB.mp4 · seed 2050959024
- Ajustes: Seedance 2.5 · 21:9 · 480p · 16 s · audio activado · 1/4 · ~48 cr
- Cambios T3 → T4: (1) plano 1 reescrito (cámara a ras del charco, derrape con salpicadura, Juan de frente, la cámara sube hasta su cara); (2) pronunciación de "chama".
- Error de T4: se pegó la línea de cambio con la flecha "→" y se perdió el final del plano 4 ("lets go of the strap... One second of silence."). Regla: los cambios se entregan siempre como el plano completo ya corregido.

## Lo que aprendimos
- La toma 1 falló porque copiamos la estructura de 3 partes sin la dirección. Cada plano necesita: función, tamaño de plano y ángulo, comportamiento de cámara (fija o movimiento con inicio y destino), acción en orden (primer término → personaje con el atrezo → la cámara se mueve).
- Hay que alternar: plano en movimiento para presentar y cámara fija para la reacción.
- Antes de entregar un prompt, compararlo plano a plano con el ejemplo de la lección.
- Seedance 2.5 Draft aparece como modelo aparte en el vídeo de Adil; en nuestra cuenta no está. La API sí tiene los campos draft / draft_job_id.

## Prompt T4 (versión limpia)
```
SCENE CONTEXT
At night, a classic early-1980s Malibu skids into the gravel parking lot of the roadside bar "La Última Parada". Juan gets out with the duffel bag of cash, Adri warns him about the police lights on the highway, Juan smiles, and they walk into the bar together, where Juan drops the bag on the counter.

REFERENCES
@juancho_V1.0 — Juan, 100% as shown in the reference image. He is the driver.
@adri_Adri_V1.0 — Adri, 100% as shown in the reference image. She is the passenger.
@malibu_Malibu_V1.0 — the car, 100% as shown in the reference image, same colour in every shot.
@prop_bolsa_dollar — the duffel bag, 100% as shown in the reference image. It belongs to @juancho_V1.0. He carries it on his right shoulder until he drops it on the counter.
@bar_frente_VArFrente_v1.0 — the bar seen from the parking lot. Use it for the light, colour, location and the neon sign.
@bar_porche_v1-0 — the same bar seen from the porch. Use it for colour and location, not for composition or framing.

SHOTS
Shot 1, 0-5s: Medium close-up, low-angle jib shot. The camera starts at ground level beside the puddle. The Malibu skids into frame, spraying gravel and puddle water, and stops. A trucker walks across the foreground. @juancho_V1.0 opens the driver's door and gets out facing the camera, with the duffel bag on his right shoulder. The camera rises to reveal his face as he looks towards the bar.
Shot 2, 5-8s: Static camera at eye level. @adri_Adri_V1.0 from the waist up, standing by the open passenger door, slightly side-on to the camera. She notices the red and blue police lights on the distant highway and taps the car roof to warn @juancho_V1.0.
Shot 3, 8-11s: Close-up of @juancho_V1.0 at eye level, three-quarter front view. Truck headlights pass in front of the camera. The camera holds while he glances at the police lights, then smiles calmly and exits frame from right to left.
Shot 4, 11-16s: From inside the bar, facing the entrance, medium distance. @juancho_V1.0 pushes the door inward and walks in with @adri_Adri_V1.0 beside him, drops the duffel bag flat on the counter with his right hand, saying "Llegamos, chama" (Venezuelan slang, pronounced CHAH-mah), lets go of the strap and leans on the bar. One second of silence.

CONTINUITY & SOUND
The duffel bag stays on Juan's right shoulder until it lands on the counter. The bar door opens inward. The police lights stay visible on the highway in shots 2 and 3. Depth in every shot: something close, something in the middle, something in the background. Rule of thirds. The bar is busy inside, as in the reference. Natural night ambience, gravel under the tyres, footsteps, clothing movement, bar chatter in shot 4. Juan speaks Spanish with a Caracas Venezuelan accent. No music.
```

- **Jerga y palabras regionales en diálogos (L05, 26-10-2026):** Seedance cambió "chama" por "chapa". Se arregló añadiendo la pronunciación en el prompt: `saying "Llegamos, chama" (Venezuelan slang, pronounced CHAH-mah)`. Regla: toda palabra de jerga o regional lleva la aclaración "(<origen> slang, pronounced X)" y se comprueba de oído en la revisión.
