---
lang: es
lang_alt: reference-manuals/geovadis/chapter-02-ai-computational-geomechanics/
---

# Inteligencia Artificial y Geomecánica Computacional

!!! abstract "Resumen de la Sesión"
    La Sesión 1 de *GeoVadis (GAIC 2025)* muestra la rápida convergencia entre la
    inteligencia basada en datos y las simulaciones numéricas basadas en la física dentro
    de la geotecnia. Los temas centrales incluyen la predicción de parámetros de
    compactación mediante redes neuronales artificiales (ANN), la micromecánica por el
    método de elementos discretos (DEM) de anclajes de placa y flujos granulares, la
    evaluación mediante aprendizaje automático de la licuefacción cíclica, las inversiones
    del parámetro de estado a partir de CPT y el modelado constitutivo termomecánico de
    arcillas.

---

## 1. Aprendizaje Automático para Geomateriales Granulares (H. Hunt, B. Indraratna, et al.)

### El cambio de paradigma en el modelado constitutivo
Las leyes constitutivas continuas tradicionales (Cam-Clay, Mohr-Coulomb, hipoplasticidad)
tienen dificultades para capturar fenómenos complejos a escala de grano —rotura de
partículas, anisotropía de fábrica, dependencia de la trayectoria de tensiones y
degradación cíclica— sin introducir un exceso de parámetros empíricos. Hunt, Indraratna y
coautores ofrecen una revisión crítica de los enfoques de aprendizaje automático (ML) en
mecánica granular:

```
    ┌───────────────────────────┐      ┌───────────────────────────┐
    │ Fenomenología continua    │      │ Micromecánica de grano    │
    │  • Cam-Clay / endurecim.  │      │  • Redes de contacto DEM  │
    │  • Calibración empírica   │      │  • Rotura de partículas   │
    └─────────────┬─────────────┘      └─────────────┬─────────────┘
                  │                                  │
                  ▼                                  ▼
    ┌──────────────────────────────────────────────────────────────┐
    │ Aprendizaje automático informado por la física (PIML / ANN)  │
    │  • Preserva conservación de energía y leyes termodinámicas   │
    │  • Incorpora morfología de grano por micro-CT y emisiones    │
    │    acústicas                                                 │
    │  • Generaliza entre trayectorias multiaxiales y ciclos       │
    └──────────────────────────────────────────────────────────────┘
```

### Hallazgos clave y limitaciones
1. **Escasez de datos y sobreajuste de dominio:** aunque los modelos alcanzan
   correlaciones elevadas ($R^2 > 0{,}95$) sobre conjuntos de datos de laboratorio
   concretos, su generalización a trayectorias de tensión de campo no ensayadas exige
   restricciones informadas por la física (por ejemplo, consistencia termodinámica,
   disipación plástica no negativa).
