---
lang: es
lang_alt: applications/tunnels/
---

# Instrumentación de túneles

## Objetivo

Monitorear el movimiento del terreno alrededor de la excavación del túnel, la convergencia de los revestimientos y los cambios de presión de poros durante la construcción — protegiendo tanto la sección transversal del túnel como las estructuras adyacentes superficiales.

---

## Referencias completas por capítulo de los manuales de referencia

### De Dunnicliff — Instrumentación geotécnica para el monitoreo del comportamiento en campo
| Capítulo | Título | Aplicación a la instrumentación de túneles |
|---------|-------|----------------------------------------|
| **Cap. 1** | Instrumentación geotécnica: una visión general | Importancia del monitoreo de túneles, consecuencias de colapso |
| **Cap. 2** | Comportamiento de suelo y roca | Comportamiento del macizo rocoso, terreno apretante, reventón de roca |
| **Cap. 3** | Beneficios del uso de instrumentación geotécnica | Verificación de diseño, seguridad de construcción, contractual |
| **Cap. 4** | Enfoque sistemático para planificar programas de monitoreo | Planificación de 20 pasos para proyectos de túnel |
| **Cap. 8** | Transductores de instrumentación y adquisición de datos | Sensores de convergencia, sistemas automatizados |
| **Cap. 9** | Medición de presión de aguas subterráneas | Presiones de desagüe, piezómetros en frente de túnel |
| **Cap. 12** | **Medición de deformación** | **Primario** — convergencia, extensómetros, inclinómetros |
| **Cap. 13** | Medición de carga y deformación | Cargas de perno de roca, tensión de revestimiento, indicadores |
| **Cap. 17** | Instalación de instrumentos | Específico de túnel: perforación desde el túnel, espacio limitado |
| **Cap. 18** | Recolección, procesamiento, presentación, interpretación | Monitoreo de convergencia en tiempo real, sistemas de alarma |
| **Cap. 23** | **Excavaciones subterráneas** | **Capítulo principal para túneles** — convergencia, pernos de roca, aguas subterráneas, presión de frente |

### De Foundation Engineering: una referencia de dominio público (USACE / FHWA)
| Capítulo | Aplicación |
|---------|-------------|
| **Cap. 10** | Presión de tierras lateral — diseño de revestimiento de túnel |
| **Cap. 12** | Muros de tablestaca y excavaciones entibadas — soporte de portales y zanja cubierta |
| **Cap. 13** | Estabilidad de taludes — taludes de portal, asentamiento superficial |

### De Soil Mechanics & Geotechnical Engineering: una referencia de dominio público (USACE / FHWA)
| Capítulo | Aplicación |
|---------|-------------|
| **Cap. 6** | Filtración y redes de flujo — entrada de aguas subterráneas, presión de frente |
| **Cap. 7** | Tensión efectiva y presión de poros — respuesta del terreno alrededor de aperturas |
| **Cap. 10** | Resistencia al cizalla — parámetros de resistencia de macizo rocoso y suelo |

---

## Arreglo típico de instrumentos para instrumentación de túneles

| Instrumento | Propósito | Capítulo Dunnicliff | Instrumento representativo |
|------------|---------|-------------------|------------------------|
| **Arreglos de convergencia / extensómetro de cinta** | Monitorear cierre de sección transversal de túnel | Cap. 12, 23 | Extensómetros de cinta, arreglos de convergencia |
| **Extensómetros multipunto de sondeo (MPBX)** | Desplazamiento del macizo rocoso sobre la corona | Cap. 12, 23 | Extensómetros MPBX, inalámbricos |
| **Inclinómetros (superficiales/de portal)** | Detectar vaguada de asentamiento superficial | Cap. 12, 23 | Inclinómetros MEMS, arreglos IPI |
| **Piezómetros** | Presiones de desagüe cerca del frente de túnel | Cap. 9, 23 | Piezómetros VW, inalámbricos |
| **Células de carga de perno de roca** | Monitoreo de carga de anclaje/perno | Cap. 13, 23 | Células de carga VW, galgas de deformación |
| **Medidores de convergencia** | Convergencia de revestimiento en tiempo real | Cap. 12, 23 | Medidores de convergencia, inalámbricos |
| **Galgas de deformación de perno de roca** | Monitoreo de carga de perno | Cap. 13 | Galgas de deformación VW, inalámbricas |
| **Células de presión (NATM)** | Presión del terreno sobre revestimiento | Cap. 10, 23 | Células de presión VW |
| **Crackmetros / jointmetros** | Apertura de junta de segmento | Cap. 12, 23 | Crackmetros, jointmetros |
| **Inclinómetro (escudo TBM)** | Articulación/alineación de TBM | Cap. 12 | Sensores de inclinación MEMS |
| **radio mallada inalámbrica** | Datos del túnel a la pasarela superficial | Cap. 8, 18 | malla inalámbrica + pasarela superficial |

