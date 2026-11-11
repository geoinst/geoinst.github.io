---
lang: es
lang_alt: reference-manuals/tailings-dam-safety/
---

# Seguridad de Presas de Relaves: Una Referencia de Ingeniería

!!! note "Acerca de esta referencia"
    Esta es una **referencia técnica abierta y original** sobre el monitoreo y la
    gestión segura de las instalaciones de almacenamiento de relaves (TSF, por su
    sigla en inglés) y sus presas, escrita en lenguaje de ingeniería sencillo. Está
    adaptada del alcance temático del **Boletín ICOLD 194 — *Tailings Dams: Safety,
    Monitoring and Surveillance* (2021)** y de la guía relacionada de la industria
    minera y ICOLD. **No** es una reproducción del texto fuente con derechos de autor.
    Se ofrece con fines educativos y de campo. Cada instalación de relaves es única y
    conlleva alta consecuencia de falla; esta referencia busca construir criterio de
    ingeniería, no fijar normas mínimas. Siga siempre el régimen regulatorio
    aplicable y el propio plan de vigilancia de la instalación.

Los relaves son los sólidos finos molidos que quedan tras extraer los minerales del
mineral. Se mezclan con agua y se depositan detrás de terraplenes de ingeniería —
**presas de relaves**— que a menudo están entre las estructuras hechas por el ser
humano más grandes de la Tierra. Como se construyen con el propio producto de desecho
y se elevan repetidamente durante décadas, exigen un enfoque distinto y disciplinado
de la seguridad, el monitoreo y la vigilancia.

Esta referencia recorre ese enfoque: entender cómo fallan las instalaciones de
relaves, construir un programa de monitoreo informado por el riesgo, seleccionar y
mantener instrumentos, y convertir las mediciones en decisiones defendibles.

---

## Alcance de esta referencia

Este libro cubre los fundamentos y el estado actual de la práctica para la seguridad,
el monitoreo y la vigilancia de las instalaciones de almacenamiento de relaves,
organizado en los siguientes capítulos:

| # | Capítulo | Qué cubre |
|---|---------|----------------|
| 1 | [Introducción: Propósito, Alcance y Organización](../../../reference-manuals/tailings-dam-safety/chapter-01-introduction.md) | Por qué la seguridad de relaves es distinta; cómo se organiza esta referencia |
| 2 | [Instalaciones de Relaves y Cómo Fallan](../../../reference-manuals/tailings-dam-safety/chapter-02-facilities-and-failures.md) | Tipos de instalación y los modos de falla dominantes |
| 3 | [Filosofía de Monitoreo para Relaves](../../../reference-manuals/tailings-dam-safety/chapter-03-philosophy.md) | La vigilancia visual y la instrumentación como pilares complementarios |
| 4 | [Planificación de un Programa de Monitoreo de Relaves](../../../reference-manuals/tailings-dam-safety/chapter-04-planning.md) | Un proceso de planificación informado por el riesgo y dirigido por la consecuencia |
| 5 | [Familias de Instrumentos para Relaves](../../../reference-manuals/tailings-dam-safety/chapter-05-instruments.md) | Herramientas topográficas, geotécnicas, hidrológicas y de teledetección de un vistazo |
| 6 | [Monitoreo de Presión de Poros y Potencial de Licuefacción](../../../reference-manuals/tailings-dam-safety/chapter-06-pore-pressure.md) | El papel central de la presión de poros en las fallas de relaves |
| 7 | [Monitoreo de Filtraciones y Superficie Freática](../../../reference-manuals/tailings-dam-safety/chapter-07-seepage.md) | Cuantificación e interpretación de filtraciones y geometría de playa |
| 8 | [Monitoreo de Deformación: Topografía y Geotécnica](../../../reference-manuals/tailings-dam-safety/chapter-08-deformation.md) | Detección de movimiento superficial e interno |
| 9 | [Sistemas Automatizados, Remotos y en Tiempo Real](../../../reference-manuals/tailings-dam-safety/chapter-09-automated.md) | Adquisidores de datos, telemetría, radar satelital y alarmas |
| 10 | [Instalación, Operación y Mantenimiento](../../../reference-manuals/tailings-dam-safety/chapter-10-iom.md) | Sostener datos confiables durante la vida de la instalación |
| 11 | [Adquisición, Gestión de Datos y Bases de Datos](../../../reference-manuals/tailings-dam-safety/chapter-11-data-management.md) | Frecuencias, validación y sistemas de datos |
| 12 | [Evaluación e Interpretación de Datos](../../../reference-manuals/tailings-dam-safety/chapter-12-evaluation.md) | Líneas base, tendencias y separación de señal y ruido |
| 13 | [Evaluación del Desempeño y Toma de Decisiones](../../../reference-manuals/tailings-dam-safety/chapter-13-decisions.md) | Disparadores, niveles de acción y respuesta de emergencia |
| 14 | [Historias de Caso](../../../reference-manuals/tailings-dam-safety/chapter-14-case-histories.md) | Lecciones de incidentes de relaves significativos |
| 15 | [Estudio de Caso: Presas de Relaves de Arenas Bituminosas del Norte de Alberta](../../../reference-manuals/tailings-dam-safety/chapter-15-oil-sands-northern-alberta.md) | Un estudio de caso detallado de la aplicación de las guías de seguridad de presas a relaves de arenas bituminosas (CDA / Golder) e instrumentación de diques in-pit (Albian) |

