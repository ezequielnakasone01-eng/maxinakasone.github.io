---
name: prompts-video-ugc
description: Genera guiones y prompts de video UGC para Veo3 (y keyframes/avatares para generador de imagen) para los clientes de la agencia, empezando por SAYU (calzado con alza interna). Usar siempre que el usuario pida un anuncio, concepto, guion, guion con tomas/B-roll, avatar, master/keyframe, prompt de Veo3, B-roll, adaptación a otro país (Italia, Portugal, Francia, Alemania, EE. UU.) o revisión de un prompt para un cliente — aunque no diga "skill" ni "Veo3", p. ej. "hazme un anuncio de SAYU con un médico", "pasa este guion a prompts", "adapta esto a Italia", "por qué Veo me muta la zapatilla".
---

# Prompts de video UGC (Veo3) por cliente

Sistema para dirigir una producción generativa: el prompt es una **mini hoja de rodaje**. La calidad no viene de hacerlo más "cinematográfico" sino de **reducir ambigüedad**: primero se fija lo que NO puede cambiar (personaje, escenario, producto, cámara), después se describe una secuencia física simple que una persona real podría grabar con un móvil, y al final se agregan diálogo y ritmo.

Objetivo de todo clip: que el espectador piense "esto lo grabó una persona" antes de pensar "esto es un anuncio".

## 0. Antes de empezar: cargar el cliente

1. Identificá el cliente. Su contexto vive en `clientes/<cliente>.md` (hoy: `clientes/sayu.md`). Leelo SIEMPRE antes de escribir copy o prompts: ahí están producto, orden de beneficios, oferta, precio, mercados, terminología por país y conceptos ya producidos.
2. Si el usuario trae material nuevo (fotos de producto, avatar ya generado, guion aprobado, nueva oferta), eso manda sobre el archivo del cliente. Si contradice algo (p. ej. otro precio), preguntá cuál vale y ofrecé actualizar `clientes/<cliente>.md`.
3. Si es un cliente nuevo, creá `clientes/<cliente>.md` copiando la estructura de `clientes/sayu.md` y pedí los datos que falten (producto, público, beneficios en orden, oferta, mercados, qué funcionó).

## 1. Detectar en qué etapa entra el pedido

El pipeline completo es:

| # | Etapa | Entregable | Referencia |
|---|---|---|---|
| 1 | Concepto | Ficha de concepto (4–8 líneas de historia) | `references/guionado.md` §Concepto |
| 2 | Guion limpio | Solo diálogo / VO, sin tomas | `references/guionado.md` §Guion limpio |
| 3 | Guion con tomas | Diálogo aprobado + `[TOMA X (N s): …]` | `references/guionado.md` §Guion con tomas |
| 4 | Avatares y masters | Prompts de imagen: avatar, escenario, producto en mano, BEFORE/AFTER, CTA | `references/avatares-masters.md` |
| 5 | Prompts Veo3 | Un prompt por clip (5–10 s) con storyboard integrado | `references/prompts-veo3.md` |
| 6 | B-roll extra | Prompts de B-roll reutilizable | `references/prompts-veo3.md` §B-roll |
| 7 | Edición | Lista de overlays para CapCut (no van en el render) | este archivo §5 |
| 8 | Localización | Misma estructura, mundo del país | `references/guionado.md` §Localización |

Empezá en la etapa que corresponda al pedido y no te saltes aprobaciones:
- "Quiero un anuncio de X" → etapa 1 + 2 y **pará** para aprobación del guion limpio (el copy se aprueba sin ruido de producción). Si el usuario pide todo de una, hacelo todo pero marcá el guion limpio como "pendiente de aprobar".
- "Este guion ya está aprobado, pasalo a prompts" → etapa 3 (si no tiene tomas) → 4 → 5.
- "Adaptalo a Italia" → etapa 8 sobre el material existente.
- "Veo me hace X mal" → `references/prompts-veo3.md` §Diagnóstico.

