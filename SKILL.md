---
name: gobernanza-ia-cl
description: Activa cuando el usuario trabaja gobernanza de inteligencia artificial — evaluar/adoptar un sistema de IA, gestión de riesgo de IA, sesgo algorítmico, decisiones automatizadas, perfilamiento, explicabilidad, transparencia algorítmica, uso de IA generativa en el sector público, Proyecto de Ley de IA en Chile, Oficio Circular 711, NIST AI RMF, EU AI Act, o ISO 42001/23894. **NO activa para** la base legal de datos personales usados para entrenar o alimentar un sistema de IA — usar `proteccion-datos-personales-cl`; **NO activa para** controles técnicos de seguridad del sistema que aloja la IA — usar `infraestructura-ciberseguridad`; **NO activa para** calidad/linaje de los datos de entrenamiento — usar `data-governance`; **NO activa para** implementación de código del modelo — usar 04-tyb-expert-programmer o 04-tyb-data-scientist-phd.
---

# Gobernanza de Inteligencia Artificial (Chile) — experta en un marco regulatorio todavía en formación

Skill de referencia normativa más reciente y menos estable de esta arquitectura: **Chile no tiene ley de
IA vigente todavía** — hay un proyecto en segundo trámite en el Senado (Boletín 16.821-19) y un
instructivo no vinculante para el sector público (Oficio 711/2023). Mientras no exista ley, esta skill
se apoya en NIST AI RMF como método de trabajo y traslada la responsabilidad de verificar vigencia al
usuario en cada consulta — más que ninguna otra skill de este ecosistema.

## Metodología de razonamiento

1. **Verificar primero si hay ley vigente o solo proyecto**: a la fecha de esta reconstrucción
   (2026-09-08) NO hay ley de IA en Chile — solo proyecto en el Senado. **Verificar activamente el estado
   actual en `tramitacion.senado.cl` antes de cualquier afirmación normativa dura** — este es el dato con
   mayor probabilidad de quedar obsoleto de toda esta arquitectura de skills.
2. **Clasificar el sistema de IA en cuestión**: ¿hace perfilamiento o decisiones automatizadas con efecto
   jurídico o significativo? Si sí, ya está regulado HOY por la Ley 19.628 modificada (Art. 8° bis, Art.
   15 ter EIPD obligatoria) — no hace falta esperar la ley de IA para tener obligaciones concretas.
3. **Si es una institución pública** (SLEP, cualquier órgano del Estado): aplicar el Oficio 711 (no
   vinculante pero es la política oficial) — especialmente el punto 3, nunca ingresar datos sensibles a
   IA generativa no contratada institucionalmente.
4. **Usar NIST AI RMF como método de trabajo** (Govern → Map → Measure → Manage) para estructurar
   cualquier evaluación de riesgo de un sistema de IA nuevo — es voluntario y no chileno, pero es lo más
   concreto disponible mientras no exista reglamento nacional.
5. **Distinguir explícitamente qué es ley, qué es proyecto de ley, y qué es solo recomendación no
   vinculante** en cualquier respuesta — la confusión entre estos 3 niveles es el riesgo principal de
   esta skill.
6. **Cruzar con las skills adyacentes según la pieza que falte**: base legal del dato de entrenamiento →
   `proteccion-datos-personales-cl`; calidad/linaje del dato → `data-governance`; control técnico del
   sistema que aloja la IA → `infraestructura-ciberseguridad`.

**Regla de cierre**: en toda respuesta sustantiva, indicar explícitamente si lo citado es (a) ley vigente,
(b) proyecto de ley en tramitación — con su estado actual verificado, no supuesto, o (c) recomendación no
vinculante — nunca presentar (b) o (c) como si fueran (a).

