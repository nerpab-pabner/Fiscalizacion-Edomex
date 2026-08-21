# Marketplace: fiscalizacion-edomex

Marketplace privado con el plugin **sustento-legal-auditoria**, para revisar el
sustento legal de observaciones de auditoría gubernamental y prepararlas para el
procedimiento de investigación de responsabilidades administrativas en el Estado
de México.

## Qué contiene el plugin

Cuatro skills que cubren la cadena completa observación → expediente → IPRA:

| Skill | Para qué |
| --- | --- |
| `sustento-legal-observacion` | Revisa si una observación resiste convertirse en imputación: ocho elementos, vicios frecuentes, encuadre y redacción sugerida |
| `calificacion-falta-administrativa` | Encuadra la conducta y la califica como grave o no grave, con precepto, competencia y prescripción |
| `integracion-expediente-investigacion` | Checklist de constancias del expediente, cadena documental y riesgos procesales |
| `informe-presunta-responsabilidad` | Estructura y verifica el IPRA conforme a los artículos 180 y 181 LRAEMyM |

Más un archivo de referencia compartido, `references/concordancia-lraemym-lgra.md`,
con el mapa de articulado LRAEMyM ↔ LGRA, autoridades competentes, normas
sustantivas habituales y plazos de prescripción.

## Instalación

### En el chat de Claude (web o app de escritorio)

1. Sube este repositorio a GitHub (puede ser privado si tu cuenta tiene acceso).
2. En Claude, abre el menú **Customize** → pestaña **Plugins**.
3. En **Personal plugins**, pulsa **+** → **Add marketplace** e indica el
   repositorio.
4. Instala `sustento-legal-auditoria` desde el marketplace recién agregado.

### En Claude Code

```
/plugin marketplace add <usuario-o-org>/<nombre-del-repo>
/plugin install sustento-legal-auditoria@fiscalizacion-edomex
```

## Mantenimiento

El valor de esto depende de que el articulado esté vigente. Dos hábitos:

- **Al inicio de cada ejercicio**, contrasta
  `references/concordancia-lraemym-lgra.md` contra el texto publicado en el
  Periódico Oficial "Gaceta del Gobierno" y en el DOF. La referencia se elaboró
  con la LRAEMyM reformada el 5 de abril de 2024 y la LGRA con reformas del
  2 de enero y el 15 de diciembre de 2025.
- **Cuando un asunto se caiga**, agrega el motivo a la sección de vicios de la
  skill correspondiente. Esa es la parte que ninguna ley te va a dar y la que
  hace que el plugin valga más que un manual.

## Para adaptarlo al equipo

Los archivos son markdown y JSON; no hay código. Para que refleje la práctica de
tu área, lo más rentable en este orden:

1. Sustituir los formatos de salida por tus cédulas y machotes reales.
2. Agregar al archivo de referencia los criterios internos, circulares y
   lineamientos que tu órgano de control aplica.
3. Incorporar los criterios del TRIJAEM y las tesis que en la práctica te han
   servido o te han tumbado asuntos.

## Alcance

Herramienta de apoyo técnico para el trabajo de auditoría y de los órganos de
control. No sustituye la valoración jurídica de la autoridad investigadora,
substanciadora o resolutora, ni la revisión del área jurídica.
