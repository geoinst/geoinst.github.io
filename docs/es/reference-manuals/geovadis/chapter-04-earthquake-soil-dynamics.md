---
lang: es
lang_alt: reference-manuals/geovadis/chapter-04-earthquake-soil-dynamics/
---

# Ingeniería Geotécnica Sísmica y Dinámica de Suelos

!!! abstract "Resumen de la Sesión"
    La Sesión 3 de *GeoVadis (GAIC 2025)* presenta avances destacados en ingeniería
    sísmica, plasticidad cíclica de suelos y mitigación de vibraciones. Las áreas de
    atención incluyen el tratamiento sostenible con biopolímeros frente a la licuefacción
    cíclica, la cuantificación del índice de empaquetamiento en suelos granulares, las
    barreras de onda con mezclas arena-caucho (SRM), el aislamiento sísmico mediante
    radieres de pilotes desconectados y geoceldas, y el monitoreo de campo de vibraciones
    inducidas por voladuras.

---

## 1. Mitigación con Biopolímeros de la Licuefacción de Arenas Limosas (N.V. Dasari, M.D. Tellam, K.K. Gonavaram)

### Alternativa ecológica de estabilización de suelos
La inyección química y la estabilización con cemento conllevan una huella de carbono
considerable y riesgos de contaminación de aguas subterráneas. Dasari y colaboradores
investigan el **quitosano** natural (un biopolímero derivado de la quitina de los
caparazones de crustáceos) como estabilizador de suelos respetuoso con el medio ambiente
para mitigar la licuefacción en arenas limosas sueltas ($FC = 15\% - 25\%$):
- **Mecanismo de puenteo por hidrogel:** tras la mezcla y el curado, el quitosano forma
  filamentos viscosos de hidrogel de biopolímero que recubren las superficies de cuarzo
  granular y puentean las gargantas porosas entre partículas.
- **Relación de resistencia cíclica ($CRR_{15}$):** los ensayos triaxiales cíclicos con
  control de deformación revelan que tratar arena limosa suelta con $1{,}0\%$ de
  quitosano incrementa la relación de resistencia cíclica ($CRR$) hasta un 180 %.