## Tabla de decisión
| La tarea trata de… | Ir a |
|---|---|
| Qué dice el proyecto de ley de IA, estructura, temas en debate | `references/especifico/mapa-proyecto-ley-ia.md` (leer la advertencia de vigencia primero) |
| Qué recomienda el Estado para uso de IA en el sector público hoy | `references/especifico/mapa-oficio-711.md` |
| Método de evaluación de riesgo de un sistema de IA (Govern/Map/Measure/Manage) | `references/complementario/crosswalk-nist-ai-rmf.md` |
| Decisiones automatizadas/perfilamiento — base legal YA vigente | skill `proteccion-datos-personales-cl` (Art. 8 bis, 15 ter) |
| Calidad/linaje de datos de entrenamiento | skill `data-governance` |
| Seguridad técnica del sistema que aloja la IA | skill `infraestructura-ciberseguridad` |
| ISO 42001/22989/23894, EU AI Act completo, libros | pendientes de adquisición/extracción, ver Fuentes complementarias |

## Reglas de oro
1. **Nunca presentar el proyecto de ley como ley vigente** — verificar estado de tramitación en cada uso
   de alto riesgo, no confiar en la fecha de esta skill indefinidamente.
2. El Oficio 711 es recomendación, no obligación legal por sí sola — pero conecta con obligaciones YA
   vigentes (Ley 19.628, Decreto 7) que si son obligatorias.
3. Un sistema de IA que perfila o decide automáticamente ya está regulado hoy (Ley 19.628 modificada) —
   no esperar la ley de IA para actuar con esos casos.
4. Nunca ingresar datos personales sensibles de un SLEP/cliente a IA generativa de consumo no contratada
   institucionalmente (Oficio 711 punto 3) — regla operativa inmediata, no aspiracional.
5. No importar definiciones del EU AI Act como si fueran automáticamente parte del derecho chileno — el
   propio proyecto de ley chileno ha sido criticado por hacer esto sin adaptación (ver
   `mapa-proyecto-ley-ia.md`).

## Fuentes — capa específica
- `sources/especifico/bcn-analisis-proyecto-ley-ia.pdf` — Asesoría Técnica Parlamentaria BCN, jul-2024,
  24 páginas, consulta a 8 expertos sobre el Proyecto de Ley de IA (Boletín 16.821-19). **No es el texto
  del proyecto ni de una ley — es análisis oficial de un estado anterior del trámite.**
- `references/especifico/mapa-oficio-711.md` — basado en resumen de fuente jurídica especializada (PDF
  primario del Oficio Circular 711/2023 no localizado aún en esta sesión).

## Fuentes — capa complementaria
- `sources/complementario/nist-ai-rmf-100-1.pdf` — NIST AI 100-1 (ene-2023), oficial y gratuito, ya usado
  también en `proteccion-datos-personales-cl` (mismo archivo, no duplicar contenido, solo referenciar).
- **Pendiente de adquisición (de pago, no descargadas)**: ISO/IEC 42001 (sistema de gestión de IA),
  ISO/IEC 22989 (conceptos y terminología), ISO/IEC 23894 (gestión de riesgo de IA).
- **Pendiente de extracción** (gratuito pero muy extenso, no procesado esta sesión): EU AI Act completo —
  se usa por ahora solo como referencia general de estructura (clasificación por 4 niveles de riesgo).
- **Libros solicitados, no localizados como copia legítima en este disco**: "The AI Capability
  Framework", "Ethical Machines" (Reid Blackman), "Turning Point: Policymaking in the Era of AI" —
  comerciales, no se buscan copias no autorizadas; si Pepe tiene acceso legítimo, indicar la fuente para
  procesarlos.

## Grafo — con qué otras skills se combina y cómo
- **`proteccion-datos-personales-cl`** (fuente-para): cualquier sistema de IA que trate datos personales
  para entrenar o decidir debe resolver primero ahí la base legal (Art. 8 bis, 15 ter) — esta skill no
  la reemplaza, la complementa con el ángulo de gestión de riesgo de IA específicamente.
- **`data-governance`** (complementa): calidad y linaje del dato de entrenamiento es requisito previo a
  cualquier evaluación de riesgo de IA seria (DAMA-DMBOK Cap. 14, Big Data and Data Science).
- **`infraestructura-ciberseguridad`** (complementa): el sistema que aloja la IA necesita los mismos
  controles técnicos que cualquier otro sistema crítico.
- **04-tyb-data-scientist-phd** / **04-tyb-expert-programmer** (deriva-a): implementación técnica del modelo.
