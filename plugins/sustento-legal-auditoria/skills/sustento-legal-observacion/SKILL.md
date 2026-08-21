---
name: sustento-legal-observacion
description: Revisa y refuerza el sustento legal de una observación de auditoría gubernamental para que resista su traslado al procedimiento de investigación de responsabilidades administrativas. Úsala siempre que el usuario comparta una observación, hallazgo, cédula de observaciones, pliego de observaciones, resultado de auditoría o informe de resultados y pregunte si "está bien fundada", "tiene sustento", "aguanta", "sirve para responsabilidades" o "cómo la redacto"; también cuando pida revisar fundamentación, encuadre normativo, nexo causal o cuantificación de daño en materia de fiscalización estatal o municipal del Estado de México, aunque no mencione la LRAEMyM ni la LGRA por su nombre.
---

# Sustento legal de observaciones de auditoría

Una observación de auditoría y una imputación de responsabilidad administrativa
son documentos distintos con estándares distintos. La observación nace de una
técnica de auditoría; la imputación tiene que sostener una acusación contra una
persona concreta ante una autoridad resolutora, con presunción de inocencia de
por medio. La mayoría de las observaciones que se caen no se caen porque el
hallazgo sea falso, sino porque nunca se redactaron pensando en ese segundo
estándar.

Tu trabajo aquí es cerrar esa brecha: tomar la observación tal como está y
decir, sin adornos, si puede sostener un Informe de Presunta Responsabilidad
Administrativa (IPRA) y qué le falta.

## Antes de empezar

Lee `${CLAUDE_PLUGIN_ROOT}/references/concordancia-lraemym-lgra.md`. Contiene el
mapa de articulado y las normas sustantivas que suelen ser la norma infringida.
Nunca cites un precepto de memoria: el articulado estatal y el federal no
coinciden.

Si el usuario no lo dijo, pregunta una sola cosa antes de trabajar: **el ámbito
y el origen del recurso** (ayuntamiento, organismo descentralizado, dependencia
estatal; recurso propio, estatal o federal). Determina la ley aplicable y la
autoridad competente, y sin eso cualquier fundamentación es provisional. Todo lo
demás dedúcelo del documento o márcalo como pendiente en la cédula.

## Los ocho elementos

Toda observación destinada a responsabilidades debe poder responder estas ocho
preguntas. Revísalas en orden; los primeros defectos suelen explicar los demás.

1. **¿Qué conducta se describe?** Un acto u omisión concreto, con circunstancias
   de modo, tiempo y lugar. Un saldo, una diferencia o un faltante no son
   conductas: son resultados. Alguien tuvo que hacer u omitir algo para
   producirlos.
2. **¿Quién la desplegó?** Servidor público identificado por nombre, cargo y
   periodo de gestión. Si la observación se dirige contra "el ente", "la
   administración" o "el área", no hay sujeto imputable.
3. **¿Por qué le era exigible?** El nexo de atribución: el precepto, manual de
   organización, reglamento interior, acuerdo de cabildo o nombramiento que le
   asignaba esa función. Sin esto, aun con la conducta probada, no hay deber
   incumplido.
4. **¿Qué norma sustantiva se infringió?** Precepto específico con artículo,
   fracción e inciso. "La normatividad aplicable" no es fundamento; es una
   confesión de que no se identificó la norma.
5. **¿Qué precepto de la LRAEMyM la tipifica?** La segunda capa. El
   incumplimiento sustantivo tiene que encuadrar en el artículo 50 o 51
   (no graves) o en alguno de los 53 al 67 (graves).
6. **¿Con qué se prueba?** Documento identificado por tipo, número, fecha y foja
   del expediente. Indica si obra en original, copia certificada o simple, y
   quién lo proporcionó. Una prueba que no se puede localizar en el expediente
   no existe para efectos del procedimiento.
7. **¿Cuál es el nexo causal?** La cadena explícita entre la conducta y la
   transgresión, y en su caso entre la conducta y el daño. Que dos hechos
   aparezcan en el mismo párrafo no los vincula.
8. **¿Hay daño o perjuicio, y cómo se cuantificó?** Monto, método de
   cuantificación y fuente de cada cifra. Distingue daño patrimonial real de
   irregularidad formal: no toda falta produce daño, y afirmar un daño que no se
   puede cuantificar debilita todo lo demás.

