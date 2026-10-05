# Avatares, escenarios y masters (prompts de Nano Banana)

Complementa a `prompts.md`: las plantillas base (lookbook, keyframe UGC, selfie, animados) están allá y mandan. Acá está el nivel de detalle que debe tener cada avatar y qué masters generar antes de Veo3. Recordá: avatares distintos por país, edad visible de 55 a 65 con marcas reales, y "no text, no labels".

Antes de Veo3 se fijan visualmente todos los estados críticos del guion. No hay un número fijo de masters: se generan **tantos como el guion necesite**. Cada clip usa como ingrediente el master que corresponde exactamente a su estado narrativo; nunca reutilizar uno incorrecto para ahorrar pasos.

## Las cuatro anclas de continuidad

| Ancla | Qué se fija | Cómo se protege |
|---|---|---|
| Personaje | cara, edad, pelo, barba, ropa, accesorios, proporciones | mismo avatar/keyframe + repetir identidad y vestuario en cada prompt |
| Escenario | arquitectura, mobiliario, piso, luz, objetos, posición | frame del escenario como ingrediente + "exact same location" |
| Producto | forma, material, costuras, suela, color, elástico, tirador | foto real obligatoria en close-ups + STRICT PRODUCT CONSISTENCY |
| Cámara/estilo | 9:16, smartphone, handheld, micro-shake, autofocus | repetir lenguaje UGC y prohibir gimbal, slow motion, look de spot |

## Avatar: nivel de detalle obligatorio

Un avatar es una referencia de identidad, no una descripción genérica. Especificá:
- **Rostro:** edad exacta o rango muy acotado, forma facial, asimetrías leves, textura de piel y poros, líneas de expresión, cejas, ojos, nariz, labios, barba/afeitado, distribución concreta de canas.
- **Pelo:** color, largo, densidad, peinado, entradas, canas, textura, mechones fuera de sitio. Nada de peluquería perfecta salvo que el concepto lo pida.
- **Cuerpo:** altura de referencia si importa, complexión, hombros, cintura, proporciones normales, postura inicial.
- **Vestuario prenda por prenda:** color, material, caída, ajuste, accesorios, calzado. Es una constante que se repite en los prompts de video.
- **Personalidad visible:** sereno, cercano, elegante, cansado, inseguro, enérgico… traducido en postura, mirada, gesto y uso de manos.
- **Imperfecciones útiles:** arrugas de ropa, asimetrías, barba no uniforme, textura real.
- **Referencia limpia:** cuerpo entero, cara + manos + calzado visibles, perspectiva natural de smartphone, fondo que no compita.
- **Calzado del avatar base:** si el producto todavía no debe aparecer en la historia, usar calzado genérico claramente distinto (p. ej. mocasines marrones gastados). Si el producto está desde el segundo 0, integrarlo en el master.
- **Estados:** si cambian calzado, altura, postura o vestuario, crear referencias separadas BEFORE y AFTER. No pedirle a Veo que invente la transformación.

Plantilla (inglés):
```
Ultra-realistic full-body reference photo, vertical 9:16, natural smartphone perspective at eye level.
[NATIONALITY] man, exactly [AGE] years old, [BUILD], [HEIGHT if relevant], normal real-world proportions.
FACE: [shape], slight natural asymmetry, real skin texture with visible pores, [expression lines], [eyebrows], [eyes], [nose], [lips], [beard/shave detail], [grey distribution].
HAIR: [color], [length], [density], [style], [receding hairline / temples], a few strands out of place, not salon-perfect.
WARDROBE: [top: color, fabric, fit, natural creases], [trousers: color, cut, how hem falls], [accessories: watch, ring…], [footwear: generic, clearly NOT the product / or product per reference].
POSTURE & PERSONALITY: [attitude] shown through [stance, gaze, hands].
Hands fully visible with natural nails and skin texture. Feet and footwear fully visible.
Background: [simple version of the location], softly secondary, does not compete with the subject.
Natural [daylight/indoor] light. No studio lighting. No beauty retouching. No text. No logos.
```

## Escenario maestro

Cuando hay varios clips se fija el lugar antes del video: arquitectura, piso, luz, mobiliario, objetos persistentes, hora del día. Ejemplos ya usados: cocina de casa española clase media-alta con mesada y caja abierta; terraza de trattoria con mesa de madera, espresso y adoquines; villa italiana con fachada clara, cipreses, entrada de madera y camino adoquinado; pasillo de hospital con control de enfermería.

```
Ultra-realistic vertical 9:16 photo of [LOCATION], shot from a natural smartphone at eye level.
Architecture: [...]. Floor: [...]. Furniture and persistent objects: [exact positions].
Time of day and light: [autumn morning daylight / hospital fluorescent…].
Lived-in details: [minor wear, everyday objects not perfectly aligned].
No people [or: background people far and out of focus]. No text. No logos. Not a studio set.
```

## Tipos de master

- **Escenario:** arquitectura, luz, muebles, objetos, vehículo, mesa, espejo, hora del día.
- **Interacción:** dos o más personajes juntos; fija distancias, relación de altura, dirección de miradas, posiciones.
- **Producto en mano:** si se sostiene, entrega, abre o enseña; protege manos, escala y orientación.
- **BEFORE / AFTER:** obligatorio si el anuncio depende de una diferencia visual (altura, postura, calzado, desgaste, presencia). Mismo cuerpo, misma ropa, mismo lugar; cambia solo lo que el estado exige. AFTER: "same exact person and anatomy, no body stretching, posture slightly more upright, height difference only from the internal lift; outsole keeps its exact real thickness".
- **CTA / mostrador:** si el cierre ocurre en otra posición, con caja, mesa, checkout o espacio limpio para gráficos.

## Ficha de producto

Antes de escribir cualquier clip se redacta la ficha de invariantes del producto (las frases fijas de SAYU están en `productos.md`). Para un producto nuevo:
```
STRICT PRODUCT CONSISTENCY:
Use the supplied real [PRODUCT] images as the strict product reference.
Preserve the exact [COLOR/MATERIAL], [UPPER DETAILS], [SIDE DETAILS], [TOE], [HEEL], [OUTSOLE] and proportions.
Do NOT redesign the product. Do NOT invent logos.
Do NOT change the sole geometry or thickness. Do NOT create an exaggerated platform.
Do NOT expose any hidden internal lift. Do NOT morph the product between shots.
```

## Paquete por anuncio

Cada anuncio = cinco piezas: (A) ficha de producto, (B) avatar(es), (C) escenario/masters, (D) prompts de clips, (E) biblioteca de B-roll. Fijadas A–C, el resto es modular. Al entregar masters, listá por cada uno: nombre de archivo sugerido (`avatar_medico.png`, `master_hospital_pasillo.png`, `master_AFTER_pareja.png`…) y en qué clips se usa.
