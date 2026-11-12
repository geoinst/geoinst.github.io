---
lang: es
lang_alt: reference-manuals/cfem/chapter-25-instrumentation-monitoring/
---
# Capítulo 25 — Instrumentación y Monitoreo Geotécnicos (Resumen)

*Fuente: CFEM 2022 (4.ª Edición), Capítulo 25, por Pierre Choquet, Dr.-Eng., P. Eng.
Esta página es un resumen original con una **sección de referencias elaborada**; no es
una reproducción del capítulo original protegido por derechos de autor.*

El diseño geotécnico conlleva incertidumbre. Esa incertidumbre se evalúa durante la
construcción y la operación mediante instrumentos. El Capítulo 25 examina los
instrumentos utilizados habitualmente para monitorear el comportamiento a corto y
largo plazo del terreno que sostiene las estructuras construidas por el ser humano,
junto con los sistemas de recolección y adquisición de datos que los respaldan.

El capítulo se organiza en torno a **seis parámetros medidos**, y este resumen sigue
esa estructura antes de pasar a la mitad *autónoma* del tema: cómo se toman, transmiten
y presentan las lecturas sin presencia humana en campo.

---

## 25.1 — Introducción

Los seis parámetros principales de monitoreo y los instrumentos que los miden:

| Parámetro | Instrumentos típicos |
|---|---|
| **Presión de aguas subterráneas** | Piezómetros (de tubo abierto, de cuerda vibratoria, neumáticos, hincados, totalmente inyectados) |
| **Desplazamiento** (superficial y en profundidad; x, y, z; relativo o absoluto) | Extensómetros, medidores de asentamiento, inclinómetros, medidores de pendiente, métodos geodésicos |
| **Deformación** (en superficies del terreno o de la estructura, o embebida) | Galgas de deformación |
| **Carga** (del elemento estructural → terreno) | Células de carga (anclajes de retención, pilotes de prueba) |
| **Presión total** (contacto terreno–estructura) | Células hidráulicas de presión total |
| **Temperatura** (superficial o perfil con la profundidad) | Termistores |

El capítulo también aborda los **métodos geodésicos** — estaciones totales, nivelación,
GPS RTK diferencial y métodos más recientes como LiDAR, InSAR terrestre e InSAR
satelital — porque se emplean junto con la instrumentación geotécnica y estructural.

---

## 25.2 — Fuentes de información *(elaboradas)*

> **Esta es la sección que convierte al capítulo en una herramienta de consulta.** Más
> que una bibliografía simple, §25.2 es una lista de lectura *guiada*, organizada por
> tipo de documento. A continuación, cada entrada se agrupa y se anota con qué es y
> por qué importa.

### 25.2.1 — El libro de texto fundamental

- ***Geotechnical Instrumentation for Monitoring Field Performance*** — **John
  Dunnicliff (1993)**, Wiley, 577 págs. — la obra de referencia de la disciplina,
  universalmente conocida como el **«Libro Rojo»**. El Capítulo 25 lo considera la
  fuente más reconocida del campo.
