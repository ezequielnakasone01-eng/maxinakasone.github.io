# Guionado: concepto → guion limpio → guion con tomas → localización

El guion decide la idea, el diálogo, la arquitectura narrativa y la evidencia visual de cada frase. Los prompts solo automatizan lo que el guion ya resolvió: si el guion se contradice, el prompt automatiza una contradicción.

## Índice
1. Principios
2. Concepto
3. Arquitecturas narrativas
4. Guion limpio
5. Guion con tomas
6. Máquina de estados y altura
7. Localización
8. QA del guion
9. Caso completo: médico para personal sanitario

---

## 1. Principios

- **Una pieza = una idea central.** "Médico para personal sanitario", "mujer hablando del marido", "pedido de Carlos", "retargeting del carrito" son ideas. "Hablar de SAYU" no.
- **El copy vende; el B-roll demuestra.** altura → comparación corporal o mecanismo interno; espalda → pisada / amortiguación / final de turno; juanete → puntera / espacio / roce; stock → estanterías y pedidos saliendo.
- **La historia no tapa el producto.** En TOF o educativo se puede retrasar el nombre hasta la solución, pero sin perder demasiado tiempo antes del beneficio diferencial.
- **Retargeting va al hueso:** frases cortas, beneficio rápido, precio, envío, escasez, CTA. Menos historia.
- **Una sola persona habla por clip.** Pareja/entrevistador/extras: mudos en ese clip.
- **Temporada:** respetar la del archivo del cliente (SAYU: otoño, nada navideño).
- **No inventar operaciones comerciales.**

## 2. Concepto

Antes del copy, proponé el concepto. Si el usuario pide ideas, dá 3–5 conceptos distintos entre sí y distintos de los "ya producidos" del cliente, con una línea de por qué cada uno suma a la tanda.

```
CONCEPTO
Nombre del ángulo:
Público / funnel (TOF, MOF, retargeting):
Quién habla:
Locación:
Historia en 4–8 líneas:
Qué hace diferente esta pieza de las anteriores:
Beneficios que entran y en qué orden:
Oferta / CTA:
Riesgo principal de producción:
```

## 3. Arquitecturas narrativas

- **Autoridad / médico:** hook al oficio → altura invisible → por qué importa en la jornada → espalda → juanete → recomendación a la categoría → oferta → escasez → CTA.
- **Pareja:** hook de relación → comparación de altura → reacción de la pareja → espalda/comodidad → juanete → producto → oferta/CTA.
- **Retargeting:** "ya las viste / carrito" → beneficio principal → objeción → precio/envío → stock → CTA directo.
- **Fundador:** legitimidad / pedido real / demostración física → beneficios → stock/fulfilment → oferta → CTA.
- **Animación:** personaje o mecanismo introduce el problema → explicación visual difícil de filmar → solución → oferta → CTA. Física coherente; nunca catálogo 3D.
- **Educativo:** problema cotidiano → explicación → recién en la solución se nombra la marca → prueba visual → CTA suave o cierre de oferta según funnel.
- **Testimonial casero:** pregunta/hook a cámara → legitimidad (segundo par, uso diario) → historia BEFORE → cambio de experiencia → demo de producto → transformación + cierre.

## 4. Guion limpio

Solo lo que el espectador escucha. Sin tomas, sin cámara, sin prompts. Se aprueba venta, ritmo, lenguaje, promesas, orden de beneficios y CTA.

```
GUION LIMPIO
HABLANTE: «Frase 1.»
HABLANTE: «Frase 2.»
...
```

Reglas:
- Escribir para ser dicho: frases cortas o medianas, respiraciones naturales, nada de párrafos que obliguen a recitar rápido.
- Registro del mercado (España: "tú").
- Cada frase tiene una función: hook, beneficio, evidencia, objeción, oferta, escasez o CTA.
- Precio y oferta inequívocos cuando el concepto los incluye.
- CTA acorde al funnel (agresivo en retargeting, natural en autoridad/educativo).
- **Ritmo Veo3:** clip hablado ≈ 8 s ≈ 18–20 palabras (animación ≈ 10 s). Indicá al final el recuento total de palabras y cuántos clips salen.
- Números, precios, medidas y marca escritos de forma fácil de pronunciar y siempre igual.

