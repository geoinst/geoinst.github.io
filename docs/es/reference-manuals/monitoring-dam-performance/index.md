---
lang: es
lang_alt: reference-manuals/monitoring-dam-performance/
---

# Monitoreo del Desempeño de Presas: Instrumentación y Mediciones

!!! note "Acerca de esta referencia"
    Esta es una **referencia técnica abierta y original** sobre el monitoreo del
    desempeño de presas, escrita en lenguaje de ingeniería sencillo y adaptada a
    partir de la estructura y el alcance temático de *Monitoring Dam Performance:
    Instrumentation and Measurements* — **ASCE Manual of Practice No. 135 (2019)**,
    preparado por el ASCE/EWRI Task Committee on Instrumentation and Monitoring of
    Dams and Levees. **No** es una reproducción del texto con derechos de autor de
    ASCE. Se ofrece con fines educativos y de campo, y cada presa es única: la
    orientación aquí busca construir criterio de ingeniería, no fijar normas mínimas.

La **seguridad de presas** depende de conocer cómo se comporta realmente una presa.
El monitoreo es la disciplina de medir ese comportamiento —tanto por observación
humana como por instrumentos— y convertir esas mediciones en decisiones oportunas y
defendibles. Esta referencia recorre el ciclo de vida completo de un programa de
monitoreo: desde definir qué podría salir mal, hasta seleccionar e instalar
instrumentos, y adquirir, evaluar y actuar sobre los datos.

---

## Alcance de esta referencia

Este libro cubre los fundamentos y el estado actual de la práctica para monitorear
el desempeño de presas (y, por extensión, sus estructuras accesorias, cimentaciones
y embalses). Está organizado en los siguientes capítulos:

| # | Capítulo | Qué cubre |
|---|---------|----------------|
| 1 | [Introducción: Propósito, Alcance y Organización](chapter-01-introduction.md) | Por qué importa el monitoreo; cómo se organiza esta referencia |
| 2 | [Desempeño de la Presa y Modos de Falla Potenciales](chapter-02-failure-modes.md) | Cómo fallan las presas y qué signos preceden a la falla |
| 3 | [Filosofía de Monitoreo: Vigilancia Visual e Instrumentación](chapter-03-philosophy.md) | Los dos pilares del monitoreo y cómo se complementan |
| 4 | [Planificación de un Programa de Monitoreo de Presas](chapter-04-planning.md) | Un proceso estructurado para definir qué, dónde y por qué monitorear |
| 5 | [Familias de Instrumentos para Monitoreo de Presas](chapter-05-instruments.md) | Sensores de topografía, geotécnicos, hidrológicos y estructurales de un vistazo |
| 6 | [Piezómetros y Monitoreo de Presión de Poros](chapter-06-piezometers.md) | Saturación, instalación y lectura de presión de poros |
| 7 | [Monitoreo de Filtraciones, Escapes y Superficie Freática](chapter-07-seepage.md) | Cuantificación e interpretación de filtraciones |
| 8 | [Monitoreo de Deformación: Topografía y Sensores Geotécnicos](chapter-08-deformation.md) | Monolitos de referencia, inclinómetros, extensómetros, inclinómetros de pendiente |
| 9 | [Sistemas de Monitoreo Automatizado, Remoto y en Tiempo Real](chapter-09-automated.md) | Adquisidores de datos, telemetría, umbrales y alarmas |
| 10 | [Instalación, Operación y Mantenimiento](chapter-10-iom.md) | Obtener datos confiables durante la vida útil del instrumento |
| 11 | [Adquisición, Gestión de Datos y Bases de Datos](chapter-11-data-management.md) | Frecuencias, validación y sistemas de datos |
| 12 | [Evaluación, Presentación e Interpretación de Datos](chapter-12-evaluation.md) | Gráficos, líneas base y separación de señal y ruido |
| 13 | [Evaluación del Desempeño y Toma de Decisiones](chapter-13-decisions.md) | De la anomalía a la acción |
| 14 | [Historias de Caso](chapter-14-case-histories.md) | Lecciones de programas de monitoreo reales |

---

## Cómo usar esta referencia

- **Comience por los Capítulos 2 y 4.** Los modos de falla y un plan estructurado
  son la base de todo buen programa de monitoreo.
- **Enlácela con el resto de la base de conocimientos.** El capítulo
  [Familias de Instrumentos](chapter-05-instruments.md)
  remite a los manuales   [Dunnicliff](../dunnicliff/index.md) y
  [FHWA](../fhwa/index.md) para procedimientos detallados de instalación.
- **Consulte al [GTI Doctor](../../gti-doctor.md).** El asistente de IA puede
  responder preguntas de monitoreo desde el corpus más amplio.

---

## Una nota sobre unidades y terminología

Tanto las unidades SI como las unidades usuales de EE. UU. aparecen en la práctica;
esta referencia usa el conjunto de unidades más común a cada tema y declara las
conversiones donde importan. "Desempeño" significa el comportamiento observado de la
presa comparado con su comportamiento esperado.

> **Seguridad primero.** Los datos de instrumentos apoyan, pero nunca reemplazan, la
> inspección visual calificada y el criterio de ingeniería de un ingeniero de presas
> calificado o del programa de seguridad de presas del propietario.

---

## Video Destacado y Recursos Prácticos

<div class="video-container" style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; margin-bottom: 1rem;">
  <iframe src="https://www.youtube-nocookie.com/embed/lIvGH5bux5Q" title="Dam Owner Academy: Dam Inspections | Association of State Dam Safety Officials (ASDSO)" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border-radius: 6px;"></iframe>
</div>
<p><em>Video Destacado (Dam Safety Institute — ASDSO / USSD): Inspecciones de Presas y Monitoreo del Desempeño para Presas de Terraplén y de Concreto.</em></p>

!!! tip "Recursos Prácticos de Campo Complementarios de RST Instruments & Measurand (Terra Insights)"
    - **RST Instruments (@RSTgeotechnical):** [Taking Initial Vibrating Wire Piezometer Readings](https://www.youtube.com/watch?v=HJISt9or_Dw){ target="_blank" }  
      *Verificación de línea base para piezómetros de cuerda vibratoria de terraplén y cimentación de presas conforme a ASCE MOP-135.*
    - **Measurand (@MeasurandVideos):** [Real-time deflection monitoring with ShapeArray](https://www.youtube.com/watch?v=518Mx-65rI0){ target="_blank" }  
      *Monitoreo continuo automatizado de deformación de corona y núcleo interno de presas de terraplén.*