---

## Cómo usar esta referencia

- **Comience por los Capítulos 2 y 4.** Los modos de falla y un plan informado por
  el riesgo son la base de todo buen programa de vigilancia de relaves.
- **Enlácela con el resto de la base de conocimientos.** El capítulo
  [Familias de Instrumentos](../../../reference-manuals/tailings-dam-safety/chapter-05-instruments.md)
  remite a los manuales [Dunnicliff](../../../reference-manuals/dunnicliff/index.md) y
  [FHWA](../../../reference-manuals/fhwa/index.md) para procedimientos detallados de instalación.
- **Consulte al [GTI Doctor](../../../gti-doctor.md).** El asistente de IA puede
  responder preguntas de monitoreo desde el corpus más amplio.

---

## Una nota sobre unidades y terminología

Tanto las unidades SI como las unidades usuales de EE. UU. aparecen en la práctica;
esta referencia usa el conjunto de unidades más común a cada tema y declara las
conversiones donde importan. Una **instalación de almacenamiento de relaves (TSF)**
incluye el embalse, el(s) terraplén(es), el sistema de deposición, el decantador y
las obras de recuperación. **Vigilancia** aquí significa la combinación de
observación humana y medición por instrumentos usada para confirmar que una
instalación se comporta como se espera.

> **Seguridad primero.** Los datos de instrumentos apoyan, pero nunca reemplazan, la
> inspección visual calificada y el criterio de ingeniería de un ingeniero de relaves
> calificado y del programa de seguridad de presas de la instalación.

---

## Video Destacado y Recursos Prácticos

<div class="video-container" style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; margin-bottom: 1rem;">
  <iframe src="https://www.youtube-nocookie.com/embed/vuwZ7Wc0Xoc" title="Jagersfontein Tailings Dam collapse: InSAR analysis" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border-radius: 6px;"></iframe>
</div>
<p><em>Seminario Web Técnico Destacado (Terra Insights / 3vGeomatics): Colapso de la Presa de Relaves de Jagersfontein — Análisis InSAR, Seguimiento de Deformación Pre-Falla, y Alerta Temprana Geotécnica.</em></p>

!!! tip "Recursos Prácticos de Campo Complementarios de RST Instruments & Measurand (Terra Insights)"
    - **RST Instruments (@RSTgeotechnical):** [RSTAR Affinity Quick Dashboard Tour](https://www.youtube.com/watch?v=AQIWe60Meho){ target="_blank" }  
      *Tablero de monitoreo en la nube para flujos de datos de piezómetros y filtraciones de instalaciones de almacenamiento de relaves (TSF).*
    - **Measurand (@MeasurandVideos):** [Real-time deflection monitoring with ShapeArray](https://www.youtube.com/watch?v=518Mx-65rI0){ target="_blank" }  
      *Seguimiento de deformación en tiempo real de coronas de presas de relaves y elevaciones aguas arriba/abajo conforme al Boletín ICOLD 194.*
