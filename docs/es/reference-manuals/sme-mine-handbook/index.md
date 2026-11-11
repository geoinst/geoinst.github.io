---
lang: es
lang_alt: reference-manuals/sme-mine-handbook/
---

# SME Mining Engineering Handbook — Instrumentación Geotécnica (Cap. 8.5)

!!! note "Acerca de esta referencia"
    Esta página es un **digest abierto y original** del **Capítulo 8.5 — *Geotechnical
    Instrumentation*** del **SME Mining Engineering Handbook** (3.ª edición),
    escrito por **Erik Eberhardt** (Universidad de British Columbia) y **Doug
    Stead** (Universidad Simon Fraser). Es un resumen a nivel de capítulo —**no** una
    reproducción del texto fuente con derechos de autor. El manual es publicado por
    la Society for Mining, Metallurgy & Exploration (SME); el capítulo original y sus
    figuras siguen siendo propiedad de los autores y del editor. El digest se ofrece
    con fines educativos y de orientación; se proporciona una traducción completa al
    vietnamita a su lado, y el PDF original en inglés se reproduce aquí como
    referencia.

El **Capítulo 8.5, *Instrumentación Geotécnica***, es uno de los sondeos modernos
más citados sobre la práctica de instrumentación en minería. Escrito por dos de los
académicos de mecánica de rocas líderes del campo, abarca **21 páginas** (pp.
551–570) y se organiza en torno a una sola idea rectora: la instrumentación cumple
**dos funciones distintas** —la función *investigativa* (recolectar los parámetros
de entrada que un modelo de diseño necesita) y la función de *monitoreo* (observar
cómo responde realmente el terreno, y advertir cuando se aparta del diseño).

Ese encuadre es lo que hace útil al capítulo. Más que un catálogo de instrumentos,
se lee como una **secuencia de decisiones**: ¿qué pregunta intenta responder, qué
parámetro la responde, qué instrumento mide ese parámetro con rango, resolución,
exactitud y confiabilidad suficientes —y cómo recupera los datos en una forma en que
alguien pueda actuar?

---

## Alcance de esta referencia

| # | Sección | Qué cubre |
|---|---------|----------------|
| 1 | **Introducción** | Funciones investigativa vs. de monitoreo; los siete criterios de selección de instrumentos —rango, resolución, exactitud, precisión, conformidad, robustez, confiabilidad |
| 2 | **Instrumentación para investigación** | Técnicas de perforación (orientación de testigo, televisión de pozo, geofísica de pozo); teledetección (LiDAR, fotogrametría digital); geofísica de superficie; caracterización de aguas subterráneas (piezómetros, ensayo de flujo); medición de esfuerzos in-situ (overcoring, fracturamiento hidráulico) |
| 3 | **Instrumentación para monitoreo** | Enfoque de planificación de 20 pasos de Dunnicliff; tipos de transductores; desplazamiento de superficie (geodésico/RTS, GPS); extensómetros; inclinómetros de pendiente; desplazamiento de perforación (inclinómetro de sondeo y en sitio, extensómetros de pozo, sistemas de convergencia, arreglos de acelerómetros en forma, TDR, fibra óptica); teledetección de deformación (InSAR, radar de taludes, LiDAR/fotogrametría); células de presión; microsismicidad |
| 4 | **Adquisición y presentación de datos** | Transmisión inalámbrica de datos; inmersión y visualización de datos; modelos integrados de datos de mina |
| 5 | **Referencias** | Una lista de 64 referencias que abarca métodos sugeridos de ISRM, simposios de estabilidad de taludes de SAIMM, y la literatura primaria de revistas |

El capítulo se ilustra con **14 figuras** y **5 tablas**, todas reproducidas en la
traducción al vietnamita más abajo.

---

## Documentos completos (PDF)