- **Las columnas trimestrales de Dunnicliff** en *Geotechnical News* (CGS) — 93
  columnas, indexadas y consultables en la sección pública del
  [sitio web de CGS](https://www.cgs.ca/instrumentation_news.html). Un archivo
  profesional vivo que prolonga el libro.

### 25.2.2 — Libros de texto y volúmenes principales de directrices

| Referencia | Cobertura |
|---|---|
| **De Rubertis, K. (Ed.), 2018** — *Monitoring Dam Performance: Instrumentation and Measurements*, ASCE, 442 págs. | Fuente principal del capítulo sobre **propiedades metrológicas** (§25.5) y monitoreo geodésico; referencia de seguridad de presas ASCE/USSD |
| **Sharon, R. & Eberhardt, E. (Eds.), 2020** — *Guidelines for Slope Performance Monitoring*, CSIRO Publishing / CRC Press, 331 págs. | Filosofía y práctica de monitoreo específicas de taludes |
| **Stark, Oommen & Ning, 2021** — *Remote Sensing for Monitoring Embankments, Dams, and Slopes*, ASCE GSP 322, 114 págs. | Estado de la práctica en teledetección (InSAR, LiDAR, fotogrametría) |
| **ICE Manual of Geotechnical Engineering** (Burland et al., 2012) — Cap. 94 *Principles of Geotechnical Monitoring* (16 págs.) y Cap. 95 *Types of Geotechnical Instrumentation and Their Usage* (26 págs.) | Un segundo tratamiento canónico; el Cap. 94 también cubre prácticas contractuales |
| **Walker & Awange, 2020** — *Surveying for Civil and Mine Engineers*, Springer, 411 págs. | Métodos geodésicos/topográficos (§25.17) |
| **Glisic & Inaudi, 2007** — *Fibre Optic Methods for Structural Health Monitoring*, Wiley, 281 págs. | Referencia sobre **sensado de fibra óptica** (§25.4.4) |
| **Ferretti et al., 2007** — *InSAR Principles: Guidelines for SAR Interferometry Processing*, ESA TM-19 | Principios detrás de **InSAR satelital** (§25.17.5) |
| **Chartered Institution of Civil Engineering Surveyors, 2017** — *Client Guide to Instrumentation and Monitoring*, Survey Liaison Group, Londres, 28 págs. | Guía de contratación y alcance para el promotor |

### 25.2.3 — Normas

**Subcomité ASTM D18.23 (Instrumentación de Campo)** — métodos de ensayo y prácticas
normalizadas estadounidenses que rigen directamente instrumentos específicos:

| Norma | Tema |
|---|---|
| **D4403-20** | Práctica normalizada para extensómetros empleados en roca |
| **D6230-13** | Método de ensayo normalizado para monitorear movimientos del terreno con inclinómetros de sonda |
| **D6598-19** | Guía normalizada para instalar y operar puntos de asentamiento destinados a monitorear deformaciones verticales |
| **D7299-12** | Práctica normalizada para verificar el desempeño de una sonda de inclinómetro vertical |
| **D7764-12** | Práctica normalizada para ensayos de aceptación previos a la instalación de piezómetros de cuerda vibratoria |

**Comité Técnico ISO 182 / WG2 — serie *ISO 18674*** («Geotechnical investigation
and testing — Geotechnical monitoring by field instrumentation»), su contraparte
internacional, publicada por partes:

| Parte | Tema | Estado al momento de escribir |
|---|---|---|
| **ISO 18674-1:2015** | Parte 1: Reglas generales | Publicada |
| **ISO 18674-2:2016** | Parte 2: Mediciones a lo largo de una línea — extensómetros | Publicada |
| **ISO 18674-3:2017** | Parte 3: Mediciones a través de una línea — inclinómetros | Publicada |
| **ISO 18674-4** | Parte 4: Medición de la presión de agua en poros — piezómetros | Publicada |
| **ISO 18674-5** | Parte 5: Medición de cambios de esfuerzo mediante células de presión total | Publicada |
| Parte 6 / 7 / 8 / 9 | Medidores hidráulicos de asentamiento / galgas de deformación / células de carga / instrumentos geodésicos de monitoreo | **Previstas** |

**DIN (Deutsches Institut für Normung)** — normas de vibración citadas para §25.19:

- **DIN 45669-1:1995** — Medición de vibraciones y choques mecánicos
- **DIN 4150-1:2001** — Vibraciones estructurales, Parte 1: predicción de parámetros de vibración
- **DIN 4150-2:1999** — Exposición humana a vibraciones en edificios *(en revisión)*
- **DIN 4150-3:2016** — Vibraciones en edificios, Parte 3: efectos sobre las estructuras

**Otras normas y guías de organismos:**

- **Transportation Research Board (TRB), 2008** — *Use of Inclinometers for
  Geotechnical Instrumentation on Transportation Projects* (Machan & Bennett) — una
  nota técnica exhaustiva sobre la práctica de los inclinómetros.
- **USGS, 2008** — *Instrumentation Guidelines for the Advanced National Seismic
  System (ANSS)*, Open-File Report 2008–1262, 48 págs. — fuente de la **clasificación
  de sistemas de movimiento sísmico intenso de clase A–D** usada en §25.18.
- **COSMOS, 2016** — *Guidelines and General Considerations for Strong-Motion
  Instrumentation of Tall Buildings* — guía de movimiento sísmico intenso para
  edificios altos.
- **US Bureau of Mines RI 8507, 1980** (Siskind et al.) — *Structure Response and
  Damage by Ground Vibration from Mine Blasting* — la referencia clásica sobre
  vibraciones por voladuras mineras que sustenta §25.19.

### 25.2.4 — Referencias regulatorias y manuales (seguridad de presas)

La lista del capítulo de **guías descargables de instrumentación para seguridad de
presas** — los manuales regulatorios ante los que, en última instancia, responde un
programa de monitoreo:

| Manual | Editor / año | Extensión |
|---|---|---|
| **EM 1110-2-1908** — *Instrumentation of Embankment Dams and Levees* | Cuerpo de Ingenieros del Ejército de EE. UU., 2020 | 290 págs. |
| **EM 1110-2-4300** — *Instrumentation for Concrete Structures* | Cuerpo de Ingenieros del Ejército de EE. UU., 1987 *(en revisión)* | 306 págs. |
| *Embankment Dam Instrumentation Manual* (Bartholomew, Murray & Goins) | U.S. Bureau of Reclamation, 1987 *(en revisión)* | 269 págs. |
| *Concrete Dam Instrumentation Manual* (Bartholomew & Haverland) | U.S. Bureau of Reclamation, 1987 | 153 págs. |
| *Engineering Guidelines for the Evaluation of Hydropower Projects*, Cap. 9 *Instrumentation and Monitoring* (2005); Cap. 14 *Dam Safety Performance Monitoring Program* (2017) | FERC | 86 / 188 págs. |
| **Boletín ICOLD 158** — *Dam Surveillance Guide* (2018) | ICOLD | 109 págs. |
| **7 documentos técnicos** sobre desarrollo e implementación de programas de monitoreo de seguridad de presas (2008–2020) | U.S. Society on Dams (USSD) | serie |
| *Manual de Mecánica de Suelos: Instrumentación y Monitoreo del Comportamiento de Obras Hidráulicas* (2012) | Comisión Nacional del Agua, México | 322 págs. |

> **Referencia cruzada.** Este sitio resume varios de ellos directamente; véanse
> [Monitoreo del Desempeño de Presas](../monitoring-dam-performance/index.md) (ASCE MOP-135)
> y [Seguridad de Presas de Relaves](../tailings-dam-safety/index.md) (Boletín ICOLD 194).

### 25.2.5 — Series de simposios

La investigación exhaustiva sobre instrumentación se ha publicado en los simposios
**«Field Measurements in Geomechanics» (FMGM)**: Zúrich 1983, Kobe 1987, Oslo 1991,
Bérgamo 1995, Singapur 1999, Oslo 2003, Boston 2007, Berlín 2011, Sídney 2015 y
Río de Janeiro 2018 — organizados por voluntarios (principalmente académicos) y
publicados comercialmente. El siguiente simposio estaba previsto en Londres 2022
bajo el patrocinio de ISSMGE. En estas actas se documentan en detalle los
**casos de estudio** de instrumentación.

---

## 25.3 — Factores humanos

El Capítulo 25 presta atención temprana a los **factores humanos**, apoyándose en tres
capítulos de Dunnicliff: planificación sistemática, especificaciones para contratación
y disposiciones contractuales. Su argumento conserva plena vigencia: los instrumentos
mecánicos/hidráulicos simples funcionaban bien en manos de ingenieros diligentes con
un propósito claro; con el avance tecnológico, «un número creciente de programas de
instrumentación ha quedado en manos de personas con motivación y sentido del propósito
incompletos», y muchas fallas pasaron a ser **fallas del matrimonio entre instrumento
y persona**, no de los instrumentos. Escrito hace décadas, el capítulo señala que
el punto es *«si no aún más cierto»* hoy, dado el ritmo más acelerado de la construcción.

---

## 25.4 — Principios de medición

Los instrumentos geotécnicos se basan en principios **eléctricos, mecánicos,
hidráulicos y neumáticos**. Los dos principios *eléctricos* dominantes:

- **Cuerda vibratoria (VW)** — con mucho, el más extendido. Un alambre de acero
  pretensado (normalmente de **0,25 mm** de diámetro y 5–15 cm de longitud) se excita
  mediante dos bobinas electromagnéticas; el alambre resuena a una frecuencia
  (**1.000–2.000 Hz**) que varía con la tensión. Su robustez y estabilidad a largo plazo
  quedaron demostradas en presas de concreto europeas después de la Segunda Guerra
  Mundial; hoy abarca presión de poros, asentamiento, extensión/compresión, deformación,
  carga, esfuerzo y presión de tierras. Con frecuencia incorpora temperatura mediante
  un termistor sellado.
- **Acelerómetros MEMS** — hacia 2010 sustituyeron a los acelerómetros servoasistidos
  y a los sensores electrolíticos de inclinación para **pendiente e inclinación**, con
  metrología igual o mejor, además de mayor robustez y mejor comportamiento frente a
  desviaciones térmicas. Sus circuitos pueden incluir un microcontrolador y un ADC,
  dando **salida digital** sobre un bus RS-485.
- **Instrumentos de salida digital** (familia relacionada) — sensores piezorresistivos
  de nivel de agua con salida 4–20 mA, sondas multiparámetro de calidad de agua y
  cadenas digitales de termistores, que usan **RS-485** o el protocolo **SDI-12**
  desarrollado por USGS.
- **Sensado de fibra óptica** — inmune a rayos y transitorios eléctricos; disponible
  como sensores puntuales, **semidistribuidos** (rejillas de Bragg) y **totalmente
  distribuidos** (dispersión Brillouin, deformación/temperatura cada metro en cables
  de hasta **30 km**).

---

## 25.5 — Propiedades metrológicas

Dado que los instrumentos suelen ser **irremplazables** una vez instalados, se exige
una metrología excelente. Las propiedades (según De Rubertis, 2018), con valores VW
típicos:

| Propiedad | Significado | Valor típico VW |
|---|---|---|
| **Resolución** | Cambio más pequeño que puede distinguirse | Muchas veces más fina que la exactitud |
| **Exactitud** | Concordancia con un patrón aceptable | **±0,1 % F.S.** (trazable al NIST) |
| **Precisión** (error aleatorio) | Cercanía a la media de lecturas repetidas | **±0,025 % F.S.** |
| **Repetibilidad** | Concordancia entre mediciones consecutivas | Igual que la precisión (VW) |
| **Linealidad** (no linealidad) | Desviación respecto de una línea recta | **0,1–0,5 % F.S.** |
| **Sesgo** | Valor indicado medio frente al valor real | Igual que la exactitud (en la práctica) |
| **Estabilidad a largo plazo** | Deriva de salida durante años con entrada constante | Establecida por décadas de casos de estudio |

La idea clave del capítulo para el monitoreo: **normalmente importa el cambio, no el
valor absoluto**, lo que hace que la *precisión* sea más importante que la exactitud.

---

## 25.6–25.7 — Estático frente a dinámico; la cadena de instrumentación

El **monitoreo estático** domina la geotecnia (respuesta lenta del terreno), mientras
que el **dinámico** cubre sismos, voladuras y vibraciones de maquinaria. La terminología
se aclara a lo largo de la cadena: **sensor → transductor → transmisor → instrumento**,
distinción que el capítulo emplea de forma coherente en secciones posteriores.

---

## 25.8 — Presión de aguas subterráneas (piezómetros)

La sección de instrumentos más extensa del capítulo abarca:

- **Piezómetros Casagrande de tubo abierto** — referencia simple y robusta.
- **Transductores eléctricos de presión** — de cuerda vibratoria y otros tipos.
- **Piezómetro VW dentro de un tubo abierto Casagrande** — instalación híbrida.
- **Instalación por zonas** en un sondeo — aislamiento de una zona de medición con
  sellos de lechada.
- **Piezómetros hincados** — despliegue rápido cuando el terreno lo permite.
- **Piezómetros totalmente inyectados** — método (referencias de Contreras, Mikkelsen,
  McKenna, Vaughan y Penman en la lista) que se ha vuelto estándar en muchas
  instalaciones de presas de terraplén.
- **Presión de poros negativa / succión** — la medición más difícil, con técnica propia.

---

## 25.9 — Pendiente e inclinación

- **Medidores de pendiente (*tiltmeters*)** — para estructuras e inclinaciones locales.
- **Inclinómetros** — caballo de batalla para el movimiento lateral del terreno, leídos
  a intervalos fijos (p. ej., 0,5 m / 2 ft) con sistemas de sonda.
- **Inclinómetros in situ y ShapeArrays** — perfiles instalados permanentemente; el
  capítulo ofrece **criterios de selección** para cada uno (§25.9.3.1–25.9.3.2).

---

## 25.10 — Asentamiento, levantamiento y asentamiento diferencial

Instrumentos cubiertos: **extensómetros de sonda**, **extensómetros de sondeo**,
**células hidráulicas de asentamiento**, **células hidráulicas diferenciales de
asentamiento** e **inclinómetros horizontales**; en conjunto abarcan desde el
asentamiento superficial hasta el levantamiento profundo.

---

## 25.11–25.14 — Grietas, deformación/carga, presión de tierras, temperatura

- **Apertura de grietas y juntas** — medidores de grietas, medidores de juntas,
  extensómetros de suelo.
- **Deformación y carga** — galgas de deformación, células de carga (concreto, acero,
  anclajes).
- **Presión de tierras** — células de presión total, células de presión hincadas.
- **Temperatura** — termistores y cadenas de termistores (también parámetro de
  referencia para la compensación de muchos otros instrumentos).

---

## 25.15 — Adquisición automática de datos y telemetría

Los **ADAS (Sistemas Automatizados de Adquisición de Datos)** son dispositivos
desplegables en campo que recolectan y almacenan mediciones de muchos sensores por
cable o radio y, opcionalmente, las transmiten a un ordenador remoto sin intervención
humana. Funciones requeridas:

- **Gestión de señales** para tipos mixtos de sensores (VW, MEMS digital, 4–20 mA,
  analógico 0–5/0–10 V, digital RS-485/SDI-12).
- **Alimentación por batería** (alcalina, de litio o de plomo-ácido + solar).
- **Almacenamiento de datos a bordo**.
- **Comunicaciones de bajo caudal** — radio, módem celular o satélite, según calendario.
- **Alarma/control local opcional**.
- Un continuo desde **registradores autónomos de 1 canal hasta redes de más de 1.000 canales**.

El capítulo distingue un **registrador de datos** (un dispositivo que reúne todas o
casi todas esas funciones) de un **ADAS** (un registrador más elaborado que además puede
formar una **red**, gestionar estados de alarma y **controlar dispositivos externos** —
SMS, accionamiento de válvulas, sirena/luz intermitente). *Nótese la tendencia del
mercado:* los registradores pequeños incorporan hoy funciones que antes solo existían
en redes ADAS.

**Registradores pequeños** (§25.15.1) — 1–10 canales, bajo consumo, baterías «D» de
3,6 V con **autonomía ≥1 año**, rango de operación **−40 °C a +80 °C** y, cada vez más,
radio de baja potencia sin licencia (unos pocos km en terreno abierto, ~1 km en ciudad).

**Redes ADAS integradas** (§25.15.2) — dos arquitecturas:

1. **Pocos sistemas centrales de adquisición + tendidos largos de cable** — desventajas:
   costo del cable, zanjas/conductos, **riesgo de transitorios por rayos cerca de la
   superficie**, resistencia añadida y riesgo de errores en empalmes. La recomendación
   del capítulo es explícita: **mantener cortos los cables de sensor** y añadir más
   puntos de adquisición.
2. **Redes de radio de concentrador a nodo** con pequeños registradores con radio
   cercanos a los instrumentos — configuración en **estrella** o red **mallada**
   (*mesh*), donde los registradores se retransmiten entre sí hasta una **pasarela**
   y de ahí a la oficina por celular, satélite, Wi-Fi o LAN.

---

## 25.16 — Software para gestión, visualización, alarmas e informes de datos

La mayoría de registradores/ADAS generan **archivos de valores delimitados**
(`*.csv`, `*.dat`) con una columna de marca de tiempo y una columna por canal; a menudo
contienen lecturas **crudas**, que la mayoría de los usuarios prefiere conservar. Las
hojas de cálculo bastan para trabajos pequeños; los proyectos grandes o prolongados
requieren software dedicado, que suele ofrecer:

- **Panel de control** (visión general del proyecto, valores en tiempo real, sensores en alarma)
- **Visualización en tiempo real** con código de color (**Verde: OK / Amarillo: umbral / Rojo: alarma**)
- **Curvas de tendencia** (lectura frente al tiempo, con desplazamiento y zoom)
- **Comprobación de alarmas** con **SMS/correo** automáticos
- **Variables virtuales** (calculadas a partir de uno o más sensores)
- **Controles de acceso** (perfiles de usuario)
- **Convertidor de archivos** (importación desde la mayoría de sistemas de registro, hojas de cálculo y registros manuales)
- **Gráficos de correlación (XY)** (p. ej., nivel piezométrico frente a lluvia; deformación frente a temperatura)
- **Vistas de perfil** (inclinómetros in situ, ShapeArrays)
- **Informes automatizados** según calendario
- **Visualización en teléfono/tableta** y **alojamiento en la nube**
- **Soporte multilingüe**
- **Importación de datos geodésicos (estación total) e InSAR**
- **Geolocalización SIG / Google Earth**

---

## 25.17 — Mediciones geodésicas

Métodos de levantamiento terrestre que detectan movimiento horizontal y vertical sobre
una **red de control topográfico** de hitos o puntos instalados en la estructura:

- **Estaciones totales y niveles** — instrumentos topográficos centrales; robótica,
  medición sin reflector y reconocimiento automático de dianas permiten operación
  **automatizada**. Exactitud típica: **1–5 segundos de arco** en ángulo;
  **1–1,5 mm + 1–2 ppm** en distancia.
- **Láseres rotativos** — para alineación y rasante.
- **Escáneres láser** — captura 3D densa (véase Adamson et al., 2019, en la bibliografía).
- **GNSS** — posicionamiento absoluto.
- **InSAR satelital** — comparación de imágenes SAR repetidas; bandas X, C y L;
  **tamaño de píxel 0,25–20 m** (habitualmente 1–3 m), **precisión 1–20 mm**;
  **>50.000 puntos por km²** sobre áreas que superan cientos de km²; medición a lo
  largo del haz de radar (≈50–70° respecto de la horizontal), por lo que el
  desplazamiento vertical real exige trigonometría; revisita de **unos pocos días a
  14+ días**. Las constelaciones ascendente y descendente aportan información horizontal.
- **InSAR terrestre** — interferometría de radar terrestre para cobertura local.
- **Fotogrametría con UAV** — levantamiento aéreo para deformación (véase Stafford et al., 2019).

---

## 25.18–25.19 — Movimiento sísmico intenso y vibraciones

- **Acelerógrafos de movimiento sísmico intenso** — acelerómetro 3D + registrador,
  que capturan la **aceleración pico de partícula** (en *g*) y la historia temporal.
  Buena práctica: una unidad en **campo libre**, otra en el **punto más alto** de la
  estructura y otras en posiciones intermedias, **sincronizadas por GPS** cuando se
  usan varias unidades. Clasificadas **A–D** según **USGS (2008)** para la red ANSS;
  Canadá opera la **CNSN** (más de 100 sismógrafos de alta ganancia y más de 60
  acelerógrafos).
- **Monitores de vibración** — sensor triaxial de velocidad (**geófono**) + registrador,
  que mide la **velocidad de partícula en cm/s** (voladuras, tráfico, vibración
  ambiental; regulada por la serie DIN 4150).

---

## 25.20 — Presentación de los datos de instrumentación

El argumento final del capítulo: **todos los datos deben compartir una misma marca de
tiempo**, y esa marca es el **único vínculo** entre los datos de monitoreo y las
actividades constructivas (que descargan y luego recargan el terreno). También deben
registrarse los factores ambientales — **temperatura y lluvia** — porque la descarga
puede abrir grietas que luego aprovecha el agua de lluvia (Figura 25-23). Integrar
los datos de monitoreo con las actividades constructivas y los factores ambientales
**sigue siendo un reto para la mayoría de los programas comerciales de graficación**,
y todo programa debe **asignar recursos suficientes** para que los datos se presenten
e interpreten sin ambigüedad.

---

## Puntos clave

- **Seis parámetros, una disciplina.** Presión de aguas subterráneas, desplazamiento,
  deformación, carga, presión total y temperatura; cada uno con sus propias familias
  de instrumentos.
- **§25.2 es el activo más reutilizable del capítulo**: un mapa guiado de las normas
  (ASTM D18.23, ISO 18674, DIN 4150), los libros de texto (Dunnicliff, De Rubertis,
  Sharon & Eberhardt, Hoek), los manuales regulatorios (USACE, Reclamation, FERC,
  ICOLD) y los simposios que sustentan la práctica del monitoreo.
- **La cuerda vibratoria y los MEMS dominan** la medición eléctrica; el sensado de
  fibra óptica es la tercera familia emergente.
- **La precisión supera a la exactitud** en monitoreo, porque lo que importa es el
  *cambio*.
- **Mantenga cortos los cables de sensor y distribuya la adquisición**: los tendidos
  largos en superficie propician daños por rayos y errores de empalme.
- **La automatización es un espectro**, desde un registrador de 1 canal hasta una red
  ADAS de más de 1.000 canales con alarmas y control.
- **Marque todo con tiempo y registre temperatura y lluvia**; de lo contrario, los
  datos no pueden interpretarse frente a la actividad constructiva.
- **Los factores humanos deciden el éxito.** El matrimonio instrumento–persona importa
  tanto como el instrumento mismo.

---

## Lista completa de referencias

*Reproducida como bibliografía del capítulo, para consulta. Las normas se revisan en
sus propios ciclos: verifique siempre la edición vigente.*

**Adamson, D., Alfaro, M., Blatz, J., Bannister, K.** — Construction and Post-Construction Deformations of an MSE Wall using Terrestrial Laser Scanning. *Geo St John's 2019*, Sociedad Geotécnica Canadiense.

**Anderson, C., Vessely, M., Christiansen, C., 2020** — Advances in Unstable Slope Instrumentation and Monitoring. TRB / NCHRP, National Academies, Washington DC.

**Burland, J., Chapman, T., Skinner, H., Brown, M. (Eds.), 2012** — *ICE Manual of Geotechnical Engineering*, Cap. 94 (Dunnicliff, Marr & Standing) y Cap. 95 (Dunnicliff). ICE Publishing, Londres.

**Choquet, P., Juneau, F., Debreuille, P.J., Bessette, J., 1999** — Reliability, Long-term Stability and Gage Performance of Vibrating Wire Sensors with Reference to Case Histories. *Proc. 5th Int. Symp. on Field Measurements in Geomechanics*, Singapur.

**Choquet, P., Taylor, R.M., 2014** — Automatic Data Acquisition Systems (ADAS) for Dam and Levee Monitoring. *Geo-Congress 2014*, ASCE, 180–191.

**Client guide to instrumentation and monitoring**, 2017 — Chartered Institution of Civil Engineering Surveyors for the Survey Liaison Group, Londres.

**Contreras, I.A., Grosser, A.T., VerStrate, R.H., 2007** — The use of the fully-grouted method for piezometer installation. *Proc. 7th Int. Symp. on Field Measurements in Geomechanics*, Boston. *(Véanse también las actualizaciones de 2008, 2011, 2012 y 2020 de los mismos autores.)*

**COSMOS, 2016** — *Guidelines and General Considerations for Strong-Motion Instrumentation of Tall Buildings*.

**De Rubertis, K. (Ed.), 2018** — *Monitoring Dam Performance — Instrumentation and Measurements*, ASCE, 442 págs.

**DIN** — DIN 45669-1:1995; DIN 4150-1:2001; DIN 4150-2:1999 (en revisión); DIN 4150-3:2016.

**Dunnicliff, J., 1993** — *Geotechnical Instrumentation for Monitoring Field Performance*, Wiley, 577 págs.

**Dunnicliff, J., 1994** — Contract Practices for Geotechnical Instrumentation. *Geotechnical News*, Vol. 12, N.º 3.

**Elwood, D.E.Y. & Martin, C.D., 2016** — Ground response of closely spaced twin tunnels constructed in heavily overconsolidated soils. *Tunnelling and Underground Space Technology*, 51, 226–237.

**Ferretti, A., Monti-Guarnieri, A., Prati, C., Rocca, F., 2007** — *InSAR Principles: Guidelines for SAR Interferometry Processing and Interpretation*. ESA TM-19.

**Glisic, B., Inaudi, D., 2007** — *Fibre Optic Methods for Structural Health Monitoring*, Wiley, 281 págs.

**McKenna, G.T., 1995** — Grouted-in Installation of Piezometers in Boreholes. *Canadian Geotechnical Journal* 32, 355–363.

**McRae, J.B., Simmonds, T., 1991** — Long-term Stability of Vibrating-wire Instruments: One Manufacturer's Perspective. *Proc. 3rd Int. Symp. on Field Measurements in Geomechanics*, Vol. 1:283–293, Balkema.

**Mikkelsen, P.E., 2002** — Cement-Bentonite Grout Backfill for Borehole Instruments. *Geotechnical News*, Vol. 20, N.º 4, 38–42.

**Mikkelsen, P.E. & Green, E.G., 2003** — Piezometers in Fully Grouted Boreholes. *6th Int. Symp. on Field Measurements in Geomechanics*, Oslo.

**Pantony, B., Fraser, S., Sinacori, J., 2021** — Satellite InSAR for Geotechnical and Structural Monitoring. *Canadian Geotechnique*, Vol. 2, N.º 1.

**Penman, A.D.M., 2002** — Measurement of Pore Water Pressures in Embankment Dams. *Geotechnical News*, Vol. 20, N.º 4, 43–49.

**Pieraccini, M., Miccinesi, L., 2019** — Ground-Based Radar Interferometry: A Bibliographic Review. *Remote Sensing* 11(9).

**Richards, D.J., Clark, J., Powrie, W., Heymann, G., 2007** — Performance of push-in pressure cells in overconsolidated clay. *Geotechnical Engineering* 160, GE1, 31–41.

**Richards, D.J., Powrie, W., Roscoe, H., Clark, J., 2007** — Pore water pressure and horizontal stress changes during construction of a contiguous bored pile multi-propped retaining wall in Lower Cretaceous clays. *Géotechnique* 57(2), 197–205.

**Ridley, A.M., 2015** — Soil suction — what it is and how to successfully measure it. *9th Symp. on Field Measurements in Geomechanics*, Australian Centre for Geomechanics, Perth, 27–46.

**Schuyler, J.N. & Gularte, F., 2000** — Automated Tiltmeter Monitoring of Bridge Response to Compaction Grouting. *SPIE 7th Annual Int. Symp. on Smart Structures and Materials*, Newport Beach, CA.

**Sellers, J.B., 1994** — Load Cell Calibrations. *Geotechnical News*, Vol. 12, N.º 3.

**Sellers, J.B., Taylor, R., 2008** — MEMS Basics. *Geotechnical News*, Vol. 26, N.º 1.

**Sharon, R., Eberhardt, E. (Eds.), 2020** — *Guidelines for Slope Performance Monitoring*, CSIRO Publishing / CRC Press, 331 págs.

**Siskind, D.E., Stagg, M.S., Kopp, J.W., Dowding, C.H., 1980** — *Structure Response and Damage by Ground Vibration from Mine Blasting*. US Bureau of Mines RI 8507.

**Soe Moe, K.W., Cruden, D.M., Martin, C.D., Lewycky, D., Lach, P.R., 2009** — Mechanisms and kinematics of river valley landslides in Edmonton. *Annual Canadian Geotechnical Conference, GeoHalifax*.

**Stafford, D.M.J. et al., 2019** — Preliminary deformation detection of high-fill sections along the Inuvik-Tuktoyaktuk Highway using UAV photogrammetry. *Geo St. John's 2019*, CGS.

**Stark, T.D., Oommen, T., Ning, Z., 2021** — *Remote Sensing for Monitoring Embankments, Dams, and Slopes: Recent Advances*, ASCE GSP 322, 114 págs.

**Tedd, P., Powell, J.J., Charles, J.A., Uglow, I.M., 1990** — In situ measurement of earth pressures using push-in spade-shaped pressure cells — 10 years' experience. *Geotechnical Instrumentation in Practice*, Thomas Telford, Londres, 701–715.

**U.S. Geological Survey, 2008** — *Instrumentation Guidelines for the Advanced National Seismic System*. Open-File Report 2008–1262, 48 págs.

**Vaughan, P.R., 1969** — A Note on Sealing Piezometers in Boreholes. *Géotechnique* 19(3), 405–413.

**Walker, J. & Awange, J.L., 2020** — *Surveying for Civil and Mine Engineers*, Springer, 411 págs.

> **Agradecimiento (capítulo original).** El autor agradece a los proveedores de
> instrumentación que facilitaron las figuras y fotografías de la publicación original.
> Esas figuras **no** se reproducen aquí.
