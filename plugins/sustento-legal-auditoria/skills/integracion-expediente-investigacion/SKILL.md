---
name: integracion-expediente-investigacion
description: Revisa y ordena la integración del expediente de investigación de responsabilidades administrativas derivado de auditoría, desde el acuerdo de inicio hasta la conclusión. Úsala cuando el usuario hable de integrar, revisar, depurar o auditar un expediente de investigación, pregunte qué constancias le faltan, cómo ordenar o foliar el expediente, qué diligencias practicar, cómo documentar la cadena hallazgo-observación-expediente, o cuando prepare la entrega del expediente a la autoridad substanciadora. Aplica a contralorías municipales, órganos internos de control y áreas de responsabilidades del ámbito estatal del Estado de México.
---

# Integración del expediente de investigación

El expediente es donde se gana o se pierde el asunto. Una investigación bien
hecha pero mal documentada es indefendible: la autoridad substanciadora, el
Tribunal y eventualmente el juez de amparo sólo conocen lo que consta en
actuaciones. Lo que el investigador sabe pero no asentó, no existe.

Lee `${CLAUDE_PLUGIN_ROOT}/references/concordancia-lraemym-lgra.md` para el
articulado. En el Edoméx la investigación se rige por los artículos 94 a 103
LRAEMyM y la calificación por los artículos 104 y 105.

## La cadena que debe quedar documentada

El expediente tiene que permitir reconstruir, sin preguntarle nada a nadie, el
camino completo:

**Fuente** (informe de resultados del OSFEM, pliego de observaciones, denuncia,
auditoría interna, vista de otra autoridad) → **acuerdo de inicio** →
**diligencias de investigación** → **conclusión** (IPRA o acuerdo de conclusión
y archivo) → **calificación notificada**.

Cada eslabón debe tener su constancia con fecha, firma y fundamento. Si un
eslabón falta, el siguiente queda sin apoyo.

## Estructura mínima del expediente

Revisa que existan y estén en orden cronológico y foliados:

**Apertura**
- Documento fuente que originó la investigación, en original o copia certificada
- Acuerdo de inicio o de radicación, con número de expediente, fundamento de la
  competencia de la autoridad investigadora y descripción del hecho
- Constancia de asignación al investigador
- En su caso, ratificación de la denuncia

**Competencia y atribuciones**
- Constancia del nombramiento del titular del órgano investigador y del
  fundamento de su competencia
- Documentación que acredita el nexo de atribución del presunto responsable:
  nombramiento, alta, reglamento interior, manual de organización, acuerdo de
  cabildo, oficio de comisión

**Diligencias**
- Oficios de requerimiento de información, con acuse de recibo
- Respuestas recibidas, completas y con sus anexos
- Actas circunstanciadas de las diligencias practicadas: inspecciones,
  verificaciones físicas, entrevistas
- Acuerdos que ordenan cada diligencia y acuerdos que tienen por recibida la
  información
- Constancias de las diligencias que no pudieron practicarse y por qué

**Pruebas**
- Documentos identificados por tipo, número, fecha y foja
- Certificación de las copias, o razón de cotejo contra el original
- Cadena documental: de dónde salió cada documento y quién lo entregó
- Dictámenes técnicos o periciales, con el acuerdo que los ordenó y la
  acreditación de quien los emite

**Cuantificación**
- Papeles de trabajo de la cuantificación del daño, con método y fuentes
- Documentos que soportan cada cifra

**Cierre**
- Acuerdo de conclusión de la investigación
- Acuerdo de calificación de la falta, fundado y motivado (artículos 104 y 105)
- IPRA, o acuerdo de conclusión y archivo por falta de elementos
- Constancias de notificación de la calificación

## Errores estructurales frecuentes

- **Expediente sin acuerdo de inicio**, que arranca directamente con oficios de
  requerimiento. Toda actuación posterior queda sin fundamento.
- **Requerimientos sin acuse.** No se puede acreditar que el ente fue requerido.
- **Diligencias sin acuerdo previo que las ordene.** Rompe la formalidad de las
  actuaciones.
- **Documentos sueltos sin foliar** o incorporados fuera de orden cronológico.
- **Confusión de roles.** La misma unidad que investigó aparece substanciando.
  Verifica la separación funcional y que conste documentalmente.
- **Datos personales sin protección.** El expediente contiene datos de terceros:
  verifica versiones públicas y el tratamiento conforme a la normatividad de
  protección de datos.
- **Investigación que se detiene en el ente y no llega a la persona.** Se
  requiere al ayuntamiento, el ayuntamiento contesta, y nunca se identifica al
  servidor público que desplegó la conducta.
- **Prescripción corriendo sin control.** Debe haber un control de plazos
  visible en el expediente, no en la cabeza del investigador.
- **Cuantificación sin papel de trabajo.** El monto aparece en el IPRA pero no
  hay cómo reproducirlo.

## Formato de salida

```
# Revisión de integración del expediente
Expediente: [número]  Ente auditado: [nombre]  Ejercicio: [año]
Autoridad investigadora: [ ]

## 1. Estado general
[INTEGRADO / INTEGRADO CON OBSERVACIONES / NO APTO PARA CONCLUIR]
[Dos o tres líneas.]

## 2. Checklist de constancias
| Bloque | Constancia | ¿Obra en autos? | Foja | Observación |
|--------|-----------|------------------|------|-------------|
[Todos los bloques de la estructura mínima.]

## 3. Cadena documental
[Reconstrucción del camino fuente → inicio → diligencias → conclusión, señalando
los eslabones rotos.]

## 4. Riesgos procesales
[Cada defecto con su consecuencia concreta: nulidad, desechamiento del IPRA,
absolución, procedencia de amparo.]

## 5. Control de prescripción
| Conducta | Fecha de comisión | Calificación | Plazo | Fecha límite | Días restantes |

## 6. Diligencias pendientes, en orden de urgencia
[Qué hacer, con qué fundamento y qué documento debe quedar en el expediente.]
```

## Criterio de trabajo

Prioriza por consecuencia, no por facilidad: un requerimiento sin acuse y una
foja mal numerada no pesan igual. Cuando detectes un defecto que ya no puede
subsanarse —una prueba obtenida sin acuerdo previo, un plazo vencido— dilo
claramente en lugar de sugerir un remiendo que después será señalado como
irregularidad adicional.

Nunca propongas fechar, foliar o documentar una actuación como si se hubiera
practicado en un momento distinto al real. Si una diligencia se omitió, la
salida es practicarla ahora dejando constancia de la fecha real, o asumir su
ausencia.
