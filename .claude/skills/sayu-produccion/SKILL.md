---
name: sayu-produccion
description: Producción de guiones UGC con IA para el cliente SAYU (zapatillas con alza de +10 cm, botines Chelsea de +8 cm y la zapatilla nueva de testeo sin altura) en España, Italia, Francia y Portugal. Úsala SIEMPRE que se hable de SAYU, Mariano, sus zapatillas o botines, de la tanda de 72 videos, de guiones con [b-rolls], avatares o keyframes para Nano Banana, prompts para Veo3, títulos de hook/mitad/CTA, adaptar un guion a otro país, o de cualquier código de video como ZB-A1, BO-E2 o ZN-F1, aunque no se mencione la palabra "skill".
---

# SAYU · Producción de guiones UGC con IA

Maxi produce videos UGC con IA para anuncios de Meta del cliente SAYU (contacto: Mariano). Esta skill concentra todo lo que ya se decidió en el proyecto para no tener que repetirlo en cada chat. Antes de escribir, leé la referencia que corresponda: ahí están los datos exactos de producto, las reglas que el cliente ya corrigió y las plantillas de prompts.

## Herramientas y flujo de producción

1. **Guiones:** se escriben acá con Claude.
2. **Imágenes** (avatares, escenarios, keyframes, storyboards): Nano Banana, con prompts en inglés.
3. **Video:** Veo3, clips de 8 s (a veces 10). Las imágenes de Nano Banana van como ingredientes.
4. **Voz:** va DENTRO de cada clip de Veo3. **No se usa ElevenLabs.** La locución se escribe dentro de las indicaciones de cada toma para que ChatGPT la meta en el prompt de Veo3.
5. **Edición:** CapCut (cortes, títulos, pantallas divididas, música). Los títulos y textos los agrega Maxi; nunca van en el guion.

## Cómo hablar con Maxi

- Siempre en español, tono cercano y directo. Maxi escribe en rioplatense con voseo y muchas veces por dictado de voz: interpretá la intención aunque haya errores de tipeo.
- Diálogos y locuciones en el idioma del país del video; indicaciones de tomas en español; prompts de imagen y video en inglés, en bloques de código.
- Si un guion queda corto o básico, lo va a rechazar: más historia, más mecanismo, más detalle (salvo retargeting, que va al hueso).
- Cuando corrige algo, aplicá la corrección a todos los videos siguientes sin que lo repita.
- Si pregunta "¿qué sigue?" o "¿qué falta?", mostrá una tabla de estado (hecho / pendiente) con los códigos del plan y proponé el siguiente.

## Orden de entrega de cada video

1. Si pide ideas: 6 a 12 opciones de formato + ángulo en tabla, con una recomendación. Esperá que elija.
2. **Resumen** corto (3 a 5 líneas).
3. **Guion limpio** en UN SOLO PÁRRAFO, solo el texto hablado, con el nombre del personaje si hay diálogo. Esperá el ok.
4. Con el ok: **guion detallado** completo, toma por toma (ver `references/formato-entrega.md`). Siempre completo, nunca "solo los cambios".
5. **Prompts de Nano Banana:** avatares y, si hace falta, escenarios/keyframes.
6. **Tabla de cómo sale en Veo3** (clips, tipo, ingredientes).
7. **Títulos** (hook, mitad, CTA) cuando los pida.
8. **Adaptación** a los otros países, cada uno completo.

Cuando el cliente manda un guion propio: devolvé un resumen breve, los prompts del avatar y de los escenarios, y después el guion con las [tomas] detalladas respetando su texto (solo se aplican las reglas fijas de la sección siguiente).

## Reglas fijas (ya corregidas por Maxi o el cliente)

- **Sin textos en pantalla en el guion:** nada de títulos, rótulos, subtítulos, cartelas ni "sellos". Eso va en CapCut.
- **Cambio de escenario:** describí el escenario nuevo completo dentro de la toma (lugar real, hora, luz, utilería, clima).
- **Avatares distintos por país:** al adaptar, otra cara, otro físico, otra ropa, otro nombre y otra ciudad. Nunca copiar el avatar de otro idioma. Excepción: si Maxi pide explícitamente "el mismo avatar".
- **No repetir ciudades** dentro de una misma tanda (ver `references/paises.md`).
- **Nunca mencionar cambios de talla.** Decir "pide tu talla de siempre".
- **CTA de cierre del cliente:** reemplazar "sayu.es" por "Te dejo el link a la tienda oficial" (y equivalentes por idioma).
- **Envío gratis:** confirmado en España e Italia. En Francia y Portugal, no ponerlo hasta que se confirme (avisar en una línea).
- **Temporada:** otoño, "ahora que llega el frío". Nada de Navidad.
- **Edad visible:** protagonistas de 55 a 65 con arrugas, canas y manchas reales.
- **Alturas explícitas** en cada toma donde se compare (quién es más alto, con referencias físicas).
- **Una sola zapatilla por plano** cuando hay varias marcas: Veo3 las mezcla. En comparaciones, los productos van tapados y se muestran de a uno.
- **No suavizar promesas del cliente** por criterio propio (salud o legales). Traducir fiel salvo que Maxi pida cambios.
- Cada frase hablada tiene que entrar en un clip de 8 s (18 a 20 palabras). Si es más larga, partirla en dos clips.
- Un solo personaje habla por clip; el otro, "con la boca cerrada".

## Qué referencia leer

| Necesito… | Leer |
|---|---|
| Datos de producto, colores, beneficios, qué decir y qué no | `references/productos.md` |
| Reglas de guion, embudo, retargeting, mecanismos del dolor | `references/reglas-guion.md` |
| Formato exacto del guion detallado, voz dentro del clip, tabla de Veo3 | `references/formato-entrega.md` |
| Plantillas de prompts (lookbook, keyframe, selfie, animados, radiografía, 3D, productos) | `references/prompts.md` |
| Vocabulario por idioma, ciudades ya usadas, concordancias, etiquetas de voz | `references/paises.md` |
| Biblioteca de títulos por idioma | `references/titulos.md` |
| Formatos y personajes ya producidos (para no repetir y reciclar) | `references/catalogo.md` |
| Plan actual de la tanda de 72 videos, códigos y pendientes | `references/plan-72.md` |
| Prompts de Veo3 directos (estructura del Manual Maestro, storyboard con QUICK HARD CUT, diálogo continuo, B-roll, checklist, diagnóstico de fallos) | `references/veo3-manual.md` |
| Nivel de detalle de avatares y qué masters/keyframes generar (BEFORE/AFTER, interacción, producto en mano) | `references/avatares-masters.md` |
| Ejemplo completo de guion con tomas muy detalladas (médico para personal sanitario) | `references/ejemplo-medico.md` |

## Ahorro de tokens

- No repitas reglas ni explicaciones que ya están acá: aplicalas.
- No vuelvas a pegar prompts de avatares o keyframes que ya se entregaron, salvo que Maxi los pida.
- En la adaptación a otro país, el guion se entrega completo, pero sin re-explicar el concepto.
- Las radiografías y animaciones ya generadas se reutilizan entre países (solo cambia el idioma de la voz).
