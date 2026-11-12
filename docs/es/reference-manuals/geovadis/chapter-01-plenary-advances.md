---
lang: es
lang_alt: reference-manuals/geovadis/chapter-01-plenary-advances/
---

# Ponencias Plenarias: Avances en Ingeniería del Terreno y Geotecnia Energética

!!! abstract "Resumen de la Sesión"
    La Sesión Plenaria de *GeoVadis (GAIC 2025)* reúne las contribuciones magistrales de
    autoridades internacionales que abordan desafíos fundamentales de la ingeniería
    geotécnica: la verificación de calidad en el mejoramiento profundo del terreno, la
    inestabilidad de taludes inducida por sismos y gobernada por el agua subterránea, el
    aprovechamiento geotérmico urbano sostenible, la mecánica de consolidación por drenaje
    radial y la caracterización experimental avanzada de geomateriales no saturados.

---

## 1. Evaluación y Control de Calidad en Mezcla Profunda y Jet Grouting (F.H. Lee)

### Contexto ingenieril y desafíos centrales
La mezcla profunda (columnas de suelo-cemento) y el *jet grouting* se emplean
ampliamente en Asia para muros de contención de excavaciones, barreras de impermeabilidad
y mejoramiento de cimentaciones en arcillas aluviales y marinas blandas. Sin embargo, las
columnas resultantes presentan una variabilidad espacial considerable en resistencia a
compresión ($q_u$), continuidad del fuste y diámetro geométrico, debido a la disipación no
uniforme de la energía de inyección in-situ y a la estratificación del suelo.

### Técnicas de diagnóstico y verificación
El profesor Lee sintetiza metodologías de evaluación no destructiva (NDE), convencionales
y modernas:
- **Testificación continua con extracción de núcleo:** referente del sector; exige una
  recuperación mínima del 85 % de testigo para determinar los perfiles espaciales de
  resistencia.
- **Muestreo húmedo de lechada (*wet grab sampling*):** extracción de la lechada fresca
  inmediatamente después de la inyección, para evaluar la uniformidad de la mezcla antes
  del fraguado.
- **Tomografía de resistividad eléctrica (ERT) y ensayo sónico cross-hole (CSL):**
  imagen no destructiva de la continuidad geométrica de la columna, defectos de
  estrangulamiento (*necking*) y verticalidad.

### Implicaciones ingenieriles y confiabilidad
El coeficiente de variación ($COV$) de la resistencia a compresión no confinada ($q_u$)
en suelos mezclados en profundidad suele situarse entre $0{,}30$ y $0{,}65$. Los
cálculos estructurales y de asentamiento que ignoran esta variabilidad sobreestiman
significativamente el factor de seguridad de diseño. El trabajo establece factores
parciales basados en confiabilidad que garantizan el cumplimiento de los estados límite
de servicio (SLS) y último (ULS) bajo un enfoque prestacional.

---

## 2. Efectos del Agua Subterránea en la Inestabilidad Cosísmica de Taludes: Sismo de la Península de Noto de 2024 (I. Towhata, S. Oji, T. Hosoya)

### El evento de la península de Noto de 2024
El 1 de enero de 2024 un sismo de gran magnitud ($M_w 7{,}5$) sacudió la península de
Noto, en la prefectura de Ishikawa (Japón), desencadenando miles de deslizamientos
cosísmicos y flujos de detritos que aislaron comunidades y devastaron infraestructuras
costeras críticas.

### El papel decisivo del agua subterránea
El profesor Towhata y sus coautores demuestran que las roturas de talud no fueron
provocadas únicamente por las fuerzas de inercia del sacudimiento:
- **Precipitación antecedente:** las intensas lluvias invernales previas y el deshielo
  habían elevado la superficie freática, saturando las rocas sedimentarias neógenas
  meteorizadas y las tobas volcánicas.