## 5. Guion con tomas

Se conserva el diálogo aprobado **intacto** y debajo de cada frase (o grupo corto) va la toma que prueba exactamente esa idea. No es todavía un prompt: es una hoja de dirección con detalle suficiente para que la etapa de generación no invente la intención.

```
HABLANTE: «Frase exacta.»
[TOMA X (N s): lugar + hora/luz + personaje + vestuario + producto + encuadre + acción física de inicio a fin + fondo vivo + estado BEFORE/AFTER + cómo termina + función visual.]
```

Campos de cada TOMA:

| Campo | Qué fija |
|---|---|
| Duración | 2–4 s la mayoría; más si la acción es compleja |
| Lugar exacto | hospital, control de enfermería, cocina, tienda, calle localizada… |
| Hora y luz | mañana gris, fluorescente, otoño cálido… |
| Personaje | edad visible, sexo, oficio, identidad/avatar |
| Vestuario | prendas, uniforme, abrigo, accesorios |
| Producto | modelo/color exacto; puesto, en mano, apoyado, en caja |
| Estado | BEFORE / transición / AFTER |
| Acción física | qué mano hace qué, de dónde parte, qué toca, cómo termina |
| Cámara | plano entero, detalle, cenital, ras de suelo, eye-level; móvil en mano/trípode |
| Movimiento | quieto, dos pasos, cambia peso, gira, presiona malla… |
| Fondo vivo | gente pasando, carros, tráfico; nadie identificable ni mirando a cámara |
| Final | dónde queda todo, sin pose congelada |
| Función | qué prueba: altura, presión, amortiguación, stock, pareja, oferta |

Pobre: `[B-roll: enfermero caminando por el hospital.]`
Operativo: `[TOMA (3 s): plano muy bajo, a 15–20 cm del suelo, en un pasillo real de hospital español con suelo vinílico gris y luz blanca de techo. Enfermero de 52 años, uniforme azul marino y SAYU blancas idénticas al ingrediente, entra ya caminando desde el fondo. Cámara fija a un lado como si un compañero hubiese dejado el móvil a ras del suelo; registra dos pasos completos: talón derecho toca, la suela cede mínimamente, el pie rueda y despega. Al fondo dos sanitarios desenfocados con carpetas; nadie mira a cámara. Termina con el pie izquierdo empezando el siguiente paso, no posado.]`

Regla de decisión rápida (qué plano según la frase):
- Personal / credibilidad / objeción → rostro medio-corto.
- Dolor o incomodidad → acción humana sutil (mano en lumbar al caminar), nunca gráfico médico ni actuación dramática.
- Material / forma / horma → producto físico en close-up, en mano o en pie.
- Pisada / amortiguación → plano bajo 3/4 de un paso completo.
- Postura / altura → plano entero a nivel de ojos.
- Compra / segundo par → prop real (caja ya abierta).
- Stock / escasez → estantería con huecos irregulares (sin rótulos generados).
- Oferta / CTA → vuelta al rostro, contexto conservado, espacio limpio para gráficos.

Marcado práctico: en una copia de trabajo podés etiquetar cada frase con [FACE], [B-ROLL], [PRODUCT], [FULL BODY], [PROP], [OFF-CAMERA] y luego convertir cada etiqueta en una TOMA.

## 6. Máquina de estados y altura

```
STATE A — BEFORE: calzado viejo/convencional, altura natural, postura más cerrada, molestias sutiles, luz algo más fría si hay contraste.
STATE B — TRANSICIÓN: el producto aparece de forma físicamente explicable (caja ya abierta, tienda, médico, compra). Todavía no asumir resultado.
STATE C — AFTER: producto puesto, alza interna, misma anatomía, postura apenas más erguida, movimiento cómodo, luz más cálida si se usa contraste.
STATE D — OFERTA/CTA: precio, envío, garantía, stock, acción. Sin teletienda.
```

Altura:
- Con pareja en tacones: BEFORE ella igual o más alta (según storyboard). AFTER él claramente más alto, con referencias corporales ("ella le llega a los ojos / a la barbilla").
- Nunca estirar piernas, engrosar la suela ni usar contrapicado. Se percibe por silueta + relación con el entorno + cámara a nivel de ojos.