---

## Directrices de instalación (de Dunnicliff Cap. 12, 17, 23)

### Monitoreo de convergencia
- **Tipos de arreglo**: extensómetro de cinta, medidor de convergencia, MPBX
- **Ubicaciones**: corona, líneas de muelle, invert
- **Frecuencia**: diaria (excavación), semanal (construcción), mensual (operación)

### Instalación de extensómetro (MPBX)
- **Profundidades de anclaje**: múltiples anclajes a diversas profundidades de recubrimiento de roca
- **Instalación**: desde corona de túnel/perforación desde superficie
- **Cabeza de referencia**: ubicación estable fuera de la zona de influencia del túnel

### Instalación de piezómetro
- **Ubicaciones**: adelante del frente, en el frente, detrás del revestimiento
- **Tipos**: piezómetros VW para lectura remota
- **Monitoreo de desagüe**: aguas arriba/abajo del túnel

### Monitoreo de perno de roca
- **Células de carga**: instaladas en cabeza de perno
- **Galgas de deformación**: adheridas al vástago del perno
- **Indicadores**: para elongación de perno largo

---

## Directrices de interpretación de datos (de Dunnicliff Cap. 18, 23)

| Parámetro | Rango normal | Nivel de alerta | Nivel crítico | Referencia |
|-----------|--------------|-------------|----------------|-----------|
| Tasa de convergencia | < 2 mm/día | > 5 mm/día | > 10 mm/día | Cap. 23 |
| Tasa de asentamiento de corona | < 2 mm/día | > 5 mm/día | > 10 mm/día | Cap. 23 |
| Pérdida de carga de perno de roca | < 10% | > 20% | > 30% | Cap. 13 |
| Cambio de presión de poros | Línea base | 2× línea base | > valor de diseño | Cap. 9, 23 |
| Tasa de pérdida de carga de perno de roca | < 5%/mes | > 10%/mes | > 20%/mes | Cap. 13 |

---

## Monitoreo automatizado para túneles (Dunnicliff Cap. 18, Cap. 23)

| Sistema | Función | Implementación |
|--------|----------|-------------------|
| **Convergencia en tiempo real** | Monitoreo continuo de corona/líneas de muelle | sensores de convergencia inalámbricos |
| **Monitoreo de presión de frente** | Presión de escudo TBM, desagüe | piezómetros inalámbricos |
| **Monitoreo de perno de roca** | Carga + deformación de perno | células de carga VW + galgas de deformación |
| **Alarmas automatizadas** | Excedencia de umbral | plataforma en la nube |
| **Integración de datos TBM** | Presión de escudo, articulación | malla inalámbrica + interfaz TBM |

---

## Páginas relacionadas
- [Dunnicliff Capítulo 23](../reference-manuals/dunnicliff/chapter-14-applications.md)
- [GTI Doctor — Consulte sobre monitoreo de túneles](../gti-doctor.md)

---

*Fuente: Compilado de Dunnicliff (616 fragmentos), Foundation Engineering (USACE/FHWA, dominio público), Soil Mechanics (USACE/FHWA, dominio público), NCHRP Synthesis 89 y manuales de referencia de campo.*
