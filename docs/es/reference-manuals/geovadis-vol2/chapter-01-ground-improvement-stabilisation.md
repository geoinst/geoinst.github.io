---
lang: es
lang_alt: reference-manuals/geovadis-vol2/chapter-01-ground-improvement-stabilisation/
---

# Mejoramiento de Suelos y Estabilización Química

!!! abstract "Resumen de la Sesión"
    La Sesión 6 de *GeoVadis (GAIC 2025)* aborda el mejoramiento moderno de suelos, la estabilización química y la remediación biogeoquímica de suelos. Las contribuciones más destacadas exploran el bombeo de lodo y la mitigación de la fluidización de la subrasante bajo tráfico ferroviario de carga pesada, los terraplenes apoyados sobre columnas de suelo geopolimérico, los nanotubos de carbono para prevenir la licuefacción, las cartas de diseño de precompresión no lineal con drenes verticales y la precipitación de calcita inducida por microorganismos (MICP).

---

## 1. Mitigación de la Fluidización de la Subrasante bajo Carga Ferroviaria Cíclica (B-H. Xu, C. Rujikiatkamjorn, B. Indraratna y cols.)

### El dilema del bombeo de lodo y la fluidización de la subrasante
Bajo tráfico ferroviario de alta velocidad y de carga pesada (cargas por eje $\ge 30\,\text{toneladas}$), las tensiones cíclicas repetidas generan elevadas presiones de agua de poros excedentes ($\Delta u$) en las arcillas blandas saturadas de la subrasante. Cuando la tensión efectiva se aproxima a cero ($\sigma' \to 0$), las partículas finas de arcilla se desprenden y forman una suspensión fluidificada de suelo y agua que asciende bombeada a través de los huecos del balasto suprayacente, provocando una degradación severa de la geometría de la vía, asentamientos diferenciales y ensuciamiento del balasto:

```
        Cargas Cíclicas Elevadas por Eje de Tren (30 - 35 toneladas)
                          │
                          ▼
        ┌───────────────────────────────────┐
        │ Capas de Balasto y Subbalasto     │
        ├───────────────────────────────────┤
        │ Arcilla Blanda Saturada Subrasante│
        └─────────────────┬─────────────────┘
                          │
       Ciclos de Tensión Cortante (N > 100.000)
                          ▼
        ┌───────────────────────────────────┐
        │ Aumento Rápido de Presión de Poros│
        │ Tensión Efectiva σ' ──► 0         │
        │ Fluidización / Lodo de Subrasante │
        └─────────────────┬─────────────────┘
                          │
       El Lodo Asciende por los Huecos del Balasto
                          ▼
        Fallo de Geometría de Vía y Asentamiento Rápido
        (Remedio: Sellado Químico-Biopolimérico + Manta de Drenaje bajo Balasto)
```

### Formulación Constitutiva Avanzada y Mitigación
El equipo del Prof. Indraratna desarrolla un modelo elastoplástico cíclico de fluidización que incorpora el arrastre hidráulico interparticular y la degradación cíclica. Valida que disponer una capa de sellado tratada con biopolímeros o drenes verticales prefabricados acelera la disipación de la presión de poros, acotando la relación de presión de poros cíclica ($r_u < 0.35$) y suprimiendo por completo el bombeo de lodo.

---

## 2. Terraplenes Apoyados sobre Columnas de Suelo Geopolimérico (S. Gupta, S. Kumar)

### Columnas de Suelo Sostenibles Activadas con Álcalis
La fabricación de cemento Portland ordinario (OPC) es responsable de aproximadamente el $8\%$ de las emisiones mundiales de $\text{CO}_2$. Gupta y Kumar evalúan ceniza volante y escoria granulada molida de alto horno (GGBS) activadas con disoluciones alcalinas (silicato sódico e hidróxido sódico) para construir columnas profundas de suelo que sostienen terraplenes de autopista:
- **Resistencia a Compresión Simple ($q_u$):** Las columnas geopoliméricas alcanzan resistencias a compresión a 28 días de $3.5\,\text{MPa} - 6.2\,\text{MPa}$, comparables o superiores a las del mezclado profundo de suelo con cemento convencional (CDSM).
- **Transferencia de Carga del Terraplén (Efecto Arco):** Simulaciones numéricas 3D en PLAXIS confirman que las columnas geopoliméricas movilizan eficazmente el arco de suelo en el relleno granular del terraplén, transfiriendo más del $75\%$ del peso del terraplén directamente al estrato portante competente.

---

## 3. Nanotubos de Carbono (CNT) para la Mitigación de la Licuefacción de Arena (S. Shaswat, R.P. Orense)

### Nanoingeniería de los Contactos Granulares
Shaswat y Orense investigan el refuerzo micromecánico de arenas limpias sueltas mediante nanotubos de carbono de pared múltiple (MWCNT) dispersados en dosificaciones bajas ($0.05\% - 0.20\%$ en peso seco):
- **Mecanismo de Puente entre Contactos:** La elevada relación de aspecto ($> 1,000$) y el módulo de tracción excepcional ($> 1\,\text{TPa}$) de los CNT crean puentes flexibles de tracción a nanoescala entre granos de cuarzo adyacentes.
- **Resistencia Cíclica:** Los ensayos triaxiales cíclicos demuestran que añadir solo un $0.1\%$ de MWCNT incrementa la relación de resistencia cíclica ($CRR_{20}$) en un $65\%$, retardando significativamente la acumulación de deformación cíclica sin perjudicar el drenaje hidráulico.

---

## 4. Curvas de Diseño de Consolidación No Lineal para Drenes Verticales (K. Kharsyiemiong, V.A. Sawant, S. Mittal)

### Superación de las Hipótesis Lineales en el Diseño de Precompresión
Las soluciones clásicas de Barron y Hansbo suponen permeabilidad ($k_h$) y compresibilidad volumétrica ($m_v$) constantes durante la consolidación. En depósitos espesos de arcilla marina, tanto la permeabilidad como la compresibilidad disminuyen en órdenes de magnitud al reducirse el índice de huecos (no linealidad $e - \log k$ y $e - \log \sigma'$).

Kharsyiemiong y cols. formulan las ecuaciones de consolidación radial no lineal:

$$\frac{\partial u}{\partial t} = C_h(e) \cdot \left[ \frac{\partial^2 u}{\partial r^2} + \frac{1}{r} \frac{\partial u}{\partial r} \right]$$

- **Curvas de Diseño Normalizadas:** Generan ábacos adimensionales que representan el grado medio de consolidación ($U_r$) frente a la relación no lineal del índice de compresión ($C_c / C_k$).
- **Impacto Ingenieril:** Ignorar la no linealidad subestima la duración necesaria de precompresión hasta en un $30\% - 45\%$, dando lugar a la retirada prematura de la sobrecarga y a asentamientos excesivos post-construcción.

---

## 5. Precipitación de Calcita Inducida por Microorganismos (MICP) mediante DEM (S. Pandey, A.K. Jha, T.N. Singh)

### Mecánica de Enlace de la Biocementación
La biocementación emplea bacterias ureolíticas (*Sporosarcina pasteurii*) para hidrolizar urea en presencia de iones calcio, precipitando cristales de carbonato cálcico ($\text{CaCO}_3$) en las gargantas de contacto entre granos:

$$\text{CO(NH}_2)_2 + 2\text{H}_2\text{O} + \text{Ca}^{2+} \xrightarrow{\text{Ureasa}} \text{CaCO}_3 \downarrow + 2\text{NH}_4^+$$

Pandey y cols. implementan modelos de partículas enlazadas en PFC3D (Particle Flow Code) para simular la rotura de enlaces a microescala bajo corte triaxial:
- **Contenido de Calcita frente a Cohesión:** Elevar el contenido másico de $\text{CaCO}_3$ del $1.5\%$ al $5.0\%$ incrementa la cohesión aparente de $18\,\text{kPa}$ a $280\,\text{kPa}$.
- **Bandas de Cizalla:** Los contactos biocementados mantienen un comportamiento elástico rígido hasta alcanzar una relación de tensiones dilatante pico, seguida de desadhesión frágil de los enlaces y transición a la fricción en estado crítico.

---

## 6. Suite de Instrumentación de Campo para el Mejoramiento de Suelos

| Técnica de Mejoramiento | Sensor Geotécnico Primario | Sensor Diagnóstico Secundario | Parámetro Monitorizado |
| :--- | :--- | :--- | :--- |
| **Fluidización de Subrasante Ferroviaria** | Piezómetro de cuerda vibratoria de alta frecuencia | Acelerómetro de subrasante | Relación dinámica de presión de poros $r_u$, aceleración vertical |
| **Terraplén sobre Columnas Geopoliméricas** | Células de presión de tierras (cabeza de columna y suelo) | Extensómetro magnético de asentamiento | Relación de concentración de tensiones ($n = \sigma_c / \sigma_s$), asentamiento |
| **Precompresión con Drenes Verticales** | Piezómetros multiprofundidad | Perfilador hidrostático de asentamientos | Disipación de presión de poros excedente ($\Delta u$), perfil de asentamiento |
| **Inyección de Compactación** | Inclinómetros ópticos de superficie | Transductor de presión de lechada en cabecera | Detección de levantamiento del terreno, presión de rechazo ($p_{inj}$) |
| **Masa de Suelo Biotratada con MICP** | Transductores ultrasónicos de onda P cross-hole | Sensores de ion amonio en efluente | Rigidez de corte a pequeña deformación ($G_0$), eficiencia de conversión de urea |
