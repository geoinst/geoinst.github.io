---
lang: es
lang_alt: reference-manuals/geovadis-vol2/chapter-02-practice-risk-site-characterisation/
---

# Práctica, Riesgo y Caracterización de Sitio

!!! abstract "Resumen de la Sesión"
    La Sesión 7 de *GeoVadis (GAIC 2025)* conecta las tecnologías de diagnóstico de vanguardia con la práctica profesional de la geotecnia y la gestión de riesgos. Los aspectos destacados incluyen la Tomografía de Resistividad Eléctrica (ERT) de lapso temporal para la imagen de filtraciones internas, la geofísica avanzada de ondas superficiales (MASW), la disipación con Dilatómetro (DMT) para el perfilado de sobreconsolidación, la visualización mecanoluminiscente de la mecánica de hincado de pilotes y el Modelado de Información de Construcción (BIM) geotécnico.

---

## 1. ERT de Lapso Temporal para el Monitoreo de Filtración en Terraplenes (V. Bherde, B. Umashankar)

### Detección No Invasiva de Defectos Internos
La erosión por tubificación, los socavones localizados y las anomalías de la superficie freática en el interior de presas de tierra y diques suelen desarrollarse sin ser detectados antes de una rotura catastrófica. Bherde y Umashankar realizan investigaciones a escala de modelo con Tomografía de Resistividad Eléctrica (ERT) de lapso temporal en 2D/3D:
- **Contraste de Resistividad:** La saturación de agua reduce drásticamente la resistividad eléctrica aparente ($\rho$), creando contrastes nítidos entre el relleno seco no saturado ($\rho > 500\,\Omega\cdot\text{m}$) y las zonas saturadas por filtración ($\rho < 50\,\Omega\cdot\text{m}$).
- **Resolución de la Inversión:** Optimizando la geometría del arreglo de electrodos (Wenner-Schlumberger frente a Dipolo-Dipolo), el sistema detecta el inicio de vacíos por tubificación ($D \approx 50\,\text{mm}$) y captura en tiempo real la velocidad de avance del frente de humedecimiento sin perforar el núcleo de la presa.

```
             Fuente de Agua de Infiltración
                     │
                     ▼
       ┌──────────────────────────────┐
       │ Terraplén Denso de Presa     │ ◄─── Resistividad Alta (Seco: > 500 Ω·m)
       │                              │
       │    Cordón de Electrodos      │
       │    ▼   ▼   ▼   ▼   ▼   ▼   ▼  │
       │                              │
       │      ░░░░░░░░░░░░░░░░        │ ◄─── Frente de Humedecimiento / Zona de Filtración
       │      ░ Pluma de Filtración ░ │      Resistividad Baja (< 50 Ω·m)
       │      ░░░░░░░░░░░░░░░░        │      Invertida en Tomograma 2D en Tiempo Real
       └──────────────────────────────┘
```

---

## 2. Geofísica Avanzada de Ondas Superficiales (MASW) (P. Vishwakarma; C.P. Lin y cols.)

### Perfilado de la Velocidad de Onda de Cizalla ($V_s$)
El Análisis Multicanal de Ondas Superficiales (MASW) proporciona un perfilado no destructivo de la rigidez del subsuelo sin costosos sondeos profundos:
- **Optimización de la Inversión de Dispersión:** Vishwakarma evalúa algoritmos de Optimización Basada en Enseñanza-Aprendizaje (TLBO) para invertir curvas experimentales de dispersión de ondas de Rayleigh en perfiles de velocidad de onda de cizalla a pequeña deformación ($V_s$) hasta $30\,\text{m}$ de profundidad.
- **Clasificación Sísmica del Sitio:** Lin y coautores despliegan sensores de ondas superficiales activos/pasivos de nueva generación para calcular $V_{s30}$, identificando zonas de amplificación de suelos blandos, paleocauces de lecho rocoso enterrados y degradación del módulo de corte ($G_{max} = \rho V_s^2$).

---

## 3. Disipación con Dilatómetro Plano (DMT) en Arcilla Marina Blanda (K. Das, G.R. Dodagoudar y cols.)