Leé solo las referencias de las etapas que vas a ejecutar.

## 2. Reglas que nunca se rompen

1. **El diálogo aprobado es sagrado.** Se copia palabra por palabra en los prompts: sin resumir, sin sinónimos, sin retraducir. Si no cabe en el clip, se divide en más clips; nunca se acelera ni se recorta.
2. **El diálogo es una sola pista continua.** Los cortes son solo visuales. Al cortar a B-roll: `The MAN continues off-camera:` y se sigue desde la palabra siguiente. Nunca reiniciar ni repetir una frase.
3. **Una sola persona habla por clip.** El resto mantiene la boca cerrada. Etiquetas inequívocas (MAN, WOMAN, DOCTOR, INTERVIEWER, FOUNDER…).
4. **El B-roll demuestra la frase**, no decora. Si no prueba lo que se acaba de decir, sobra.
5. **El producto es la foto real** (referencia ABSOLUTA). Se sostiene, se apoya, se calza o se pisa; nunca flota, nunca gira 360°, nunca se rediseña. Beneficios internos (alza) quedan internos e invisibles.
6. **Storyboard secuencial dentro de UN video**: SHOT/MOMENT + QUICK HARD CUT, con la aclaración anti-grid obligatoria.
7. **Cámara de smartphone UGC**: handheld, micro-shake, autofocus breathing, velocidad normal. Nada de gimbal, slow motion, dolly, orbit, look de spot. Sin teléfono visible salvo que el guion lo pida.
8. **Nadie queda congelado.** Cada shot tiene una acción secundaria con motivo y termina en movimiento.
9. **Cero texto generado.** Subtítulos, precios, "+10 CM", badges, web, garantía → edición. En el prompt se pide espacio limpio.
10. **Cada prompt es autónomo.** Veo no recuerda el clip anterior: repetir identidad, vestuario, locación, luz, props, estado y producto en cada uno.
11. **Línea de idioma al final**: `native Spain Spanish dialogue:` / `native Italian accent dialogue:` / etc., seguida del diálogo exacto completo del clip.
12. **No inventar operaciones comerciales** (cambios de talla, promos, procesos) que el cliente no confirmó.

## 3. Formato de salida

Entregá en Markdown, con cada prompt dentro de un bloque de código para copiar y pegar directo. Encabezá cada bloque con lo que necesita el operador:

```
### CLIP 2 — Evidencia BEFORE (≈8 s) · estado: BEFORE
Ingredientes: avatar_hombre_BEFORE.png · master_cocina.png · (producto: no aparece)
Diálogo del clip (19 palabras): «…»
```
seguido del prompt en inglés (estructura de `references/prompts-veo3.md`).

Para guiones: guion limpio en prosa con hablante; guion con tomas con `«frase»` + `[TOMA X (N s): …]` debajo.

Al final de un paquete completo agregá:
- **Tabla de ingredientes por clip** (qué avatar/master/foto de producto adjuntar a cada uno).
- **Lista de overlays para CapCut** (precio, envío, garantía, "+10 CM", subtítulos, CTA).
- **QA**: confirmá que pasaste el checklist de `references/prompts-veo3.md` §Checklist; si algo no pasa, decilo.

Si el usuario lo pide como archivo (.docx/.md), generalo con el mismo contenido.

## 4. Idioma

Hablale al usuario en español rioplatense/neutral como él. Guiones en el idioma del mercado (España: tuteo peninsular). Prompts de Veo3 e imagen **en inglés**, salvo el diálogo, que va en el idioma del mercado.

## 5. Qué va a edición (nunca al render)

Subtítulos · precio y moneda · "ENVÍO GRATIS" · "30 DÍAS" · "+10 CM" / "+8 CM" · web · badges · escasez en texto · comentarios/reseñas/UI de WhatsApp exacta · música (salvo pedido explícito). En el prompt: "leave clean space in the upper third for graphics added in editing".
