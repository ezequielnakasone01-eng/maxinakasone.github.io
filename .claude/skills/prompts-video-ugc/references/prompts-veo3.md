# Prompts Veo3: arquitectura, plantillas, B-roll, negativos, QA

## Índice
1. Dividir en clips
2. Arquitectura del prompt
3. Plantilla maestra
4. Storyboard: SHOT vs MOMENT
5. Diálogo
6. Actuación y cámara
7. Patrones de B-roll
8. Negativos por riesgo
9. Ingredientes por tipo de clip
10. Caja / unboxing
11. Ejemplo resuelto
12. Checklist
13. Diagnóstico de fallos

---

## 1. Dividir en clips

- Por unidades narrativas, no por segundos. Cada clip = una función principal y un mini arco visual.
- Clip de 8–10 s → 3–5 shots internos de 1–3 s. ≈18–20 palabras por clip hablado.
- Si el texto no entra, más clips; nunca acelerar la dicción ni recortar palabras.
- Estructura típica de 5 clips: (1) hook + contexto · (2) evidencia / historia BEFORE · (3) cambio de experiencia AFTER · (4) demo de producto · (5) transformación + cierre/CTA.
- Hook: acción visible desde el segundo 0 (acercarse, bajar del coche, levantar el producto, empezar a caminar).
- Producto: cortar a manos, textura, lateral, talón, suela o puesto; nunca 7–8 s de alguien sosteniéndolo quieto.
- Transformación: acciones físicas reales, nunca morph.
- CTA: volver al rostro, conservar contexto, espacio limpio para gráficos.

## 2. Arquitectura del prompt (orden fijo)

1. **OBJECTIVE** — qué clip, quién habla, función narrativa.
2. **STRICT CONTINUITY** — identidad, vestuario, locación, luz, props/vehículo, estado (BEFORE/AFTER).
3. **STRICT PRODUCT CONSISTENCY** — bloque del cliente (si el producto es visible).
4. **IMPORTANT** — reglas globales: sin teléfono visible, nunca congelado, el diálogo no se reinicia.
5. **STORYBOARD RULE** — anti-grid.
6. **SHOT / MOMENT 1..N** — tiempo, encuadre, acción, manos, mirada, foco, diálogo.
7. **PERFORMANCE**
8. **CAMERA**
9. **NEGATIVE** — elegidos según los riesgos del clip.
10. **AUDIO** — ambiente y continuidad de voz.
11. **native [LOCALE] dialogue:** + diálogo exacto completo del clip.

## 3. Plantilla maestra

```
OBJECTIVE:
Create an ultra-realistic vertical 9:16 UGC [testimonial/demo/interview/B-roll] clip of [PERSON] in [LOCATION]. Narrative function: [hook / BEFORE evidence / product demo / CTA].

STRICT CONTINUITY:
Use the supplied [AVATAR/KEYFRAME] as the ABSOLUTE identity, wardrobe, location and lighting reference.
Same man: [age, hair, beard, key facial anchors].
Same wardrobe: [garment by garment].
Exact same location: [location anchors], same [light / time of day].
Persistent props: [open parcel on the counter / black car in background / …].
Narrative state: [BEFORE — generic loafers, natural height | AFTER — SAYU on, internal lift, same anatomy].

STRICT PRODUCT CONSISTENCY:
[Client product block.]

IMPORTANT:
The camera behaves like a handheld selfie/UGC camera, but NO PHONE OR CAMERA DEVICE EVER APPEARS IN THE FRAME.
The [SPEAKER] never stands frozen: hands, eyes, weight and props move naturally for a reason.
Dialogue continues seamlessly across cuts and must NEVER restart or repeat.
Only the [SPEAKER] speaks. [Other characters] keep their mouths closed.

IMPORTANT STORYBOARD RULE:
The following SHOTS happen chronologically inside ONE normal edited vertical video.
DO NOT create a storyboard grid, panels, borders, collage, split screen or simultaneous moments.
Each shot happens after the previous one.

SHOT 1 — 0:00–0:02:
[Framing]. [Action with start and end, which hand does what, where he looks].
The [SPEAKER] says: «[exact fragment]»
QUICK HARD CUT.

SHOT 2 — 0:02–0:04:
[Causal B-roll: framing, physical action, focus].
The [SPEAKER] continues off-camera: «[next exact words]»
QUICK HARD CUT.

SHOT 3 — 0:04–0:07:
[Return to face or second evidence]. «[continues]»
End while [he/hands] are still moving naturally.

PERFORMANCE:
Natural, conversational, understated. [Specific gestures tied to words]. Real eye movement camera → product → camera. No theatrical influencer acting. No frozen advertising pose.

CAMERA:
Raw handheld smartphone-style UGC. Vertical 9:16. Natural micro-shake. Minor imperfect reframing, sometimes a fraction late. Natural autofocus breathing in close-ups. Natural home exposure. Normal speed. Quick hard cuts only. No phone visible. No gimbal. No slow motion. No dolly, orbit, crane or slider. No cinematic shallow depth of field.

NEGATIVE:
NO generated text. NO subtitles. NO banners. NO website. NO music. NO floating product. NO CGI rotation. NO 360 spin. NO morphing. NO extra fingers. NO product redesign. NO frozen pose. [clip-specific negatives]

AUDIO:
Natural [location] ambience ([room tone, footsteps, cardboard, fabric, sole on floor]). One single continuous voice across all cuts. No added voice-over.

native [LOCALE] dialogue:
[SPEAKER]: «[FULL EXACT DIALOGUE FOR THIS CLIP]»
```