- **Picos transitorios de presión de poros:** el sacudimiento intenso generó elevadas
  sobrepresiones de agua de poro ($\Delta u$) a lo largo de contactos geológicos entre
  capas permeables e impermeables, reduciendo drásticamente la tensión normal efectiva
  ($\sigma' = \sigma - u$).
- **Roturas retardadas:** varios deslizamientos de gran magnitud se movilizaron horas
  después del sismo principal, lo que subraya el papel de la redistribución del flujo
  subterráneo y de las obstrucciones locales del drenaje.

```
                    Estado previo al sismo: línea freática elevada
                    ┌───────────────────────────────────────────────┐
                    │ Infiltración de lluvia / deshielo             │
                    │    ▼          ▼          ▼          ▼         │
       Superficie   ┌─────────────────────────────────────────────┐ │
       del terreno ►│ Cobertura meteorizada saturada               │ │
                    │═════════════════════════════════════════════│ │
                    │ Nivel freático (elevado)                     │ │
                    └─────────────────────────────────────────────┘ │
                                          │                         │
               Sacudimiento dinámico cosísmico (Mw 7,5)             │
                                          ▼                         │
                    ┌─────────────────────────────────────────────┐ │
                    │ Sobrepresión de poros dinámica (Δu)          │ │
                    │ Tensión efectiva σ' = σ - (u + Δu)           │ │
                    │ La resistencia al corte τ_f cae críticamente │ │
                    │ ──► Deslizamientos planares y rotacionales ► │ │
                    └─────────────────────────────────────────────┘ │
                    └───────────────────────────────────────────────┘
```

---

## 3. Cimentaciones Urbanas Energéticas Sostenibles (L. Laloui, E. Ravera, A.F. Rotta Loria)

### Concepto de geo-estructuras termoactivas
Las geo-estructuras energéticas —pilotes energéticos, muros pantalla energéticos y
revestimientos de túnel energéticos— integran tuberías intercambiadoras de calor
(circuitos de fluido de circuito cerrado) directamente en los elementos de cimentación
estructurales, con una doble funcionalidad:
1. Soporte estructural primario de las cargas mecánicas de la superestructura.
2. Intercambio de energía térmica renovable con el terreno circundante para calefacción
   y refrigeración de edificios mediante bombas de calor geotérmicas (GSHP).

### Interacción termomecánica suelo-estructura
Las variaciones térmicas ($\Delta T$) inducen expansión y contracción térmica cíclica en
el hormigón estructural:
- **Tensiones térmicas restringidas:** cuando la expansión axial térmica está coartada
  por la resistencia de punta del pilote y el rozamiento del fuste, se desarrollan
  tensiones de compresión térmica significativas:
  $$\Delta \sigma_{th} = - E_{pile} \cdot \alpha_c \cdot \Delta T$$
  donde $E_{pile}$ es el módulo elástico y $\alpha_c$ el coeficiente de dilatación
  térmica del hormigón.
- **Fluencia del suelo y plasticidad cíclica:** la repetición estacional de los ciclos
  térmicos altera la rigidez y la movilización del corte en las arcillas circundantes, lo
  que exige una verificación cuidadosa frente a la fatiga térmica y al asentamiento
  diferencial.

---

## 4. Consolidación bajo Drenaje Radial (R.G. Robinson, G. Sridhar, R.P. Aparna)

### Mecánica del drenaje radial en suelos blandos
La consolidación radial acelerada mediante drenes verticales prefabricados (PVD) es
práctica habitual para la precarga de arcillas marinas blandas y rellenos de dragado. El
profesor Robinson y sus colaboradores revisan las soluciones clásicas de Barron y Hansbo:

$$\bar{U}_r = 1 - \exp\left( -\frac{8 \, T_r}{\mu} \right)$$

donde $T_r = c_h t / d_e^2$ es el factor de tiempo radial, $d_e$ el diámetro equivalente
de influencia del dren y $\mu$ el factor geométrico y de resistencia de la zona alterada
(*smear*):

$$\mu \approx \ln\left(\frac{n}{s}\right) + \frac{k_h}{k_s}\ln(s) - \frac{3}{4} + \pi z (2l - z)\frac{k_h}{q_w}$$

### Conclusiones prácticas clave
- **Permeabilidad de la zona alterada ($k_h / k_s$):** la relación entre la permeabilidad
  horizontal del terreno inalterado y la de la zona alterada suele estar entre $2$ y $5$,
  lo que retrasa severamente la consolidación si no se controla la perturbación del
  mandril.
- **Resistencia hidráulica del dren ($q_w$):** en drenes verticales largos
  ($> 20\,\text{m}$), la capacidad de descarga hidráulica del núcleo se convierte en el
  cuello de botella gobernante.

---

## 5. Mecánica Experimental de Suelos No Saturados (T. Nishimura)

### Ensayos de laboratorio con succión controlada
El profesor Nishimura presenta técnicas experimentales avanzadas para caracterizar el
comportamiento de suelos no saturados:
- **Técnica de traslación de ejes (*axis translation*):** separa la presión de aire de
  poro ($u_a$) y la presión de agua de poro ($u_w$) a través de discos cerámicos de alta
  entrada de aire, permitiendo controlar la succión mátrica ($\psi = u_a - u_w$).
- **Curva característica suelo-agua (SWCC):** captura los ciclos histéricos de
  humedecimiento y secado que gobiernan la retención de agua.
- **Resistencia al corte de Mohr-Coulomb extendida:**
  $$\tau_f = c' + (\sigma - u_a)\tan\phi' + (u_a - u_w)\tan\phi^b$$
  donde $\phi^b$ define la tasa de incremento de la resistencia al corte con la succión
  mátrica.

---

## 6. Lista de Verificación de Instrumentación de Campo para Avances en Ingeniería del Terreno

| Aplicación | Sensor primario recomendado | Sensor secundario / redundante | Parámetro ingenieril clave |
| :--- | :--- | :--- | :--- |
| **Columnas de mezcla profunda y jet grouting** | Ensayo sónico cross-hole (CSL) | Testificación + ensayo UCS en laboratorio | Continuidad de columna, $q_u$, estrangulamientos |
| **Taludes cosísmicos** | Piezómetro de cuerda vibratoria | Tubo inclinométrico | Presión de agua de poro ($\Delta u$), profundidad de deslizamiento |
| **Pilotes energéticos termoactivos** | Galgas de cuerda vibratoria + sister bars | Detección distribuida de temperatura (fibra DTS) | Deformación axial térmica ($\epsilon_{th}$), temperatura ($T$) |
| **Precarga al vacío con PVD** | Piezómetros multinivel | Extensómetros magnéticos de asentamiento | Disipación por consolidación ($U_r$), asentamiento |
| **Taludes de suelo no saturado** | Tensiómetros / psicrómetros de alta capacidad | Reflectometría en el dominio del tiempo (TDR) | Succión mátrica ($\psi$), humedad volumétrica ($\theta$) |
