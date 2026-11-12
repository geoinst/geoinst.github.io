---
lang: es
lang_alt: reference-manuals/geovadis/chapter-05-foundations-deep-excavation/
---

# Cimentaciones, Excavaciones Profundas y Sistemas de Contención

!!! abstract "Resumen de la Sesión"
    La Sesión 4 de *GeoVadis (GAIC 2025)* abarca avances críticos en sistemas de
    cimentación, excavaciones profundas y estructuras de contención de tierras. Las
    contribuciones examinan el desempeño de radieres de pilotes bajo cargas combinadas
    vertical-lateral (V-H), los pilotes compuestos suelo-cemento, la estabilidad de
    trincheras en muros pantalla con paneles ampliados, el ensayo de carga estática
    bi-direccional (BDSLT), la mezcla profunda de suelos con inserciones de acero para
    taludes de excavación de 10 metros y el comportamiento térmico de arreglos de
    micropilotes energéticos.

---

## 1. Radieres de Pilotes bajo Carga Combinada V-H (A. Garg, V.A. Sawant, S. Mehndiratta)

### Mecánica de interacción por elementos finitos 3D
Las estructuras esbeltas, las torres de puente y las chaquetas de aerogeneradores imponen
cargas verticales ($V$), horizontales ($H$) y momentos ($M$) concurrentes y severos sobre
los radieres de pilotes. Garg y colaboradores realizan simulaciones acopladas 3D
elastoplásticas por elementos finitos para analizar el reparto de carga entre la base del
radier y el grupo de pilotes:
- **Movilización del contacto radier-suelo:** bajo cargas puramente verticales, el radier
  transmite directamente al suelo superficial entre el $30\%$ y el $45\%$ de las cargas
  gravitatorias totales. Bajo corte lateral elevado ($H/V > 0{,}2$), el rozamiento de la
  base del radier se moviliza rápidamente, derivando hasta el $40\%$ de la demanda
  horizontal antes de que se movilice una deflexión lateral significativa de los pilotes.
- **Ablandamiento p-y del grupo de pilotes:** el desplazamiento lateral cíclico induce
  plasticidad del suelo en los primeros $3D - 5D$ de profundidad del pilote, reduciendo la
  rigidez lateral del grupo entre un $25\%$ y un $35\%$.
- **Recomendaciones de diseño:** optimizar la distribución de longitudes de pilote
  (pilotes centrales más largos reductores de asentamiento, pilotes perimetrales más
  rígidos resistentes al corte) minimiza el asentamiento diferencial del radier y la
  fisuración perimetral.

---

## 2. Pilotes Compuestos Suelo-Cemento (S. Koga, K. Watanabe, T. Naito, N. Tsuchiya)

### Concepto y modelado en centrifugadora
Los pilotes compuestos suelo-cemento consisten en un núcleo rígido de hormigón prefabricado
o tubo de acero insertado concéntricamente en una columna exterior de suelo-cemento
mezclado en profundidad. Koga y Watanabe emplean ensayos en centrifugadora geotécnica
($50g$) y modelos a escala real 1g para esclarecer los mecanismos de transferencia de
carga vertical y lateral:

```
            Carga vertical P
                  │
                  ▼
        ┌───────────────────┐
        │ Núcleo de         │ ◄─── Núcleo de alta rigidez axial (Ec)
        │ hormigón / acero  │
        │                   │
        ├─┬───────────────┬─┤
        │ │ Suelo-cemento │ │ ◄─── Envase de columna ampliada (E_sc, D_col)
        │ │ envolvente    │ │      Amplía el perímetro de apoyo y el área de punta
        ├─┼───────────────┼─┤
        │ │               │ │
        │ │ Resistencia   │ │ ◄─── Alta movilización por rozamiento en la
        │ │ al corte del  │ │      interfaz rugosa suelo-cemento / terreno
        │ │ suelo         │ │
        └─┴───────────────┴─┘
```

### Conclusiones mecánicas clave
1. **Transferencia de carga vertical:** la tensión axial es absorbida inicialmente por el
   núcleo interior de alto módulo y se transfiere progresivamente a la envuelta de
   suelo-cemento mediante el rozamiento en la interfaz núcleo-lechada. El diámetro
   ampliado de la base ($D_{col} = 2 - 3 \times D_{core}$) incrementa el área de apoyo de
   punta entre un $400\%$ y un $900\%$.
2. **Resistencia lateral:** bajo cargas horizontales, la columna exterior de
   suelo-cemento moviliza una elevada resistencia pasiva en los estratos superiores,
   reduciendo la deflexión lateral en cabeza de pilote en más del $50\%$ frente a un
   pilote prefabricado desnudo.

---

## 3. Estabilidad de Trinchera en Muros Pantalla con Paneles Ampliados (A. Iwata, K. Watanabe, T. Watanabe)

