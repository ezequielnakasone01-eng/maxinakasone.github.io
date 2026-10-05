# Formato de entrega

## Guion limpio
Un solo párrafo, solo el texto hablado, con el nombre del personaje delante de cada intervención. Debajo: duración aproximada y, si hay datos a confirmar, una línea con eso. Terminar preguntando si va así.

## Guion detallado (estructura fija)

```
# [Código] · "[Título del video]" · [País] · [producto y color] · ~[duración]

**Resumen** (3 a 5 líneas)

**Reglas para todas las escenas**
- Lugar y temporada
- Personajes (idénticos a la referencia cargada como ingrediente; quién habla)
- Alturas
- Producto (frase fija en inglés)
- Estética / cámara
- Audio
- Voz dentro de cada clip (etiqueta fija en inglés)

## Guion detallado
**Clip N · [Personaje] (a cámara / voz en off):** frase
[TIPO DE TOMA · ENCUADRE (duración): escenario completo si cambia, acción segundo a segundo, gestos, utilería, cámara, alturas, producto "idéntico al ingrediente de producto". Si es off: "Su voz sigue fuera de cuadro."]

## Prompts para Nano Banana (avatares y, si hace falta, escenarios)

## Cómo sale en Veo3 (tabla: clips, tipo, ingredientes)
```

## Qué trae cada [toma]
- Etiqueta: QUIRÓFANO, UGC A CÁMARA, UGC SELFIE, B-ROLL, B-ROLL UGC · CASO REAL, INSERTO MUDO, RADIOGRAFÍA, ANIMACIÓN 3D, PANTALLA DIVIDIDA, ESCENA X.
- Duración en segundos (hablados hasta 8 s; b-roll con cortes de 2 a 4 s).
- Lugar real del país (barrio, calle, plaza), hora y luz. Si cambia el escenario, describirlo entero.
- Personaje: edad, pelo, ropa, accesorios, calzado, "idéntico a la imagen de referencia cargada como ingrediente".
- Acción segundo a segundo, gestos, expresión, mirada.
- Utilería que hace real la escena (café, llaves, hojas secas, fotos).
- Cámara: trípode, en mano, selfie, ras de suelo, cenital; temblor leve.
- Altura: quién es más alto.
- Producto con la frase fija.
- Si hablan dos en cuadro: el otro "con la boca cerrada".
- NUNCA indicaciones de títulos o textos en pantalla.

## Voz dentro del clip (no se usa ElevenLabs)
Al final de cada prompt va una etiqueta idéntica en todos los clips del video, en inglés, con idioma, acento, edad y tono. Ejemplos:
- Narrador: "Off-screen male narrator voice-over in Spanish from Spain: deep, mature, warm, calm and confident Castilian voice, slow pace, the same narrator voice in every clip. No on-screen character speaks. Soft ambient sound underneath."
- Protagonista en primera persona: "The man's own voice, first person, in [idioma]: … the same voice in every clip." + "he speaks on camera with natural lip-sync" o "off-screen voice-over, his mouth stays closed".
- Vocero en quirófano o tienda: "The doctor speaks in Spanish from Spain: … the same voice in every clip." + "he speaks on camera with natural lip-sync" o, en insertos, "his voice continues off-camera, no one on screen speaks".
Cada frase de 18 a 20 palabras como máximo; si el cliente escribió frases largas, partirlas en dos clips sin cambiar el texto.

## Tabla de cómo sale en Veo3
| Clip | Contenido | Escenario | Ingredientes |
Indicar keyframes (frame inicial y final si hay transformación), qué se reutiliza entre países y duración total.

## Títulos
Tabla por idioma con Hook / Mitad / CTA, en mayúsculas, cortos y con un emoji al final. Indicar en qué clip va la mitad.
