---
lang: es
lang_alt: reference-manuals/geovadis-vol2/chapter-05-transportation-geotechnics/
---

# Geotecnia del Transporte

!!! abstract "Resumen de la Sesión"
    La Sesión 10 de *GeoVadis (GAIC 2025)* investiga los exigentes desafíos geotécnicos de la infraestructura vial y ferroviaria. Los temas centrales abarcan los muros de Suelo Mecánicamente Estabilizado (MSE) espalda con espalda bajo carga ferroviaria cíclica, las rejillas de caucho reciclado de bandas transportadoras de desecho para controlar la degradación del balasto, el modelado dinámico 3D tren-vía-subrasante, las subrasantes expansivas de pavimento estabilizadas con geoceldas, los terraplenes ligeros de geoespuma EPS y las respuestas estructurales del pavimento ante cargas por eje de vehículos eléctricos.

---

## 1. Muros MSE Espalda con Espalda bajo Carga Ferroviaria Pesada (S. Attara, B. Umashankar)

### Terraplenes de Aproximación con Espacio Restringido
En corredores de transporte estrechos y rampas de aproximación a puentes, los muros de contención se construyen espalda con espalda con capas de refuerzo de georrejilla solapadas o conectadas. Attara y Umashankar analizan el comportamiento dinámico de muros MSE espalda con espalda sometidos a carga ferroviaria cíclica ($P_{axle} = 250\,\text{kN}$):
- **Refuerzo Solapado frente a Conectado:** Cuando la distancia entre paramentos ($W$) es reducida ($W/H < 1.4$), conectar directamente las capas de georrejilla opuestas impide el abombamiento exterior del paramento y reduce el desplazamiento lateral máximo del muro en más del $40\%$ frente a láminas solapadas sin conectar.
- **Empuje Dinámico de Tierras Lateral:** El paso de ruedas a alta velocidad genera picos transitorios de presión dinámica de tierras que se atenúan exponencialmente con la profundidad. Las deformaciones de tracción máximas de la georrejilla se concentran en la zona superior de $0.3H$ inmediatamente bajo la losa de vía.

```
       Geometría de Muro MSE Espalda con Espalda bajo Sobrecarga Ferroviaria Cíclica
       ┌────────────────────────────────────────────────────────┐
       │   Vías Férreas y Cargas por Eje de Tren de Alta Velocidad│
       │   ══════════════════════════════════════════════════   │
       │   ┌────────────────────────────────────────────────┐   │
       ├───┴────────────────────────────────────────────────┴───┤
       │◄── Paramento 1  Relleno Granular Compactado  Paramento 2─►│
       ││ ════════════════════════════════════════════════════ ││
       ││ Capas de Georrejilla Continuas Conectadas             ││
       ││ ════════════════════════════════════════════════════ ││
       ││ (Deslizamiento Lateral Nulo; Deflexión Acotada)       ││
       ││ ════════════════════════════════════════════════════ ││
       ├───┬────────────────────────────────────────────────┬───┤
       │   │ Lecho de Cimentación de Suelo In Situ           │   │
       └───┴────────────────────────────────────────────────┴───┘
```

---

## 2. Rejillas de Caucho de Bandas Transportadoras de Desecho en Vías con Balasto (S. Hettiyahandi, B. Indraratna, T. Ngo, Y. Qi y cols.)

### Economía Circular en el Mantenimiento de Vías de Alta Velocidad
La rotura del balasto y los asentamientos representan más del $50\%$ de los presupuestos mundiales de mantenimiento de vías. El grupo de investigación del Prof. Indraratna desarrolla rejillas de caucho perforadas revalorizadas a partir de bandas transportadoras industriales al final de su vida útil:
- **Disipación de Energía:** Colocadas bajo la capa de balasto, la elevada relación de amortiguamiento y la resiliencia de la rejilla de caucho absorben las ondas de choque generadas por las irregularidades rueda-carril.
- **Reducción de la Degradación del Balasto:** Ensayos triaxiales cíclicos a gran escala ($500,000$ ciclos a $f = 15\,\text{Hz}$) demuestran que las rejillas de caucho reducen el Índice de Rotura de Balasto ($BBI$) entre un $45\%$ y un $50\%$ frente al balasto sin reforzar.
- **Módulo Resiliente de la Vía ($M_R$):** La capa compuesta amortigua la aceleración cíclica de la vía preservando su elasticidad, lo que reduce significativamente la frecuencia de bateo del balasto.

---

## 3. Estabilización con Geoceldas de Subrasantes Expansivas de Pavimento (S. Srivastava, B. Umashankar, P.K. Mahopatra y cols.)