## 4. Storyboard: SHOT vs MOMENT

| Formato | Cuándo | Ejemplo |
|---|---|---|
| MOMENT 1..N | escena continua, físicamente conectada | entrevistador entra, llega a la mesa, pregunta y acerca el micrófono |
| SHOT + QUICK HARD CUT | ritmo de edición dentro del clip | plano medio → macro del cuero → lateral → suela → rostro |
| B-roll puro | sin diálogo ni lipsync | botín en manos, textura, elástico, pasos en adoquines |

Cada SHOT especifica: duración, encuadre, quién se mueve, qué hacen las manos, hacia dónde mira, qué queda en foco y qué frase suena en ese instante. Para UGC dinámico, cambio de plano cada ~1–3 s cuando el ritmo lo pide.

## 5. Diálogo

- Copia exacta del aprobado; nada de sinónimos ni retraducción.
- Cada línea dentro del SHOT/MOMENT donde se pronuncia **y** el diálogo completo del clip repetido al final tras la línea de idioma.
- Etiquetas de hablante inequívocas; turnos claros, nunca dos voces simultáneas salvo que el guion lo pida.
- B-roll en medio de una frase → `The MAN continues off-camera: «…»` desde la palabra siguiente.
- Números, precios, medidas y marcas escritos de forma pronunciable y siempre igual en todo el anuncio.

Correcto:
```
SHOT 1:
He says: «Vienen súper bien empaquetadas»
QUICK HARD CUT.
SHOT 2:
Close-up of the already-open package.
The MAN continues off-camera: «y las he pedido otra vez en la tienda oficial.»
```
Incorrecto: `SHOT 2: He starts again: «Vienen súper bien empaquetadas...»` → lipsync incoherente y audio duplicado.

## 6. Actuación y cámara

Cada shot lleva al menos una acción secundaria con motivo:
- Manos: apoyarse en la mesada, tocar la caja, indicar la puntera, ajustar el pantalón, gesto abierto, dos dedos apoyados.
- Mirada: cámara → producto → cámara; caja → cámara; pies → cámara.
- Cabeza: un asentimiento, leve inclinación, cejas.
- Peso: apoyarse de un lado, cambiar de pie, girar el tronco.
- Objetos y ropa: bajar una zapatilla, cambiar el agarre, acomodar dobladillo o manga.

"Siempre en movimiento" ≠ gesticular sin parar: cada gesto acompaña el significado y vuelve a reposo natural.

Señales UGC: micro-shake, reencuadre leve, llegar una fracción tarde a la acción, autofocus breathing, fondos vivos pero secundarios (peatones, camarero, hojas, tráfico suave), encuadre algo imperfecto, terminar en movimiento.

Regla de cámara: **imperfecto en cámara, preciso en dirección.**

## 7. Patrones de B-roll

El B-roll se coloca dentro del storyboard exactamente donde cubre su frase. Además se pueden generar B-rolls sueltos reutilizables para edición.

