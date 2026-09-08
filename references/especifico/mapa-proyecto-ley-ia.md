# Proyecto de Ley que Regula los Sistemas de Inteligencia Artificial (Boletín 16.821-19)

> ## ADVERTENCIA DE VIGENCIA — LEER ANTES DE CITAR CUALQUIER DATO DE ESTE ARCHIVO
> **NO ES LEY VIGENTE.** Es un proyecto de ley, refundido con el Boletín 15.869-19, aprobado en general
> por la Cámara de Diputados (4-ago-2025) y en primer trámite constitucional (13-oct-2025); actualmente
> en **segundo trámite constitucional en el Senado** (Comisión de Desafíos del Futuro, Ciencia, Tecnología
> e Innovación + Comisión de Hacienda), con urgencia, verificado por búsqueda web 2026-09-08. El texto
> puede modificarse en el Senado antes de convertirse en ley. **Verificar el estado actual en
> `tramitacion.senado.cl` (boletín 16821-19) antes de cualquier uso operativo o de alto riesgo.**
>
> La fuente citable en `sources/especifico/bcn-analisis-proyecto-ley-ia.pdf` es un documento de
> **Asesoría Técnica Parlamentaria de la BCN, julio 2024** (consulta a 8 expertos sobre el proyecto en su
> versión de esa fecha) — es un análisis oficial y verificado, pero **anterior a la aprobación en general
> por la Cámara (ago-2025)** y a las indicaciones del Senado. Da la estructura y los temas en debate, no
> garantiza que cada artículo mencionado sobreviva igual en el texto final.

## Estructura del proyecto (10 títulos, según la versión analizada jul-2024)

> **TEXTO LITERAL** (`sources/especifico/bcn-analisis-proyecto-ley-ia.pdf.extracto/chunk_018.md`)
> "TÍTULO 8. Confidencialidad, infracciones y sanciones (artículos 23 a 29) [...] se describen las
> infracciones y sanciones, así como el procedimiento administrativo sancionador, que estará
> principalmente a cargo de la **agencia de Protección de Datos Personales**; el procedimiento de
> reclamación judicial, materias de responsabilidad civil y el procedimiento aplicable."

**Razonamiento aplicado — hallazgo relevante, verificar si se mantiene**: en la versión analizada, la
fiscalización de la ley de IA recaería en la **misma Agencia de Protección de Datos Personales** creada
por la Ley 19.628 modificada (ver `proteccion-datos-personales-cl`), no en una agencia de IA separada —
si esto se mantiene en el texto final, ambas materias (datos personales e IA) quedarían bajo un mismo
regulador en Chile, a diferencia de la UE (que sí separa autoridades). **Verificar activamente si esto
cambió durante el trámite en el Senado.**

> **TEXTO LITERAL** (`chunk_019.md`)
> "TÍTULO 9. Disposiciones finales [...] este apartado del proyecto define los elementos que deberá
> incluir el reglamento de la ley, que incluye los **listados de sistemas de IA de alto riesgo y de riesgo
> limitado**, además de cómo dar cumplimiento a las reglas que se aplicarían a cada una de estas
> categorías."

**Razonamiento aplicado:** confirma la clasificación por niveles de riesgo que menciona tu investigación
(inaceptable / alto / limitado / sin riesgo — mismo enfoque del EU AI Act, ver
`references/complementario/`) — pero el detalle fino de qué sistemas caen en cada categoría se delega a
un **reglamento posterior**, no está en el articulado mismo. **No until el reglamento exista, la
clasificación operativa exacta no puede citarse con precisión de artículo.**

> **TEXTO LITERAL** (`chunk_007.md`)
> "Pregunta 2. El artículo 3° establece **25 definiciones** ¿Le parecen suficientes y adecuadas? [...]
> muchos [conceptos] idénticos a la regulación de la Unión Europea, sin correlato con la regulación
> nacional."

**Razonamiento aplicado:** el propio panel de expertos consultado por la BCN advierte que el proyecto
importa definiciones del EU AI Act sin adaptarlas necesariamente al ordenamiento chileno — razón adicional
para usar el EU AI Act solo como referencia comparada (complementario), nunca asumir que un concepto
chileno significa exactamente lo mismo que su equivalente europeo sin verificar la definición local final.

### Título 10 — Modificación a la Ley de Propiedad Intelectual
> **TEXTO LITERAL** (`chunk_019.md`)
> "el proyecto propone incorporar a la Ley N° 17.336 sobre propiedad intelectual un nuevo artículo 71 T
> sobre el análisis estadístico de datos de lenguaje, sonido o lenguaje de grandes grupos de obras o de
> grandes volúmenes de datos, donde no haya explotación encubierta de obras protegidas."

**Razonamiento aplicado:** esto es la regla chilena equivalente a la excepción de "text and data mining"
del derecho europeo — relevante si un cliente entrena o usa modelos de IA sobre corpus de texto/obras con
derechos de autor (ej. un modelo de lenguaje entrenado con material educativo).

## Cifra de multa (20.000 UTM) mencionada en investigación externa — NO VERIFICADA
Tu investigación menciona multas de hasta 20.000 UTM. **No se encontró esa cifra en el documento
disponible** (`sources/especifico/bcn-analisis-proyecto-ley-ia.pdf`, que es un análisis cualitativo, no
un resumen de sanciones). No se propaga esa cifra como verificada — antes de citarla en cualquier
entregable, obtener el texto actual del articulado (Título 8, Arts. 23-29) desde
`tramitacion.senado.cl` o `camara.cl` y verificar el monto exacto vigente a esa fecha.

## Grafo
Ver `## Grafo` en `SKILL.md`. Se cruza con `references/complementario/crosswalk-eu-ai-act.md` y con
`proteccion-datos-personales-cl` (posible fiscalizador común, tratamiento de datos de entrenamiento).