=== "Vietnamita — traducción completa (PDF)"

    **Bản dịch tiếng Việt đầy đủ — Chương 8.5** (29 pp., A4).
    Traducción íntegra de todo el Capítulo 8.5, con **5 tablas** y **14 figuras**,
    incluida la lista completa de referencias. Terminología normalizada según
    **TCVN** (áp kế, thiết bị đo biến dạng sâu, ống đo nghiêng, hộp đo áp lực…),
    presentada en fuente **Times New Roman**.

    [:material-file-download: **Descargar PDF de la traducción vietnamita (completo)**](https://geoinst.github.io/assets/sme-mine-handbook/sme-mine-handbook-ch85-vietnamese.pdf){ .md-button .md-button--primary }

=== "Inglés — capítulo original (PDF)"

    **Capítulo original en inglés** — *SME Mining Engineering Handbook, Chapter 8.5:
    Geotechnical Instrumentation* (21 pp., pp. 551–570), por Erik Eberhardt y
    Doug Stead. Reproducido aquí tal como lo publica la Society for Mining,
    Metallurgy & Exploration (SME) como referencia.

    [:material-file-download: **Descargar el Capítulo 8.5 original (inglés, PDF)**](https://geoinst.github.io/assets/sme-mine-handbook/sme-mine-handbook-ch85-original-en.pdf){ .md-button }
    &nbsp;
    [Página del editor — SME](https://www.smenet.org/){ target=_blank }

---

## Por qué este capítulo importa en esta base de conocimientos

El Capítulo 8.5 es la **contraparte del lado minero** al material del lado civil sobre
el que se construye el resto de esta biblioteca:

- Su **marco de criterios de selección** (rango, resolución, exactitud, precisión,
  conformidad, robustez, confiabilidad) es el vocabulario que este sitio usa cada vez
  que se especifica un instrumento —véase
  [Primeros Pasos](../../../getting-started/index.md).
- Su **tabla de transductores** (LVDT, cuerda vibratoria, acelerómetro, fibra óptica,
  MEMS) explica *por qué* cada instrumento se comporta como lo hace, y es el
  complemento natural de los digests [Dunnicliff](../../../reference-manuals/dunnicliff/index.md)
  y [FHWA](../../../reference-manuals/fhwa/index.md).
- Su **procedimiento de planificación de 20 pasos de Dunnicliff** es la columna
  vertebral detrás de la [arquitectura ADAQS de seis capas](../../../vi/adaqs/index.md)
  neutra al proveedor de este sitio.
- Sus secciones de **esfuerzos in-situ** y **piezómetros** dan la base de mecánica de
  rocas y aguas subterráneas desde la cual
  [Mecánica de Suelos](../../../reference-manuals/soil-mechanics/index.md) y
  [Ingeniería de Cimentaciones](../../../reference-manuals/foundation-engineering/index.md)
  se aproximan desde el lado del suelo.

---

## Cómo usar esta referencia

- **Lea primero los criterios de selección** (§1). La mayoría de las fallas de
  instrumentación son fallas de especificación, no de sensor.
- Use la **tabla de 20 pasos de Dunnicliff** como lista de verificación antes de
  comprar nada —los pasos 1–8 son los más omitidos.
- Trabaje **investigación antes que monitoreo**: el capítulo es explícito en que el
  monitoreo predictivo debe seguir a un período de monitoreo investigativo.
- Enlácelo con [Dunnicliff](../../../reference-manuals/dunnicliff/index.md),
  [FHWA](../../../reference-manuals/fhwa/index.md),
  [Monitoreo del Desempeño de Presas](../../../reference-manuals/monitoring-dam-performance/index.md)
  y [Seguridad de Presas de Relaves](../../../reference-manuals/tailings-dam-safety/index.md)
  para profundidad del lado civil.
- Consulte al [GTI Doctor](../../../gti-doctor.md) para extraer detalles del corpus
  más amplio.

> **Seguridad y vigencia.** La tecnología de teledetección y sensores inalámbricos ha
> avanzado considerablemente desde que se escribió este capítulo —los tiempos de
> revisiteo InSAR, la precisión del radar y la sensibilidad distribuida por fibra
> óptica siguen mejorando. Trate los **principios y la lógica de selección** como
> duraderos y **verifique las especificaciones actuales de los instrumentos** con
> los fabricantes antes de confiar en ellas para un diseño o una presentación
> regulatoria.

---

## Video Destacado y Recursos Prácticos

<div class="video-container" style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; margin-bottom: 1rem;">
  <iframe src="https://www.youtube-nocookie.com/embed/pgIjAXKyPWY" title="Rock Mass Properties - Dr. Evert Hoek Lecture Series" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border-radius: 6px;"></iframe>
</div>
<p><em>Conferencia Magistral Destacada (Rocscience): Serie de Conferencias del Dr. Evert Hoek — Rock Mass Properties: Caracterización In-situ, Sistema GSI, y Mecánica de Rocas Subterránea y a Cielo Abierto.</em></p>

!!! tip "Recursos Prácticos de Campo Complementarios de RST Instruments & Measurand (Terra Insights)"
    - **RST Instruments (@RSTgeotechnical):** [Wireless Data Collection with RSTAR](https://www.youtube.com/watch?v=xFplwoCngEU){ target="_blank" }  
      *Redes autónomas de sensores geotécnicos de toda la mina para bancos a cielo abierto y facility de relaves.*
    - **Measurand (@MeasurandVideos):** [Real-time deflection monitoring with ShapeArray](https://www.youtube.com/watch?v=518Mx-65rI0){ target="_blank" }  
      *Seguimiento continuo de cizalle y movimiento subsuperficial a lo largo de muros altos de mina y depósitos de estéril.*