**Producto en manos (8 s):**
```
SHOT 1 — 0:00–0:02: Start from the reference frame. Hands hold the physical product close to camera and tilt it 15–20 degrees.
QUICK HARD CUT.
SHOT 2 — 0:02–0:04: Extreme close-up. Thumb runs across the [leather/mesh] once and gently presses it. Natural autofocus breathing.
QUICK HARD CUT.
SHOT 3 — 0:04–0:06: Tight side profile. Grip changes naturally, revealing [elastic panel and rear pull tab / ventilated side pattern].
QUICK HARD CUT.
SHOT 4 — 0:06–0:08: Tilt upward only enough to reveal the conventional outsole and heel, then return to lateral profile.
End while the hands are still moving naturally.
All product movement comes entirely from the hands; the product never moves on its own.
```

**Producto puesto:**
```
1. Both feet planted on [floor].
2. One natural heel-to-toe step.
3. Lateral ankle-height tracking shot.
4. Heel lifts briefly, outsole appears.
5. Camera rises from footwear to full body.
No body stretching. No magical height transformation. Natural trouser movement.
```

**Biblioteca mínima por producto:** en manos (lateral → textura → detalle funcional → suela) · puesto (pies quietos → paso lateral → talón → frontal) · macro de material presionado por un dedo · calzarse (abrir/elástico/tirador → pie entra → pantalón cae) · caminata contextual (producto nítido, fondo/vehículo desenfocado) · transición (cámara sube del calzado al protagonista).

**Jerarquía visual:** experiencia/objeción → rostro medio-corto · dolor → plano medio/3/4 con gesto sutil · pisada → plano bajo 3/4 de un paso completo · horma/mesh/puntera → close-up físico · altura/postura → plano entero eye-level · paquete → caja ya abierta · resultado → plano entero/medio con actividad natural.

**Vehículos y objetos de lujo:** contexto, no protagonista. Fijar modelo, color y posición en STRICT CONTINUITY; nítido en el hook, desenfocado en los close-ups de producto. La acción lo justifica (mirar el coche al nombrarlo, sostener las llaves, alejarse caminando).

**Insertos educativos (radiografía / presión / amortiguación):** solo si el concepto lo pide; sutiles, dentro de la geometría exterior real del producto, sin efectos de ciencia ficción, con espacio para el rótulo que va en edición.

## 8. Negativos por riesgo

No copiar una lista genérica: elegir según el clip.

| Riesgo | Negativo |
|---|---|
| Selfie artificial | NO phone visible. |
| Producto IA | NO floating product. NO CGI rotation. NO artificial 360 spin. NO product redesign. NO morphing. |
| Altura falsa | NO platform. NO visible hidden lift. NO body stretching. NO low-angle height trick. |
| Look publicitario | NO cinematic movement. NO cinematic orbit. NO slow motion. NO gimbal-perfect movement. NO dramatic studio lighting. |
| Edición errónea | NO grid. NO split screen. NO collage. |
| Overlay accidental | NO text. NO subtitles. NO banner. NO website. |
| Dolor exagerado | NO dramatic pain acting. NO medical graphics. |
| Avatar muerto | NO frozen advertising pose. |
| Anatomía | NO extra fingers. NO deformed hands. |
| Unboxing | NO opening the parcel. NO invented shipping labels or logos. |
| Audio | NO music unless explicitly requested. NO added voice-over. |
| Temporada | NO Christmas decorations. |

## 9. Ingredientes por tipo de clip

| Tipo de clip | Avatar/keyframe | Escenario | Foto producto |
|---|---|---|---|
| Hook con producto lejos | Sí | Sí o incluido en keyframe | Opcional |
| Close-up producto | Sí si aparecen manos/ropa | Sí | OBLIGATORIA |
| Cambio de calzado | Sí | Sí | OBLIGATORIA |
| Caminata con producto | Sí (master AFTER) | Sí | OBLIGATORIA |
| CTA medio | Sí | Sí | Recomendada |
| B-roll solo producto | Manos si importa continuidad | Sí | OBLIGATORIA |

## 10. Caja / unboxing casual

"Me acaba de llegar" no significa abrirla desde cero. Lo natural: caja ya abierta sobre la mesada, mano apoyada en el borde, mover apenas el papel protector, mostrar que el segundo par está ahí, mirar caja → cámara. Evitar: cortar cinta de forma teatral, abrir/cerrar solapas, sacar elementos uno a uno, logos o etiquetas de envío inventadas, pose de influencer.

## 11. Ejemplo resuelto — testimonial cocina, clip 1

