---
lang: es
lang_alt: applications/dam-monitoring/
---

# Monitoreo de presas

## Objetivo

Detectar cambios de filtración, erosión interna y deformación en presas de terraplén / de concreto para prevenir fallas catastróficas.

---

## Referencias completas por capítulo de los manuales de referencia

### De Dunnicliff — Instrumentación geotécnica para el monitoreo del comportamiento en campo
| Capítulo | Título | Aplicación al monitoreo de presas |
|---------|-------|--------------------------------|
| **Cap. 1** | Instrumentación geotécnica: una visión general | Importancia del monitoreo de presas, consecuencias de falla |
| **Cap. 2** | Comportamiento de suelo y roca | Comportamiento de terraplén, filtración, erosión interna |
| **Cap. 3** | Beneficios del uso de instrumentación geotécnica | Seguridad, verificación de diseño, control operativo |
| **Cap. 4** | Enfoque sistemático para planificar programas de monitoreo | Planificación de 20 pasos específica para presas |
| **Cap. 9** | **Medición de presión de aguas subterráneas** | **Primario** — piezómetros en terraplén, cimentación, estribos |
| **Cap. 10** | Medición de tensión total en suelo | Células de presión de tierras en núcleo de terraplén |
| **Cap. 11** | Medición de cambio de tensión en roca | Monitoreo de tensión de roca de cimentación |
| **Cap. 12** | **Medición de deformación** | Extensómetros, asentamiento, inclinómetros, convergencia |
| **Cap. 13** | Medición de carga y deformación | Cargas de puntal, galgas de deformación en estructuras de concreto |
| **Cap. 17** | Instalación de instrumentos | Perforación en terraplenes, inyección de lechada, encaminamiento de cables |
| **Cap. 18** | Recolección, procesamiento, presentación, interpretación | Adquisición automatizada de datos (Cap. 18.1.2), umbrales de alarma |
| **Cap. 21** | **Presas de terraplén** | **Capítulo principal para presas** — presión de poros, deformación, filtración, ADAS |

### De Foundation Engineering: una referencia de dominio público (USACE / FHWA)
| Capítulo | Aplicación |
|---------|-------------|
| **Cap. 13** | Estabilidad de taludes — estabilidad de talud aguas arriba/abajo |
| **Cap. 10** | Presión de tierras lateral — estado de tensión de cimentación |
| **Cap. 14** | Mejora de suelos e instrumentación de cimentación — control de filtración y deformación |

### De Soil Mechanics & Geotechnical Engineering: una referencia de dominio público (USACE / FHWA)
| Capítulo | Aplicación |
|---------|-------------|
| **Cap. 5** | Permeabilidad — análisis de filtración, diseño de filtro |
| **Cap. 6** | Filtración y redes de flujo — superficie freática, sobrelevación |
| **Cap. 7** | Tensión efectiva y presión de poros — presión de poros en núcleos de presas |
| **Cap. 8** | Distribución de tensión en suelo — distribución de tensión de terraplén |
| **Cap. 9** | Consolidación — asentamiento de cimentaciones de terraplén |
| **Cap. 10** | Resistencia al cizalla — parámetros de tensión efectiva para núcleos |

### NCHRP Synthesis 89
| Tema | Aplicación |
|-------|-------------|
| Práctica de carreteras | Monitoreo de presas para presas de agencias de carreteras |

---

## Arreglo típico de instrumentos para monitoreo de presas

| Instrumento | Propósito | Capítulo Dunnicliff | Instrumento representativo |
|------------|---------|-------------------|------------------------|
| **Piezómetros multinivel** | Perfil de presión de poros a través del terraplén | Cap. 9, 21 | Cadenas de piezómetros VW, inalámbricos |
| **Piezómetros de tubo / pozo abierto** | Medición redundante de presión de poros | Cap. 9, 21 | Piezómetros de tubo vertical |
| **Vertederos en V / medidores de filtración** | Cuantificar flujo de filtración aguas abajo | Cap. 21 | Medición de caudal |
| **Extensómetros (de varilla/magnéticos)** | Deformación interna del terraplén | Cap. 12, 21 | Extensómetros de varilla, extensómetros magnéticos |
| **Inclinómetros** | Deformación lateral de estribos/cimentación | Cap. 12, 21 | Inclinómetros MEMS, arreglos IPI |
| **Monumentos de asentamiento superficial** | Asentamiento de cresta, alineación horizontal | Cap. 12, 21 | Placas de asentamiento, GNSS |
| **Células de presión de tierras** | Tensión en núcleo de terraplén | Cap. 10, 21 | Células de presión de tierras VW |
| **Crackmetros / jointmetros** | Monitoreo de grieta/junta en concreto | Cap. 12 | Crackmetros, jointmetros |
| **Péndulos (presas de concreto)** | Desplazamiento de cresta relativo a cimentación | Cap. 21 | Péndulos invertidos/inversos |
| **Vertederos / canaletas de filtración** | Cuantificar descarga de filtración | Cap. 21 | Vertederos en V |
| **Sensores de temperatura** | Hidratación de concreto, congelación-deshielo | Cap. 14 | Termistores, RTD |
| **malla inalámbrica** | Datos inalámbricos de todos los sensores | Cap. 8, 18, 21 | malla inalámbrica + retorno celular/satelital |
| **ADAS (adquisición automatizada de datos)** | Alarmas en tiempo real, reportes automatizados | Cap. 18.1.2, 21 | inalámbrico + plataforma en la nube |