### Control del Agrietamiento Diferencial por Hinchamiento-Retracción
Los pavimentos construidos sobre suelos arcillosos negros expansivos de alta plasticidad sufren levantamientos diferenciales estacionales severos, fisuración longitudinal y fatiga en malla de cocodrilo. Srivastava y cols. investigan colchones de confinamiento 3D con geoceldas instalados en la interfaz subrasante-base:
- **Confinamiento Celular Integral:** Los alveolos de la geocelda confinan el árido granular, generando elevadas tensiones de aro localizadas que transforman las cargas verticales de rueda en distribuciones horizontales amplias de tensiones.
- **Relación de Beneficio por Tráfico ($TBR$):** Ensayos cíclicos con placa de carga y modelado por elementos finitos muestran que el refuerzo con geoceldas incrementa la Relación de Beneficio por Tráfico ($TBR$) en $2.5 - 3.8$, permitiendo reducir un $30\%$ el espesor de la capa asfáltica y suprimiendo por completo el ahuellamiento superficial durante las estaciones húmedo-seco.

---

## 4. Terraplenes Ligeros de Geoespuma EPS sobre Arcillas Ultrablandas (V.V. Butle, G.S. Parvathi, A. Mandal, V. Srinivasan)

### Asentamiento de Consolidación Nulo sobre Lodos Costeros
Construir terraplenes de relleno convencionales ($18 - 20\,\text{kN/m}^3$) sobre arcillas costeras profundas induce asentamientos de consolidación colosales e inestabilidad global del talud. Butle y cols. evalúan bloques de geoespuma de poliestireno expandido (EPS) ultraligeros ($\gamma \approx 0.15 - 0.25\,\text{kN/m}^3$):
- **Compensación de la Carga Gravitatoria:** Sustituir $3\,\text{m}$ de relleno de suelo por geoespuma EPS reduce la presión total de sobrecarga en más del $90\%$, eliminando los asentamientos de consolidación primaria y secundaria.
- **Comportamiento Dinámico Ferroviario / Vial:** Las simulaciones por elementos finitos confirman que las losas de reparto de carga de hormigón armado sobre los bloques de EPS acotan las deformaciones de compresión cíclicas dentro de límites elásticos ($\epsilon < 1\%$), garantizando durabilidad a fatiga a largo plazo.

---

## 5. Demandas Estructurales del Pavimento frente a Vehículos Eléctricos (P. Chaudhary, S. Saride)

### Impacto de las Baterías Pesadas en la Longevidad del Pavimento
Los vehículos eléctricos (VE) incorporan paquetes de baterías pesados que incrementan el peso en vacío entre un $20\%$ y un $35\%$ frente a vehículos equivalentes de motor de combustión interna (MCI):
- **Desplazamiento de los Espectros de Carga por Eje:** Chaudhary y Saride analizan las relaciones de daño de pavimento con datos de simulador de vehículos pesados y modelado viscoelástico Kenlayer.
- **Daño por Fatiga y Ahuellamiento:** La flota de VE más pesada incrementa las deformaciones de tracción del asfalto ascendentes ($\epsilon_t$) y las deformaciones de compresión de la subrasante ($\epsilon_v$), acelerando las velocidades de ahuellamiento de la subrasante entre un $28\%$ y un $42\%$.
- **Recomendaciones de Diseño:** Los códigos de diseño normalizados deben adoptar factores revisados de Eje Simple Equivalente (ESAL) para camiones y especificar ligantes modificados con polímeros o intercapas geosintéticas para preservar la vida útil del pavimento.

---

## 6. Lista de Verificación de Instrumentación en Geotecnia del Transporte

| Activo de Transporte | Sensor Estructural Primario | Sensor Dinámico / de Tráfico | Métrica Clave de Desempeño Monitorizada |
| :--- | :--- | :--- | :--- |
| **Muro MSE Espalda con Espalda** | Camisas de Inclinómetro de Alta Precisión | Células de Presión de Tierras Dinámicas | Deflexión lateral del muro, empuje horizontal dinámico |
| **Vía Férrea con Balasto**| Células de Carga bajo Durmiente | Acelerómetros Triaxiales Multieje | Tensión de contacto dinámica del durmiente, vibración de vía ($a_{rms}$) |
| **Subrasante Vial con Geoceldas**| Células de Presión de Suelo en Subrasante | Transductores de Desplazamiento en Huella de Rueda (LVDT)| Distribución de tensión vertical en subrasante, profundidad de ahuellamiento |
| **Terraplén de Geoespuma EPS** | Extensómetros Magnéticos Multiprofundidad | Células de Presión de Tierras bajo Losa | Asentamiento de la arcilla de cimentación, deformación elástica de la geoespuma |
| **Sección de Pavimento para VE Pesados**| Galgas de Deformación en Asfalto (Transversal / Longitudinal)| Deflectómetros Multiprofundidad de Pavimento (MDD) | Deformación de tracción ascendente $\epsilon_t$, deflexión resiliente |