### Muros pantalla con paneles ampliados en T y en cruz
Para resistir momentos flectores masivos en excavaciones urbanas ultraprofundas, los
muros pantalla incorporan a menudo paneles con alas ampliadas (paneles en T, paneles
cruciformes). Sin embargo, el aumento de la superficie de la trinchera eleva el riesgo de
colapso de la zanja de lodos durante la excavación:
- **Mantenimiento de la presión de lodos:** los análisis de equilibrio límite 3D y por
  elementos finitos indican que la carga hidrostática de lodos debe superar el nivel
  freático en al menos $1{,}5\,\text{m}$ para evitar desprendimientos plásticos
  localizados hacia el interior en las esquinas reentrantes.
- **Lodos poliméricos frente a bentoníticos:** los lodos poliméricos con modificadores
  viscoelásticos mantienen una estabilidad reológica superior y una continuidad de la
  torta de filtración a través de lentes variables de arena y grava, evitando la pérdida
  de lodo y el colapso.

---

## 4. Mezcla Profunda de Suelos con Inserción de Acero para Soporte de Excavación de 10 m (Z.W. He, J. Si, K.W. Leong)

### Sistema de contención para emplazamientos urbanos restringidos
He y colaboradores presentan un caso de diseño y monitoreo de campo exitoso para una
excavación de sótano de 10 metros de profundidad en arcilla urbana sensible:
- **Arquitectura del sistema:** columnas solapadas de suelo-cemento mezclado en
  profundidad de triple eje ($D = 850\,\text{mm}$), reforzadas con perfiles metálicos
  H insertados (método SMW) en centros de columna alternos.
- **Anclaje por tirantes:** dos niveles de anclajes al terreno pretensados, perforados a
  través del muro compuesto, proporcionan sujeción lateral.
- **Desempeño en campo:** las medidas inclinométricas registraron una deflexión lateral
  máxima del muro de contención de solo $18\,\text{mm}$ ($< 0{,}2\% H$), holgadamente
  dentro del límite de servicio admisible para la protección de edificios colindantes.

---

## 5. Ensayo de Carga Estática Bi-Direccional de Pilotes (BDSLT) (A.K. Chakraborti, S.K. Golchha, A. Uppadhyay)

### Ensayo con celda Osterberg (BDSLT) en pilotes perforados de gran capacidad
Los ensayos de carga estática convencionales descendentes sobre pilotes perforados
profundos ($Q_{ult} > 25\,000\,\text{kN}$) exigen enormes lastres de reacción o pilotes
de anclaje a tracción, con graves problemas de seguridad y coste. Chakraborti y
colaboradores evalúan ensayos en pilotes perforados profundos mediante celdas Osterberg
(celdas O) expandibles hidráulicamente, embebidas en la punta del pilote:
- **Principio de autoequilibrio:** la celda O empuja hacia arriba contra el rozamiento
  del fuste superior mientras empuja simultáneamente hacia abajo contra la resistencia de
  punta y el rozamiento del fuste inferior.
- **Curva equivalente de carga en cabeza:** mediante el método de síntesis de
  Schmertmann / celda O, las curvas carga-movimiento ascendente y descendente se combinan
  en una curva equivalente convencional de carga en cabeza:
  $$S_{top}(Q) = S_{up}(Q_{shaft}) + S_{elastic\_shortening}$$
- **Instrumentación con galgas de deformación:** las *sister bars* multinivel instaladas
  a lo largo del fuste delatan con precisión la degradación del rozamiento unitario
  ($f_s$) a través de estratos de arcilla y lutita.

---

## 6. Resumen de Instrumentación para Excavaciones y Cimentaciones

| Estructura subsuperficial | Sensor diagnóstico primario | Sensor secundario | Parámetro ingenieril clave |
| :--- | :--- | :--- | :--- |
| **Radier de pilotes** | Células de presión de tierras (base del radier) | Galgas de cuerda vibratoria en cabeza de pilote | Relación de reparto de carga radier/pilote, presión de contacto |
| **Muro pantalla (perfil H / barrette)** | Tubo inclinométrico (dentro del muro) | Células de carga en cabezas de anclaje | Perfil de deflexión lateral, pérdida de carga de anclaje |
| **Respuesta del terreno en excavación profunda** | Extensómetros magnéticos multipunto | Inclinómetros de superficie en estructuras colindantes | Perfil de asentamiento vertical subsuperficial del terreno |
| **Ensayo de pilote BDSLT / celda O** | Transductores de desplazamiento a través de la celda | Sister bars multinivel en la jaula | Carrera ascendente/descendente, rozamiento unitario del fuste $f_s$ |
| **Mezcla profunda (muro SMW)** | Inclinómetros en perfiles H de acero | Piezómetros de cuerda vibratoria tras el muro | Deflexión del muro, descenso del nivel freático |
