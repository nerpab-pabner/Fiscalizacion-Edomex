---
name: calificacion-falta-administrativa
description: Encuadra una conducta detectada en auditoría dentro del catálogo de faltas administrativas y la califica como grave o no grave, con el precepto exacto, la competencia resultante y el plazo de prescripción. Úsala cuando el usuario pregunte si una conducta "es grave o no grave", "en qué artículo encuadra", "es peculado o desvío", "va al Tribunal o lo resuelve el OIC", cuando pida calificar una falta, elaborar el acuerdo de calificación, o cuando dude entre daño culposo y falta grave. También aplica a faltas de particulares vinculados con faltas graves (proveedores, contratistas, ex servidores públicos).
---

# Calificación de faltas administrativas

La calificación no es una etiqueta: define quién resuelve, qué plazo de
prescripción corre, qué sanciones proceden y qué medio de defensa tiene el
presunto responsable. Calificar mal es la forma más rápida de perder un asunto
que estaba bien investigado.

Lee `${CLAUDE_PLUGIN_ROOT}/references/concordancia-lraemym-lgra.md` antes de
citar cualquier precepto.

## El orden correcto de razonamiento

Se califica desde los **elementos de la conducta**, nunca desde el nombre que se
le dio en la auditoría. Que la cédula diga "desvío de recursos" no significa que
encuadre en el artículo 55 LRAEMyM. Procede así:

1. **Aísla la conducta.** Un acto u omisión, un sujeto. Si hay varios, califica
   cada uno por separado; pueden tener calificaciones distintas.
2. **Determina el elemento subjetivo.** ¿La conducta fue dolosa —el servidor
   público quiso el resultado o lo aceptó— o culposa/negligente? Esta es la
   bifurcación principal y casi siempre la más discutida.
3. **Recorre el catálogo de graves (artículos 53 a 67 LRAEMyM).** Verifica los
   elementos típicos de cada figura candidata, uno por uno. Si falta un
   elemento, la figura no aplica, por más que el hecho suene parecido.
4. **Si ninguna figura grave se integra**, revisa el artículo 50 (catálogo de
   obligaciones) y el artículo 51 (daños y perjuicios culposos o negligentes a
   la Hacienda Pública).
5. **Deriva las consecuencias**: competencia, sanciones aplicables,
   prescripción, medio de impugnación.

## Las confusiones que importan

**Peculado (54) vs. desvío de recursos públicos (55).** El peculado supone
apropiación o uso para fines ajenos al servicio, en beneficio propio o de un
tercero, de recursos que se tenían bajo administración o custodia. El desvío
supone autorizar, solicitar o realizar actos para que recursos públicos se
apliquen a **fines distintos** a los autorizados por norma, contrato o
presupuesto. No se necesita apropiación para que haya desvío; se necesita cambio
de destino. Cuando el recurso se ejerció en un objeto público pero distinto al
etiquetado, la figura suele ser desvío, no peculado.

**Daño culposo (51) vs. falta grave.** Esta es la línea divisoria de la
competencia. El artículo 51 exige daño o perjuicio causado de manera culposa o
negligente **y sin que se integre alguna falta grave**. Si el hallazgo es un
error de aplicación, una omisión de supervisión o una decisión torpe sin
propósito ilícito acreditable, la calificación honesta es no grave, aunque el
monto sea alto. El monto no agrava la falta; los elementos sí.

**Abuso de funciones (58) como cajón de sastre.** Se invoca cuando no se logró
integrar otra figura. Exige que el servidor público ejerza atribuciones que no
tiene, o que las ejerza para causar un perjuicio o generar un beneficio
indebido. Si lo que hay es un incumplimiento de procedimiento, revisa primero el
artículo 50.

**Contratación indebida (62).** Aplica cuando se autoriza contratar a quien
está impedido: inhabilitado, en conflicto de interés, o en los demás supuestos
del precepto. No cubre cualquier irregularidad del procedimiento de contratación
—adjudicación directa mal fundada, fraccionamiento, falta de investigación de
mercado—; esas suelen encuadrar en el artículo 50 en relación con la Ley de
Contratación Pública del Estado de México y Municipios.

**Faltas de particulares.** Proveedores, contratistas y ex servidores públicos
sólo responden por los supuestos de los artículos 68 a 77, y siempre vinculados
a una falta grave. No existe la "falta no grave de particular". Si no se acredita
la falta grave del servidor público con la que se vincula, la imputación al
particular se queda sin base.

## Consecuencias de la calificación

| | No grave | Grave |
| --- | --- | --- |
| Preceptos | 50 y 51 LRAEMyM | 53 a 67 LRAEMyM |
| Resuelve | Contraloría / OIC / contraloría municipal | Tribunal de Justicia Administrativa del Estado de México |
| Sanciones | Artículos 79 a 81 | Artículos 82 a 84 |
| Prescripción (art. 78) | 3 años | 7 años |
| Impugnación de la calificación | Sí, artículos 106 a 114 | — |

Ese último renglón merece atención: la calificación de **no grave** es
impugnable por el denunciante. Si vas a calificar como no grave una conducta que
razonablemente podría ser grave, deja constancia expresa del razonamiento en el
acuerdo; ahí es donde se defiende la decisión.

## Formato de salida

```
# Acuerdo de calificación — análisis
Conducta analizada: [descripción en una oración]
Servidor público / particular: [nombre y cargo]
Fecha o periodo de comisión: [fecha]

## 1. Calificación
[GRAVE / NO GRAVE / NO CONSTITUYE FALTA ADMINISTRATIVA]
Precepto: [artículo, fracción LRAEMyM]

## 2. Elementos típicos y su acreditación
| Elemento del tipo | ¿Se acredita? | Medio de prueba en el expediente |
|-------------------|---------------|----------------------------------|
[Una fila por cada elemento de la figura elegida.]

## 3. Figuras descartadas y por qué
[Las que se consideraron y el elemento que falta en cada una. Esta sección es la
que sostiene el acuerdo frente a una impugnación: no la omitas.]

## 4. Elemento subjetivo
[Dolo o culpa, y en qué se apoya la conclusión.]

## 5. Consecuencias
- Autoridad resolutora competente: [ ]
- Sanciones aplicables: [artículos]
- Prescripción: [plazo, inicio del cómputo, fecha límite]
- Impugnabilidad de esta calificación: [ ]

## 6. Si es falta de particular
- Falta grave del servidor público con la que se vincula: [ ]
- Supuesto aplicable: [artículo 68 a 77]
```

## Criterio de honestidad técnica

No inflar ni desinflar. Calificar como grave una conducta que no integra los
elementos genera una imputación que el Tribunal desechará y desgasta la
credibilidad del órgano de control. Calificar como no grave una conducta que sí
los integra deja impune un hecho y expone a quien firmó el acuerdo. Cuando los
elementos estén genuinamente en duda, dilo así —"no se acredita con lo que obra
en el expediente"— e indica qué diligencia lo resolvería, en lugar de forzar la
calificación en cualquiera de las dos direcciones.

Cierra con una línea recordando que la calificación definitiva corresponde a la
autoridad investigadora en el acuerdo respectivo.