```
OBJECTIVE:
Create an ultra-realistic vertical 9:16 UGC testimonial clip of a Spanish man around 60 years old speaking naturally from the kitchen of his home.

STRICT CONTINUITY:
Preserve exactly the same man, clothing, kitchen, daylight and open parcel.

IMPORTANT:
The camera behaves like a handheld selfie/UGC camera, but NO PHONE OR CAMERA DEVICE EVER APPEARS IN THE FRAME.
The MAN must never stand frozen. He accompanies what he says with small natural gestures, glances and weight shifts.
Dialogue must NEVER restart or repeat after a cut.

SHOT 1:
Medium-close kitchen UGC framing. He leans slightly against the counter and says the opening question while gesturing naturally.
QUICK HARD CUT.
SHOT 2:
Casual BEFORE B-roll: same man in ordinary loafers walks two steps and briefly presses one palm to his lower back.
The MAN continues off-camera with the next words.
QUICK HARD CUT.
SHOT 3:
Low casual insert of old loafers as he shifts weight. Voice continues, never restarts.
QUICK HARD CUT.
SHOT 4:
Back in kitchen. Parcel is ALREADY OPEN. He rests one hand on the edge and reveals the second pair without opening anything.

CAMERA:
Raw handheld smartphone-style UGC. Normal speed. No phone visible. No gimbal. No slow motion.

NEGATIVE:
NO generated text. NO subtitles. NO opening the parcel. NO medical graphics. NO dramatic pain acting. NO frozen pose. NO music.
```
(En producción, cada SHOT además lleva el fragmento exacto de diálogo y el prompt cierra con `native Spain Spanish dialogue:` + diálogo completo.)

## 12. Checklist (pasarlo antes de entregar cada prompt)

- ¿El clip tiene UNA función narrativa? ¿Qué estado es: BEFORE, transición o AFTER?
- ¿Está claro qué imagen es referencia de personaje, escenario y producto, y es el master correcto para ese estado?
- ¿Identidad, vestuario, locación, luz y props bloqueados y repetidos?
- ¿Producto con invariantes explícitas y mutaciones probables prohibidas?
- ¿Anti-grid explícito? ¿Cada acción tiene un orden físico posible y filmable con un móvil?
- ¿Diálogo exacto, asignado al hablante correcto, ubicado en su SHOT, cada frase una sola vez?
- ¿B-roll con "continues off-camera" donde corresponde? ¿El B-roll prueba la frase?
- ¿El diálogo cabe en la duración? Si no, ¿se dividió en más clips?
- ¿Números/precios/marca pronunciables y consistentes?
- ¿El sujeto hace algo con manos/cuerpo en cada shot y termina en movimiento?
- ¿La caja está en el estado correcto? ¿Sin teléfono visible?
- ¿Sin texto, subtítulos, banners ni web? ¿Espacio limpio si va gráfico?
- ¿Sin slow motion, gimbal ni look cinematográfico?
- ¿Avatar descrito con detalle suficiente para no salir genérico?
- ¿Línea de idioma/acento al final?
- Test final: si muteo, ¿los B-rolls explican lo que se dice? Si cierro los ojos, ¿suena como una sola toma continua?

## 13. Diagnóstico de fallos

| Problema | Corrección |
|---|---|
| Veo muestra cuatro cuadros a la vez | Anti-grid explícito + SHOTs como secuencia cronológica con hard cuts. |
| El calzado muta | Foto real + bloque de invariantes + repetir prohibiciones en el shot crítico. |
| Aparece plataforma externa | Declarar alza interna; suela exterior con grosor/forma exactos. |
| Se siente IA/cinematográfico | Más handheld, autofocus, pequeños errores de encuadre, gestos humanos, menos luz/composición perfecta. |
| Plano hablado aburrido | Intercalar inserts de producto con diálogo off-camera. |
| Personaje cambia entre clips | Keyframe maestro + repetir identidad/ropa/escenario en STRICT CONTINUITY. |
| Texto defectuoso en video | Quitar overlays del prompt; agregarlos en CapCut. |
| Producto flota al rotar | El movimiento viene enteramente de las manos; nunca se mueve solo. |
| Aparece un celular | Quitar toda mención de "selfie con teléfono"; "NO PHONE OR CAMERA DEVICE EVER APPEARS". |
| Avatar quieto mientras habla | Agregar acción secundaria con motivo en cada shot. |
| Diálogo repetido o voces cruzadas | Cada frase una vez, "continues off-camera", un solo hablante por clip. |
| Altura se finge con contrapicado o piernas largas | Cámara eye-level, plano entero, "same anatomy, no body stretching", master AFTER. |