## 7. Localización

Localizar ≠ traducir. Se conserva: concepto, hook funcional, orden de beneficios, arco BEFORE/AFTER, función de cada toma, oferta aprobada (salvo precio/condición por mercado). Se localiza: ciudad/barrio/arquitectura, nombres propios (Carlos → Carlo), expresiones y ritmo del idioma, comidas, objetos domésticos, vestuario/uniformes, moneda y formato numérico, unidades (EE. UU. en pulgadas), terminología anatómica y de talla (tabla en el archivo del cliente), línea de idioma de Veo3.

Ejemplo: un guion español con Gran Vía / Retiro en Italia pasa a Milán, Bérgamo o Nápoles, con casa, café, objetos y vestuario italianos. La función ("hombre de 55 demuestra altura caminando con SAYU") se mantiene.

Entregá la versión localizada como guion limpio + guion con tomas, y marcá en una lista breve qué cambiaste del mundo (no solo del texto).

## 8. QA del guion

- ¿El concepto agrega algo nuevo a la tanda?
- ¿El hook habla al público correcto?
- ¿Si aparecen los tres beneficios, altura va primero?
- ¿Suena hablado y no redactado? ¿Cada frase tiene función?
- ¿Cada TOMA prueba exactamente su frase y tiene lugar, luz, personaje, vestuario, producto, acción y cámara claros?
- ¿Cada acción puede ocurrir de verdad? ¿Está claro BEFORE / transición / AFTER?
- ¿La pareja conserva la relación de alturas?
- ¿El producto se describe idéntico al ingrediente?
- ¿Nada de operaciones inventadas? ¿Temporada correcta (otoño, no Navidad)?
- ¿Precio / envío / garantía correctos? ¿CTA acorde al funnel?
- ¿La adaptación está localizada y no solo traducida?

## 9. Caso completo: médico para personal sanitario (referencia de calidad)

**Concepto:** médico español de 55–60 años en un hospital real. Habla a médicos, enfermeros, auxiliares, celadores y a quien pasa guardias largas de pie. Abre con los +10 cm internos y gira hacia lo que importa en el turno: reparto de carga, amortiguación, puntera ancha. El producto aparece como solución en la explicación, no como teletienda. El personal sanitario adicional solo aparece en B-roll y no habla.

**Guion limpio:**
«Si trabajas en un hospital y pasas ocho, diez o doce horas de pie, mira esto. Estas zapatillas te dan diez centímetros más de altura por dentro, sin que nadie vea el alza. Pero si haces guardias, eso no es lo más importante. La plantilla anatómica reparte el peso por todo el pie y la suela amortigua cada paso antes de que toda esa carga termine en tu espalda. Y delante tienen una puntera más ancha, para que el juanete tenga espacio y deje de rozar durante todo el turno. Son las SAYU. Por eso se las recomiendo especialmente a médicos, enfermeros, auxiliares y a cualquiera que pase el día de pie. Ahora están a 59,95 euros, con envío gratis y treinta días para probarlas en casa. Con el frío quedan pocas de este lote. Dale al link y pídelas ahora.»

**Guion con tomas (extracto representativo):**

MÉDICO: «Si trabajas en un hospital y pasas ocho, diez o doce horas de pie, mira esto.»
[TOMA 1 (4 s): hospital español moderno pero real, no set ni clínica de lujo. Pasillo ancho junto a un control de enfermería, paredes blanco roto, puertas gris claro, suelo vinílico gris azulado con marcas mínimas de uso, paneles de luz blanca. Médico de 57 años, idéntico al avatar definitivo, pelo corto canoso con entradas reales, piel de su edad con poros y líneas de expresión, bata blanca abierta sobre pijama azul marino y zapatillas neutras sin protagonismo. Plano medio fijo a la altura de los ojos, como móvil en trípode a 1,5–1,8 m, médico ligeramente desplazado para dar profundidad al pasillo. Habla a cámara sin sonrisa publicitaria; en "ocho, diez o doce horas" una mano abierta con tres pequeños pulsos naturales, sin contar con los dedos. Detrás pasan desenfocados una enfermera con carpeta y un auxiliar con un carro pequeño, sin mirar a cámara. En "mira esto" baja brevemente la mirada al suelo y vuelve al objetivo. Termina con la mano volviendo junto a la bata, no congelada.]

