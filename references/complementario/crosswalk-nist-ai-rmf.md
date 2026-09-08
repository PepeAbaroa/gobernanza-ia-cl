# Cruce NIST AI RMF 1.0 ↔ normativa chilena de IA — Chile aún no tiene ley propia, NIST da el método mientras tanto

> **Jerarquía distinta a las demás skills de esta arquitectura**: en protección de datos y ciberseguridad,
> la ley chilena manda y el estándar internacional enriquece. **Aquí Chile todavía no tiene ley de IA
> vigente** (ver `mapa-proyecto-ley-ia.md`) — mientras el proyecto no se apruebe, NIST AI RMF y el Oficio
> 711 son las referencias más concretas disponibles para actuar responsablemente hoy. Cuando la ley se
> apruebe, este archivo debe revisarse para que NIST vuelva a ser complementario de una norma chilena
> específica, no el marco principal por defecto.

## Las 4 funciones NIST AI RMF 1.0

> **TEXTO LITERAL** (`sources/complementario/nist-ai-rmf-100-1.pdf.extracto/chunk_024.md`)
> "The Core is composed of four functions: GOVERN, MAP, MEASURE, and MANAGE. [...] Governance is designed
> to be a cross-cutting function to inform and be infused throughout the other three functions."

> **TEXTO LITERAL** (`chunk_025.md`, función Govern)
> "The GOVERN function: cultivates and implements a culture of risk management within organizations
> designing, developing, deploying, evaluating, or acquiring AI systems; outlines processes, documents,
> and organizational schemes that anticipate, identify, and manage the risks a system can pose [...]
> connects technical aspects of AI system design and development to organizational values and principles
> [...] addresses full product lifecycle [...] including [...] third-party software or hardware systems
> and data."

**Razonamiento aplicado:** GOVERN es transversal (igual diseño que NIST CSF 2.0 y NIST Privacy Framework,
ya usados en `infraestructura-ciberseguridad` y `proteccion-datos-personales-cl` — NIST reutiliza esta
arquitectura de "función de gobierno central" en sus 3 frameworks). Para un SLEP que evalúe adoptar un
sistema de IA (ej. corrector automático, sistema de alerta de deserción), el orden recomendado es: GOVERN
primero (política y cultura de riesgo) → MAP (entender el contexto y mapear el sistema específico) →
MEASURE/MANAGE (medir y gestionar el riesgo concreto).

## Cruce con lo que Chile ya exige hoy (Oficio 711 + normativa vigente)

| Función NIST AI RMF | Qué ya exige Chile hoy (sin esperar la ley de IA) |
|---|---|
| **GOVERN** | Oficio 711 punto 1 (IA centrada en las personas: evaluar si la IA es la solución apropiada antes de adoptarla) |
| **MAP** (entender el contexto, mapear el sistema y sus datos) | Oficio 711 punto 3 (privacidad y uso de datos) + `proteccion-datos-personales-cl` (Art. 15 ter EIPD, obligatoria si hay perfilamiento — un sistema de IA que perfila casi siempre dispara esto) |
| **MEASURE** | Sin equivalente chileno específico todavía — hueco real hasta que exista reglamento de la ley de IA |
| **MANAGE** | Oficio 711 punto 3 (seguir normas de ciberseguridad, Decreto 7) + `infraestructura-ciberseguridad` |

**Razonamiento aplicado:** MEASURE (medir cuantitativamente el riesgo/desempeño/sesgo del sistema de IA)
es la función menos cubierta por la normativa chilena actual — ninguna fuente específica disponible hoy
desarrolla métricas obligatorias de IA. Es el área donde más vale apoyarse en NIST AI RMF (y su Playbook,
mencionado en `chunk_025.md`) mientras no exista una guía chilena propia.

## Sobre el EU AI Act (mencionado en tu investigación) — pendiente de extracción completa
El EU AI Act es el marco vinculante más maduro del mundo (clasificación por riesgo: inaceptable/alto/
limitado/mínimo; prohíbe *social scoring*; exige auditorías a sistemas de alto riesgo) — **la propia
Asesoría Técnica de la BCN advierte que el proyecto de ley chileno importa varias definiciones de este
marco sin adaptarlas completamente** (ver `mapa-proyecto-ley-ia.md`). No se extrajo el texto completo del
EU AI Act en esta sesión (es un reglamento europeo extenso, >100 artículos) — queda pendiente para una
sesión dedicada si se necesita profundidad de cita literal; mientras tanto, se usa como referencia de
que la clasificación por 4 niveles de riesgo que propone Chile sigue el mismo patrón europeo, no es una
invención nacional.

## Grafo
Se combina con `mapa-proyecto-ley-ia.md`, `mapa-oficio-711.md` (ambos en `references/especifico/`) y
`proteccion-datos-personales-cl` (EIPD, decisiones automatizadas). Ver `## Grafo` en `SKILL.md`.