- **Retardo de la presión de agua de poro:** la tasa de generación de sobrepresión de
  poro ($\Delta u / \sigma'_0$) se ralentiza drásticamente, evitando la pérdida
  catastrófica de confinamiento efectivo durante los ciclos sísmicos.

```
       Arena limosa suelta sin tratar        Arena tratada con biopolímero de quitosano
       ┌───────────────────────────┐            ┌───────────────────────────┐
       │   ○       ○       ○       │            │   ○───────○═══════○       │
       │     ○       ○       ○     │   ─────►   │   │  Biopolímero  │       │
       │   ○       ○       ○       │            │   ○═══Hidrogel════○       │
       │ (Contactos granulares     │            │ (Redes de unión            │
       │  sueltos)                 │            │  trabadas)                │
       └─────────────┬─────────────┘            └─────────────┬─────────────┘
                     │                                        │
             Sacudimiento sísmico                    Sacudimiento sísmico
                     ▼                                        ▼
       ┌───────────────────────────┐            ┌───────────────────────────┐
       │ Pico rápido de Δu (ru ► 1)│            │ Δu amortiguada (ru < 0,40)│
       │ Rotura por licuefacción   │            │ Integridad elastoplástica  │
       └───────────────────────────┘            └───────────────────────────┘
```

---

## 2. Índice de Empaquetamiento para la Resistencia a Licuefacción (M.U. Rehman, R.K. Kandasami, S. Banerjee)

### Más allá de la densidad relativa ($D_r$)
La densidad relativa ($D_r$) suele correlacionarse mal con la resistencia a licuefacción
de arenas con angularidad de grano variable y distribuciones granulométricas amplias.
Rehman y colaboradores proponen un **índice de empaquetamiento ($I_p$)** informado por la
micromecánica:

$$I_p = \frac{e_{max} - e}{e_{max} - e_{min}} \cdot \left( \frac{d_{50}}{d_{10}} \right)^{\alpha} \cdot \Phi_s$$

donde $\Phi_s$ es la esfericidad de la partícula y $\alpha$ un coeficiente de
granulometría.
- **Verificación por micro-CT:** la tomografía 3D de rayos X demuestra que arenas con
  idéntico $D_r$ pero menor esfericidad forman números de coordinación ($Z_c$) más altos
  y arcos de fuerza de contacto más rígidos.
- **Correlación con $CRR$:** el índice de empaquetamiento logra una correlación unificada
  con la relación de resistencia cíclica tanto para arenas limpias uniformes como para
  arenas limosas bien graduadas ($R^2 = 0{,}94$).

---

## 3. Apantallamiento de Vibraciones mediante Zanjas con Mezcla Arena-Caucho (SRM) (A. Boominathan, J.S. Dhanya, et al.)

### Mecánica dinámica de barreras de onda
Las vibraciones transmitidas por el terreno inducidas por hincado de pilotes por impacto,
líneas ferroviarias de alta velocidad y maquinaria pesada provocan resonancia estructural
y fatiga acústica en edificios urbanos colindantes. Boominathan y colaboradores ensayan
zanjas de apantallamiento de ondas abiertas frente a rellenas con mezclas arena-caucho
(SRM):
- **Desajuste de impedancia:** los trozos de neumático triturado mezclados con arena
  gruesa ($30/70$ en peso) crean una relación de desajuste de impedancia acústica
  ($\rho v_s$) inferior a $0{,}35$ respecto al subsuelo virgen.
- **Atenuación de ondas de Rayleigh:** los análisis numéricos 3D por elementos finitos y
  los ensayos de campo experimentales revelan que una zanja SRM de profundidad
  normalizada $H / \lambda_R \ge 0{,}75$ atenúa la amplitud de la onda de Rayleigh hasta
  un 68 % en la zona de apantallamiento pasivo.
- **Estabilidad geotécnica:** a diferencia de las zanjas abiertas, que exigen entibación o
  colapsan con niveles freáticos altos, las zanjas SRM mantienen paredes verticales
  autoportantes mientras filtran la vibración.

---

## 4. Desempeño Sísmico de Radieres de Pilotes Desconectados (A.K. Suman, J.S. Rajeswari)

### Aislamiento sísmico mediante capa de almohadillado
En regiones de alta sismicidad, conectar rígidamente los pilotes al radier de cimentación
concentra enormes fuerzas de corte inerciales y momentos flectores en las cabezas de los
pilotes:
- **Diseño con almohadilla desconectada:** se interpone una capa compactada de grava con
  geogrid ($0{,}5\,\text{m} - 1{,}0\,\text{m}$ de espesor) entre la cara inferior del
  radier y las cabezas de los pilotes.
- **Desacoplamiento inercial:** los ensayos dinámicos en centrifugadora y las
  simulaciones por elementos finitos confirman que la capa de almohadilla desliza
  plásticamente durante las aceleraciones espectrales de pico, acotando la transferencia
  máxima de corte hacia los pilotes.
- **Reducción de momentos:** los momentos flectores en cabeza de pilote se reducen entre
  un $50\%$ y un $75\%$ frente a radieres rígidamente conectados, eliminando las roturas
  frágiles por corte en la unión radier-pilote y manteniendo un control de asentamiento
  adecuado bajo cargas gravitatorias estáticas.

---

## 5. Monitoreo de Vibraciones Inducidas por Voladuras (A. Anil, T. Naskar, A. Boominathan, A. Joseph)

### Firmas dinámicas de demolición
Durante la demolición controlada por voladura de chimeneas industriales pesadas y torres
de carbón, la energía explosiva genera ondas de choque transitorias que se propagan por
estratos geológicos complejos:
- **Sensores triaxiales de velocidad:** geófonos ortogonales (transversal, vertical,
  radial) registran la velocidad pico de partícula ($PPV$) y los espectros de frecuencia.
- **Ley de atenuación USBM:** los datos de campo se ajustan a la ecuación de distancia
  escalada:
  $$PPV = K \cdot \left( \frac{R}{\sqrt{Q}} \right)^{-B}$$
  donde $Q$ es la carga explosiva por retardo (kg) y $R$ la distancia de alejamiento (m).
- **Control de vibraciones:** la telemetría de arreglo en tiempo real verifica que las
  frecuencias de vibración se mantienen por encima de las frecuencias naturales
  estructurales ($> 20\,\text{Hz}$), evitando la resonancia en naves industriales
  colindantes.

---

## 6. Matriz de Instrumentación para Dinámica de Suelos

| Fenómeno dinámico | Sensor primario de monitoreo | Instrumento complementario | Parámetro de salida |
| :--- | :--- | :--- | :--- |
| **Desencadenamiento de licuefacción sísmica** | Piezómetro de cuerda vibratoria de alta frecuencia | Par de acelerómetros downhole | $\Delta u$ dinámica, deformación de corte cíclica $\gamma_{cyc}$ |
| **Verificación de barrera de vibraciones** | Geófonos triaxiales de superficie ($4{,}5\,\text{Hz}$) | Sismógrafo digital | Velocidad pico de partícula ($PPV$), frecuencia FFT |
| **Radier de pilotes desconectado** | Células dinámicas de presión de tierras | Sister bars en punta de pilote | Tensión de contacto del radier, transferencia de carga axial del pilote |
| **Atenuación por hincado de pilotes** | Acelerómetros piezoeléctricos | Vibrómetro láser Doppler | Aceleración pico de vibración del terreno ($a_{max}$) |
| **Velocidad de onda de corte subsuperficial** | Geófono downhole / sonda cross-hole | Registrador de suspensión P-S | Velocidad de onda de corte $V_s$, módulo de pequeña deformación $G_{max}$ |
