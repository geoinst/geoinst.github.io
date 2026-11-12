---
lang: es
lang_alt: reference-manuals/soil-mechanics/
---

# Mecánica de Suelos e Ingeniería Geotécnica: Una Referencia de Dominio Público

!!! note "Acerca de esta referencia"
    Esta es una **referencia técnica abierta y original** sobre mecánica de suelos e
    ingeniería geotécnica, escrita en lenguaje de ingeniería sencillo. Al igual que el
    libro [Ingeniería de Cimentaciones](../foundation-engineering/index.md),
    se construye **enteramente a partir de fuentes de dominio público** —el
    ***Soils and Foundations Reference Manual*** de FHWA NHI y los **Manuales de
    Ingeniería del USACE**, todos los cuales son **obras del gobierno de EE. UU. en
    dominio público**. No se reproduce ningún libro de texto con derechos de autor.
    Se ofrece con fines educativos y de campo; cada sitio es único y esta referencia
    construye criterio de ingeniería, no normas mínimas. Los manuales subyacentes
    están indexados en el asistente de IA [GTI Doctor](../../../gti-doctor.md).

La **mecánica de suelos** es la ciencia de cómo el suelo —un material de tres fases
de sólidos, agua y aire— responde al esfuerzo y al agua. Es la base de todo cálculo
geotécnico: capacidad de carga, asentamiento, estabilidad de taludes, presión de
tierras y filtración descansan sobre ella. Esta referencia cubre el núcleo clásico
—composición y clasificación, compactación, permeabilidad y filtración, esfuerzo
efectivo, consolidación, resistencia al corte y rigidez— más las cuestiones
prácticas de ensayos in-situ, selección de parámetros y suelos problemáticos.

---

## Alcance de esta referencia

| # | Capítulo | Qué cubre |
|---|---------|----------------|
| 1 | [Introducción y Fuentes](chapter-01-introduction.md) | Por qué la mecánica de suelos; el corpus de dominio público |
| 2 | [Composición del Suelo y Propiedades Índice](chapter-02-composition-index.md) | Fases, pesos unitarios, relación de vacíos, límites de Atterberg |
| 3 | [Clasificación de Suelos](chapter-03-classification.md) | Sistemas USCS y AASHTO; qué le dicen al ingeniero |
| 4 | [Compactación](chapter-04-compaction.md) | Ensayos Proctor, humedad–densidad, control de campo |
| 5 | [Permeabilidad](chapter-05-permeability.md) | Ley de Darcy, medición de laboratorio y campo |
| 6 | [Filtración y Redes de Flujo](chapter-06-seepage.md) | Redes de flujo, empuje, piping, filtros |
| 7 | [Esfuerzo Efectivo y Presión de Poros](chapter-07-effective-stress.md) | El principio del esfuerzo efectivo; total vs. efectivo |
| 8 | [Distribución de Esfuerzos en el Suelo](chapter-08-stress-distribution.md) | Boussinesq, cartas de influencia, aumento de esfuerzo con la profundidad |
| 9 | [Consolidación](chapter-09-consolidation.md) | Teoría de Terzaghi, $c_v$, preconsolidación, tasa de asentamiento |
| 10 | [Resistencia al Corte](chapter-10-shear-strength.md) | Mohr–Coulomb, drenado vs. no drenado, ensayos de laboratorio |
| 11 | [Rigidez y Esfuerzo–Deformación](chapter-11-stiffness.md) | Módulo, no linealidad, comportamiento de pequeña deformación |
| 12 | [Ensayos In-situ y Selección de Parámetros](chapter-12-in-situ-testing.md) | SPT, CPT, pala, presurómetro; elección de parámetros |
| 13 | [Suelos Problemáticos](chapter-13-problem-soils.md) | Suelos expansivos, colapsables, orgánicos y licuables |
| 14 | [Programa de Ensayos de Laboratorio y Campo](chapter-14-testing-program.md) | Planificación de ensayos para responder preguntas de diseño |

---

## Las fuentes de dominio público

| Fuente | Título | Alcance |
|--------|-------|-------|
| FHWA-NHI-06-088 (Vol. I) | *Soils and Foundations Reference Manual* | Propiedades del suelo, clasificación, compactación, filtración, esfuerzo, consolidación, resistencia al corte |
| USACE EM 1110-2-1906 | *Laboratory Soils Testing* | Procedimientos estándar de ensayo de laboratorio |
| USACE EM 1110-1-1904 | *Settlement Analysis* | Parámetros de consolidación y asentamiento |
| USACE EM 1110-2-1902 | *Slope Stability* | Resistencia al corte para análisis de estabilidad |
| FHWA-NHI-01-031 (GEC-5) | *Evaluation of Soils and Rock for Subsurface Investigations* | Ensayos in-situ y selección de parámetros |

> **Dominio público significa reutilizable.** Los manuales de USACE y FHWA son
> obras del gobierno federal de EE. UU. y no están sujetos a derechos de autor en
> Estados Unidos. Esta referencia los presenta como una síntesis original, no como
> una copia literal.

---

## Cómo usar esta referencia

- **Léala junto con el libro [Ingeniería de Cimentaciones](../foundation-engineering/index.md)**
  —este aporta los parámetros y la mecánica del suelo; aquel los aplica a las cimentaciones.
- **Úsela con los libros de monitoreo.** La presión de poros (Capítulo 7) y la
  resistencia al corte (Capítulo 10) son la física detrás de las referencias de
  instrumentos [Dunnicliff](../dunnicliff/index.md) y
  [FHWA](../fhwa/index.md).
- **Consulte al [GTI Doctor](../../../gti-doctor.md)** para el texto de los manuales subyacentes.

> **Los parámetros no son verdad.** Todo parámetro de suelo lleva incertidumbre;
> la buena ingeniería la acota y diseña para el rango, no para un número único.

---

## Video Destacado y Recursos Prácticos

<div class="video-container" style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; margin-bottom: 1rem;">
  <iframe src="https://www.youtube-nocookie.com/embed/uElPkghqoJw" title="What is Geotechnical Engineering? | ISSMGE" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border-radius: 6px;"></iframe>
</div>
<p><em>Video Destacado (Sociedad Académica — ISSMGE): Visión general oficial de la Mecánica de Suelos y la Ingeniería Geotécnica por la International Society for Soil Mechanics and Geotechnical Engineering.</em></p>

!!! tip "Recursos Prácticos de Campo Complementarios de RST Instruments & Measurand (Terra Insights)"
    - **RST Instruments (@RSTgeotechnical):** [Taking Initial Vibrating Wire Piezometer Readings](https://www.youtube.com/watch?v=HJISt9or_Dw){ target="_blank" }  
      *Lecturas de línea base in-situ de presión de poros para evaluación de esfuerzo efectivo y seguimiento de consolidación.*
    - **Measurand (@MeasurandVideos):** [ShapeArray Rail Settlement Monitoring](https://www.youtube.com/watch?v=f3NMguxiZSE){ target="_blank" }  
      *Monitoreo continuo de deformación y asentamiento de subyacente bajo carga cíclica.*