Añade siempre una novena verificación: **temporalidad**. Fecha de comisión de la
conducta y cómputo de prescripción conforme al artículo 78 LRAEMyM (3 años no
graves, 7 años graves). Una observación impecable fuera de plazo no sirve.

## Vicios que tumban observaciones

Búscalos activamente; son los que más aparecen en la práctica.

- **Observación sin sujeto.** Redactada contra el ente. No puede convertirse en
  IPRA sin rehacerse.
- **Fundamento genérico.** Cita de una ley completa, de un capítulo, o la
  fórmula "y demás disposiciones aplicables".
- **Confusión entre debilidad de control interno y falta administrativa.** Que
  un procedimiento no esté documentado es una recomendación, no necesariamente
  una conducta imputable. Sepáralas.
- **Recomendación disfrazada de observación.** Si la conclusión es "deberá
  implementar", no hay imputación.
- **Salto de la irregularidad al daño.** Se detecta un incumplimiento formal y
  se le asigna un monto igual al total de la operación, sin demostrar que el
  recurso se perdió o se aplicó indebidamente.
- **Prueba no idónea.** Copias simples sin certificar, papeles de trabajo del
  propio auditor usados como prueba del hecho, o documentos sin firma ni sello
  de recepción.
- **Encuadre por el nombre y no por los elementos.** Llamar "desvío" a lo que
  materialmente es un daño culposo del artículo 51, o al revés. Esto no es un
  detalle de estilo: define la competencia y el plazo de prescripción.
- **Pluralidad de conductas en una sola observación.** Si hay tres conductas,
  tres sujetos y tres normas, hay tres imputaciones. Fusionarlas obliga a la
  autoridad resolutora a desglosar o a absolver en bloque.
- **Cita al articulado equivocado.** Federal en asunto estatal o viceversa.

## Formato de salida

Entrega siempre una **cédula de análisis de sustento legal** con esta
estructura:

```
# Cédula de análisis de sustento legal
Observación: [número / identificación]  Ejercicio: [año]  Ente: [nombre]
Ámbito y ley aplicable: [LRAEMyM / LGRA / concurrente]

## 1. Veredicto
[Una de tres: SOSTIENE IPRA / SOSTIENE CON CORRECCIONES / NO SOSTIENE]
[Dos o tres líneas explicando por qué.]

## 2. Verificación de elementos
| # | Elemento | Estado | Qué dice la observación | Qué falta |
|---|----------|--------|--------------------------|-----------|
[Estado: Cumple / Parcial / Ausente. Una fila por cada uno de los ocho elementos
más temporalidad.]

## 3. Encuadre normativo propuesto
- Norma sustantiva infringida: [artículo, fracción, inciso, ordenamiento]
- Precepto que tipifica la falta: [artículo LRAEMyM]
- Calificación preliminar: [grave / no grave] — [razón en una línea]
- Autoridad resolutora que correspondería: [OIC-Contraloría / TRIJAEM]
- Prescripción: [plazo, fecha de inicio del cómputo, fecha límite]

## 4. Vicios detectados
[Lista. Para cada uno: en qué parte del texto está y qué consecuencia procesal
tiene. Si no hay vicios, dilo.]

## 5. Redacción sugerida
[La observación reescrita con los ocho elementos explícitos. Marca entre
corchetes cada dato que el usuario debe completar del expediente: [nombre],
[foja], [monto].]

## 6. Diligencias pendientes
[Qué se necesita recabar antes de que esto pueda sustentar un IPRA.]
```

## Cómo escribir el veredicto

Sé directo. Si la observación no sostiene una imputación, dilo en la primera
línea y explica por qué; suavizarlo le cuesta tiempo al usuario y le cuesta el
asunto al órgano de control. Igualmente, si la observación está bien construida,
dilo sin inventar objeciones de relleno.

Cuando un dato no esté en lo que te compartieron, no lo supongas: márcalo entre
corchetes como pendiente. Un nombre inventado, una foja inventada o un artículo
inventado en un documento que va al expediente es un problema mucho más grave
que un espacio en blanco.

## Advertencia de alcance

Este análisis es apoyo técnico para el trabajo del área de auditoría o del
órgano de control; no sustituye la valoración jurídica de la autoridad
investigadora ni la determinación de la substanciadora o resolutora. Dilo una
vez, al final, en una línea. No lo repitas en cada sección.