2. **Integración de la morfología del grano:** incorporar descriptores morfológicos 3D
   de micro-CT (esfericidad, redondez, rugosidad superficial) en redes convolucionales
   mejora notablemente la predicción de los ángulos de fricción en estado crítico
   ($\phi'_{cs}$).

---

## 2. Mecánica de Arrancamiento de Anclajes de Placa Horizontales Profundos mediante DEM (R.S. Sowmya, R. Gopika, T.K. Sudheesh)

### Profundidad de empotramiento y mecanismo de rotura
Los anclajes de placa horizontales profundos se emplean ampliamente en torres de
transmisión, sistemas de amarre offshore y muros de contención. Sowmya y colaboradores
utilizan modelado 3D de elementos discretos (DEM) para revelar el movimiento
micromecánico del suelo sobre los anclajes a distintas relaciones de empotramiento
($H/B$):

- **Comportamiento de anclaje somero ($H/B < 3$):** la superficie de rotura se propaga
  directamente hasta la superficie del terreno, con rotura general por corte y un
  levantamiento superficial significativo.
- **Comportamiento de anclaje profundo ($H/B \ge 5$):** se forman bandas de corte
  localizadas y un bulbo de compactación inmediatamente sobre la placa. La rotura está
  gobernada por expansión local de cavidad y efecto arco, no por una superficie de rotura
  que aflore.

### Factores de arrancamiento
El factor de arrancamiento $N_\gamma = Q_u / (\gamma A H)$ se estabiliza a gran
profundidad de empotramiento:

$$Q_u = A \cdot \left[ \gamma H N_\gamma + c' N_c \right]$$

Las visualizaciones DEM de la red de fuerzas de contacto revelan cadenas de fuerza
intensas que irradian diagonalmente desde los bordes del anclaje, transformando el
tirón de tracción en arcos de compresión de confinamiento lateral.

---

## 3. Predicción mediante ANN de Parámetros de Compactación de Suelos (H. Paneru, N.P. Bhandary)

### Optimización de los controles de compactación
Los ensayos Proctor estándar y modificado consumen mucho tiempo y mano de obra. Paneru y
Bhandary evalúan arquitecturas de perceptrón multicapa (MLP) para predecir el contenido
de humedad óptimo ($OMC$) y la densidad seca máxima ($MDD$) a partir de propiedades
índice básicas:
- **Variables de entrada:** límite líquido ($LL$), límite plástico ($PL$), índice de
  plasticidad ($PI$), fracción arcillosa ($CF$), fracción arenosa ($SF$) y peso
  específico ($G_s$).
- **Arquitectura del modelo:** retropropagación de Levenberg-Marquardt con
  regularización bayesiana.
- **Desempeño predictivo:** el modelo ANN alcanzó $R^2 = 0{,}93$ para $MDD$ y
  $R^2 = 0{,}91$ para $OMC$, lo que permite un cribado rápido de campo para terraplenes
  de carreteras y subrasantes.

---

## 4. Aprendizaje Automático para la Susceptibilidad a Licuefacción Cíclica (S. Sah, V. Bherde, U. Balunaini)

### Entrenamiento con datos triaxiales cíclicos
La evaluación del desencadenamiento de licuefacción bajo pulsos sísmicos irregulares se
apoya tradicionalmente en curvas de relación de tensiones cíclicas ($CSR$) frente a
número de ciclos ($N_L$). Sah y colaboradores entrenan clasificadores de bosque aleatorio
(RF) y máquinas de vectores de soporte (SVM) sobre extensos conjuntos de datos triaxiales
cíclicos:
- **Conjunto de características:** tensión efectiva media de confinamiento inicial
  ($\sigma'_{m0}$), relación de tensiones cíclicas ($CSR$), densidad relativa ($D_r$),
  contenido de finos ($FC$) y frecuencia de carga ($f$).
- **Relación de presión de agua de poro ($r_u$):** el modelo pronostica con precisión la
  transición desde la movilidad cíclica estable ($r_u < 0{,}6$) hasta la licuefacción
  desbocada y rápida ($r_u \to 1{,}0$).

---

## 5. Interpretación del Parámetro de Estado por CPT en Arena (B. Dalnayak, V. Singh, S. Chatterjee)

### Inversión del estado in-situ
El ensayo de penetración de cono (CPT) proporciona de forma continua la resistencia de
punta ($q_c$) y el rozamiento del manguito ($f_s$). Mediante análisis de elementos finitos
en grandes deformaciones (formulación ALE / CEL), Dalnayak y colaboradores simulan la
penetración estacionaria del cono normalizado de $60^\circ$ en arena para calibrar el
parámetro de estado ($\psi = e - e_c$):

$$Q_{p} = \frac{q_c - \sigma_{v0}}{\sigma'_{v0}} = k \cdot \exp(-m \cdot \psi)$$

donde $k$ y $m$ son coeficientes de calibración específicos de la arena. Este marco
numérico elimina la incertidumbre en la determinación de la densidad relativa in-situ y
de la resistencia al desencadenamiento de licuefacción sin necesidad de muestreo
inalterado por congelación.

---

## 6. Síntesis: Sinergias entre Mecánica Computacional y Monitoreo de Campo

| Modelo computacional / de IA | Problema geotécnico físico | Instrumentación de campo para calibración |
| :--- | :--- | :--- |
| **Modelos constitutivos neuronales / PIML** | Degradación cíclica de suelos de cimentación | Ensayos de columna resonante, arreglos sísmicos downhole |
| **Modelos DEM de arrancamiento de anclajes** | Arrancamiento de anclajes de placa / micropilotes | Células de carga calibradas, LVDT de desplazamiento de alta precisión |
| **Predictores ANN de compactación** | Compactación de subrasante y terraplenes | Densímetro nuclear, ensayo del cono de arena, ensayo de placa de carga |
| **Clasificadores ML de licuefacción** | Desencadenamiento de licuefacción sísmica | Arreglo de piezómetros (sobrepresión de poros $r_u = \Delta u / \sigma'_0$) |
| **Elementos finitos en grandes deformaciones (CPT)** | Perfilado del parámetro de estado ($\psi$) | Resistencia de punta de piezocono (CPTu) $q_t$, presión de poros $u_2$ |