### Relación de Sobreconsolidación ($OCR$) In Situ Directa
Determinar la tensión de preconsolidación ($\sigma'_p$) y el coeficiente de consolidación horizontal ($c_h$) en arcillas aluviales y marinas sensibles mediante ensayos edométricos de laboratorio es propenso a la perturbación de la muestra. Das y cols. realizan ensayos con Dilatómetro Plano de Marchetti (DMT) con disipación de presión temporizada (lecturas $A$):
- **Índice de Tensión Horizontal ($K_D$):** La relación de sobreconsolidación in situ se correlaciona directamente con el índice de tensión horizontal:
  $$OCR = (0.5 \cdot K_D)^{1.56}$$
- **Disipación de la Presión de Poros:** El tiempo necesario para un decaimiento del $50\%$ de la presión ($t_{50}$) proporciona estimaciones fiables del coeficiente de consolidación horizontal ($c_h$) que concuerdan estrechamente con las velocidades de asentamiento retrocalculadas en terraplenes de autopista instrumentados cercanos.

---

## 4. Imagen por Mecanoluminiscencia de la Penetración de Pilotes (A. Kondo, E. Kohama, D. Takano, R.J. Bathurst)

### Visualización Óptica de los Contactos a Escala de Grano
Visualizar la localización de la deformación de corte y las zonas de trituración bajo la punta de un pilote en avance exigía históricamente complejas radiografías de rayos X. Kondo y cols. desarrollan un método óptico innovador con granos de arena recubiertos de **fósforo mecanoluminiscente** ($\text{SrAl}_2\text{O}_4:\text{Eu}$):
- **Respuesta Luminiscente a la Tensión:** Ante el corte mecánico y la tensión de contacto por compresión, el fósforo emite luz verde visible proporcional a la magnitud de la tensión de contacto localizada.
- **Fotometría de Alta Velocidad:** Cámaras de alta velocidad capturan bulbos dinámicos de concentración de tensiones y la formación de bandas de cizalla intensas que irradian desde la punta del pilote durante su penetración sostenida en arena densa.

---

## 5. Ensayo de Penetración Estándar (SPT): Valoración Forense de la Práctica (M.M. Hoque, M.M. Rahman)

### Normas Globales frente a la Realidad de las Regiones en Desarrollo
El Ensayo de Penetración Estándar (valor $N$) sigue siendo el parámetro de caracterización de sitio más omnipresente en el diseño de cimentaciones a nivel mundial. Hoque y Rahman revisan las prácticas de campo en Bangladés y el sur de Asia, señalando discrepancias críticas frente a la norma ASTM D1586:
- **Relación de Energía del Martillo ($ER$):** Los mecanismos manuales de disparo por cabrestante y cuerda entregan relaciones de energía reales entre el $45\%$ y el $58\%$, frente al $60\%$ normalizado del martillo automático de disparo ($N_{60}$).
- **Limpieza del Sondeo y Perforación por Lavado:** La limpieza incompleta del fondo y el desequilibrio de carga hidrostática en la entubación inducen tubificación de fondo, reduciendo los valores de $N$ medidos hasta en un $50\%$.
- **Valor Normalizado Corregido:** Los proyectistas deben aplicar sistemáticamente las fórmulas de corrección:
  $$N_{60} = N_{raw} \cdot \frac{ER}{60} \cdot C_B \cdot C_S \cdot C_R$$
  donde $C_B, C_S, C_R$ contemplan el diámetro del sondeo, el revestimiento del tomamuestras y la longitud de varillaje.

---

## 6. Matriz de Instrumentación de Campo para la Caracterización de Sitio

| Herramienta de Caracterización | Sensor Geofísico / In Situ Primario | Sonda Complementaria de Campo / Laboratorio | Parámetro Geotécnico Derivado |
| :--- | :--- | :--- | :--- |
| **Arreglo ERT de Lapso Temporal** | Cable de Resistividad Multielectrodo | Piezómetros en Ubicaciones Anómalas | Saturación interna, velocidad de filtración, tubificación |
| **Arreglo Sísmico MASW** | Arreglo Lineal de Geófonos ($4.5\,\text{Hz}$) | Registrador Sísmico P-S en Sondeo | Velocidad de onda de cizalla $V_s$, módulo a pequeña deformación $G_0$ |
| **Dilatómetro Plano (DMT)** | Cuchilla Dilatométrica de Acero Inoxidable | Penetrómetro Piezocono (CPTu) | $OCR$ in situ, consolidación horizontal $c_h$ |
| **Arreglo Mecanoluminiscente**| Sensor Fotométrico CCD de Alta Velocidad | Células de Carga Dinámicas en Cabeza de Pilote | Bulbo de tensión de contacto, bandas de cizalla localizadas |
| **Equipo SPT Calibrado** | Subsistema SPT Instrumentado (Carga y Aceleración) | Caja Calibradora de Relación de Energía | Relación de energía entregada $ER$, valor normalizado $N_{60}$ |