---

## Directrices de instalación (de Dunnicliff Cap. 9, 10, 12, 17, 21)

### Instalación de piezómetro en terraplenes
- **Cadenas multinivel**: instalar durante la construcción en cada capa
- **Punta filtrante**: saturada, compatible con material del núcleo
- **Sellos**: bentonita sobre/bajo cada zona filtrante
- **Encaminamiento de cable**: protegido en conducto, con alivio de tensión en cada capa
- **Caja terminal**: Cap. 21.4.3 (sobre el nivel máximo de agua)

### Instalación de extensómetro
- **Profundidades de anclaje**: múltiples anclajes en elevaciones clave (cimentación, media altura, cerca de cresta)
- **Cabeza de referencia**: referencia estable fuera de la influencia de la presa
- **Lectura**: VW o eléctrica, accesible en cresta

### Medición de filtración
- **Vertederos en V**: pie aguas abajo, calibrados
- **Colectores de filtración**: drenes franceses con medición de caudal
- **Trazadores**: prueba de tinte para rutas de filtración

---

## Directrices de interpretación de datos (de Dunnicliff Cap. 18, 21)

| Parámetro | Rango normal | Nivel de alerta | Nivel crítico | Referencia |
|-----------|--------------|-------------|----------------|-----------|
| Relación de presión de poros (u/σ') | < 0,5 | > 0,6 | > 0,8 | Cap. 21 |
| Aumento de caudal de filtración | Línea base | 2× línea base | 5× línea base | Cap. 21 |
| Tasa de asentamiento de cresta | < 5 mm/año | > 20 mm/año | > 50 mm/año | Cap. 21 |
| Desplazamiento horizontal | < 10 mm/año | > 25 mm/año | > 50 mm/año | Cap. 21 |
| Apertura de crackmetro | < 0,5 mm | > 2 mm | > 5 mm | Cap. 13, 21 |

---

## Monitoreo automatizado (Dunnicliff Cap. 18.1.2, Cap. 21)

| Sistema | Función | Implementación |
|--------|----------|-------------------|
| **ADAS** | Adquisición automatizada de datos | inalámbrico + DT Link |
| **Umbrales de alarma** | Configurables por parámetro | tablero en la nube |
| **Validación de datos** | QA/QC automatizada | QA/QC integrada |
| **Reportes** | Reportes programados | reportes programados |
| **Acceso remoto** | Tablero basado en web | plataforma en la nube |

---

## Páginas relacionadas
- [Dunnicliff Capítulo 21](../reference-manuals/dunnicliff/chapter-14-applications.md)
- [GTI Doctor — Consulte sobre monitoreo de presas](../gti-doctor.md)

---

*Fuente: Compilado de Dunnicliff (616 fragmentos), Foundation Engineering (USACE/FHWA, dominio público), Soil Mechanics (USACE/FHWA, dominio público), NCHRP Synthesis 89 y manuales de referencia de campo.*

---

## Video destacado y recursos prácticos

<div class="video-container" style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; margin-bottom: 1rem;">
  <iframe src="https://www.youtube-nocookie.com/embed/tdxGnlsV65A" title="Dam Owner Academy: Seepage, Slope Stability & Seismic Issues" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border-radius: 6px;"></iframe>
</div>
<p><em>Video destacado (Asociación de Funcionarios Estatales de Seguridad de Presas - ASDSO): Academia para Propietarios de Presas — Filtración, estabilidad de taludes y problemas sísmicos: mecanismos críticos y monitoreo de campo.</em></p>

!!! tip "Recursos prácticos de campo complementarios de RST Instruments y Measurand (Terra Insights)"
    - **RST Instruments (@RSTgeotechnical):** [Lecturas iniciales de piezómetro de cuerda vibrante](https://www.youtube.com/watch?v=HJISt9or_Dw){ target="_blank" }  
      *Procedimiento estándar de verificación de línea base para piezómetros de cuerda vibrante antes de la instalación en terraplenes y cimentaciones de presas.*
    - **Measurand (@MeasurandVideos):** [Monitoreo de deflexión en tiempo real con ShapeArray](https://www.youtube.com/watch?v=518Mx-65rI0){ target="_blank" }  
      *Monitoreo continuo y automatizado de deformación de cresta y núcleo interno para presas de terraplén con ShapeArray.*