MÉDICO: «Estas zapatillas te dan diez centímetros más de altura por dentro, sin que nadie vea el alza.»
[TOMA 2 (3 s): plano muy bajo, 15–20 cm del suelo, mismo hospital. Enfermero de 52 años, uniforme azul marino, SAYU blancas idénticas al ingrediente. Cámara fija al borde del pasillo, 3/4 frontal. Entra ya caminando desde 2–3 m; dos pasos completos a velocidad normal. El pantalón cae limpio sobre el cuello de la zapatilla; la silueta no delata plataforma. Al fondo otro sanitario cruza y una puerta automática queda abierta. Termina avanzando, no posando. TOMA 3 (2 s, inserto educativo): vista lateral de un pie real dentro de la SAYU sobre el mismo suelo; tratamiento de radiografía limpio, huesos en cian, estructura de elevación en amarillo cálido completamente dentro de la geometría exterior, que no cambia. Espacio para "+10 CM" en CapCut. TOMA 4 (2 s): plano entero a nivel de ojos del mismo enfermero junto a una pared con líneas verticales y puerta estándar; se acomoda el bolsillo y retoma la marcha. La altura se percibe por la silueta.]

MÉDICO: «La plantilla anatómica reparte el peso por todo el pie...»
[TOMA 6 (3 s): detalle 3/4 desde arriba de una pierna y pie del enfermero sobre el vinílico, como B-roll de móvil de un compañero. Transfiere peso gradualmente: talón → mediopié → antepié. Como único recurso educativo, una distribución de presión muy sutil azul/verde se extiende uniforme por la base; nada grotesco ni flotante. La zapatilla mantiene forma y escala. Termina cuando el peso empieza a pasar al otro pie.]

MÉDICO: «Y delante tienen una puntera más ancha, para que el juanete tenga espacio y deje de rozar durante todo el turno.»
[TOMA 9 (4 s): zona de descanso del personal. El enfermero sentado en un banco, SAYU puesta en el pie derecho. Plano muy cerrado de puntera y lateral medial del antepié, cámara a la altura del zapato. La mano baja desde la rodilla, el pulgar presiona una vez la malla donde estaría el juanete; cede unos milímetros y recupera la forma. El pie sigue dentro para que se vea espacio real. Dos dedos recorren el borde de la puntera sin estirarla y la mano vuelve a la rodilla. Piel y uñas naturales.]

MÉDICO: «Son las SAYU.»
[TOMA 10 (2 s): vuelta al médico en el control. Sobre el mostrador, desde el inicio de la toma, una única SAYU blanca apoyada. Mano en el talón y otra cerca del antepié, la levanta 10–15 cm, cambia unos grados el ángulo de muñeca para mostrar malla, cordones, suela blanca e inserto negro, y la vuelve a acercar al mostrador. Sin giro 360° ni acercarla al lente.]

MÉDICO: «Con el frío quedan pocas de este lote.»
[TOMA 13 (2,5 s): almacén realista de SAYU sin personas hablando. Estantería metálica con cajas negras y huecos irregulares; aún hay stock. Una mano entra desde la derecha, agarra una caja por el lateral, encuentra resistencia con la de al lado, reajusta el agarre, la saca y deja el hueco visible. Sin rótulos generados.]

MÉDICO: «Dale al link y pídelas ahora.»
[TOMA 14 (2,5 s): plano final del médico, mismo lugar y vestuario, SAYU apoyada en el mostrador. Mira a cámara, una indicación corta hacia abajo con el índice en "link", retira la mano, pequeño asentimiento en "pídelas ahora" y gira el torso unos grados hacia el control como si volviera al trabajo. Corte seco.]

**Notas de producción:** solo habla el médico; hospital real sin escenas clínicas sensibles ni pacientes identificables; producto idéntico al ingrediente; "+10 CM", "59,95 €", "ENVÍO GRATIS", "30 DÍAS" en CapCut; el médico parece alguien que trabaja allí, no un médico de TV.
