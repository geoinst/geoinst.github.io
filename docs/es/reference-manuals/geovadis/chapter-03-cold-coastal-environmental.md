---
lang: es
lang_alt: reference-manuals/geovadis/chapter-03-cold-coastal-environmental/
---

# Geotecnia Fría, Costera y Ambiental

!!! abstract "Resumen de la Sesión"
    La Sesión 2 de *GeoVadis (GAIC 2025)* aborda desafíos geopolíticos y ambientales en la
    interfaz entre geotecnia, cambio climático y aislamiento de residuos. Las
    contribuciones centrales exploran la degradación por congelación-deshielo en terrenos
    alpinos, el análisis digital de imágenes de la fisuración por desecación de arcillas,
    el hinchamiento de bentonitas bajo gradientes químicos y térmicos extremos, el
    monitoreo de campo de la presión de agua de poro durante la precarga al vacío y el
    almacenamiento geotérmico somero en formaciones no saturadas.

---

## 1. Mecánica de Congelación-Deshielo en Suelos Estacionalmente Helados (C. Tagar, A. Kalita, A. Dey)

### Vulnerabilidad de la infraestructura de gran altitud
La infraestructura construida a gran altitud —como el túnel de Sela, a 4 200 m de cota
en Arunachal Pradesh (India)— afronta una severa ciclicidad térmica estacional. Tagar y
colaboradores realizan ensayos multiciclo de congelación-deshielo (temperaturas
oscilando entre $-15^\circ\text{C}$ y $+20^\circ\text{C}$) sobre suelos naturales de
subrasante:
- **Alteración de la estructura porosa:** la formación criogénica de lentes de hielo
  expande los microporos existentes durante la congelación. El deshielo posterior deja
  índices de huecos ($e$) ampliados y rompe los enlaces de cementación entre partículas.
- **Degradación de la resistencia a compresión no confinada ($q_u$):** la resistencia
  cae exponencialmente durante los primeros 5 ciclos, perdiendo hasta el 45 % de la
  resistencia virgen original antes de alcanzar una meseta residual asintótica.
- **Módulo resiliente ($M_R$):** los ensayos triaxiales cíclicos confirman una reducción
  sustancial de la rigidez de la subrasante, lo que explica el ahuellamiento prematuro y
  la fisuración por fatiga en corredores viarios alpinos.

---

## 2. Fisuración por Desecación en Arcilla Compactada (S. Majumder, B.K. Agarwal, A. Sachan)

### Análisis digital de imágenes (DIA) y correlación digital de imágenes (DIC)
La fisuración por desecación compromete la integridad hidráulica de las barreras
arcillosas de vertederos, los terraplenes de canales y los núcleos de presas de tierra.
Majumder y colaboradores emplean seguimiento óptico de alta resolución junto con mapeo
de deformaciones por DIC para monitorizar la iniciación y propagación de grietas durante
un secado continuo:
- **Umbral de deformación de tracción:** las grietas se inician cuando las deformaciones
  de tracción localizadas superan la capacidad de deformación de tracción
  ($\epsilon_{t,lim} \approx 1{,}2\% - 1{,}8\%$) en los contornos de las celdas.
- **Factor de intensidad de fisuración (CIF):** se cuantifica como la relación entre el
  área superficial de grietas y el área total de la probeta ($CIF = A_{crack} / A_{total}$).
- **Frontera de succión:** la fisuración comienza precisamente cuando la succión mátrica
  se aproxima al valor de entrada de aire ($AEV$), desencadenando el retroceso del
  menisco de agua hacia los poros subsuperficiales.

```
       Evaporación de humedad (secado) ──► El menisco retrocede hacia los poros
                                           │
                                           ▼
       Aumenta la succión mátrica (ψ = ua - uw) ──► Crece la tensión capilar
                                           │
                                           ▼
       La tensión de tracción supera la resistencia a tracción del suelo (σ_t > f_t)
                                           │
                                           ▼
       Inicio de grieta en defectos de desecación ──► DIC detecta localización de deformación
                                           │
                                           ▼
       Interconexión de la red de grietas ──► El CIF salta, la permeabilidad aumenta 100x
```

---

## 3. Hinchamiento e Infiltración de Barreras de Bentonita (D. Ito, N. Yamada, H. Wang, H. Komine)

### Almacenamientos geológicos profundos de residuos radiactivos
Las mezclas compactadas de bentonita y arena actúan como barreras de ingeniería que
aíslan los contenedores de residuos nucleares de alta actividad. Ito y colaboradores
investigan cómo el intercambio catiónico ($Na^+$ frente a $Ca^{2+}$) y la intrusión de
agua subterránea salina alteran la presión de hinchamiento ($p_s$) y la conductividad
hidráulica ($k$) de la barrera:
- **Impacto de la valencia catiónica:** el agua subterránea salina con iones divalentes
  ($Ca^{2+}, Mg^{2+}$) comprime la doble capa difusa (DDL), reduciendo el volumen de
  hinchamiento libre en más del 60 % respecto al agua desionizada.
- **Capacidad de autosellado:** pese a la salinización, la bentonita sódica compactada
  conserva presión de hinchamiento suficiente ($p_s > 2\,\text{MPa}$) a densidades secas
  $\rho_d \ge 1{,}6\,\text{g/cm}^3$ para sellar juntas constructivas y grietas térmicas.
- **Influencia térmica acoplada (T. Nishimura):** a temperaturas elevadas
  ($T = 60^\circ\text{C} - 80^\circ\text{C}$), los ensayos de hinchamiento con succión
  controlada revelan una redistribución acelerada del agua y migración de vapor térmico
  alejándose de las fuentes de calor.

---

## 4. Consolidación por Precarga al Vacío: Caso de Estudio de Fisherman Island (L. Karagoz, B. Indraratna, et al.)

### Verificación de campo de la consolidación asistida por vacío
En el puerto de Brisbane (Fisherman Island, Australia), la ganancia de terreno al mar
sobre arcillas marinas ultrablandas y profundas exigió combinar precarga al vacío con
drenes verticales prefabricados (PVD). Karagoz e Indraratna analizan datos completos de
monitoreo de campo:
- **Distribución de presión negativa de vacío:** se aplica una presión de poro negativa
  sostenida de $-70\,\text{kPa}$ a $-80\,\text{kPa}$ bajo la geomembrana estanca,
  propagándose a lo largo de los PVD hasta $20\,\text{m}$ de profundidad.
- **Equivalencia de tensión efectiva:** a diferencia de los rellenos de sobrecarga física
  que aumentan la tensión total ($\Delta \sigma$), la presión de vacío induce
  directamente una presión de poro negativa ($-\Delta u$), generando un incremento
  isotrópico de tensión efectiva ($\Delta \sigma' = -\Delta u$) sin provocar rotura por
  corte ni expulsión lateral hacia el exterior en el pie del terraplén.
- **Perfilado de disipación de la presión de agua de poro:** los piezómetros de cuerda
  vibratoria instalados a $3\,\text{m}$, $8\,\text{m}$, $14\,\text{m}$ y $19\,\text{m}$
  de profundidad muestran una consolidación radial acelerada que alcanza el 90 % de la
  consolidación primaria en 120 días.

---

## 5. Optimización del Almacenamiento Geotérmico Somero (A. Deshmukh, A.J. Puppala, X. Yu, et al.)

### Almacenamiento subterráneo de energía térmica (UTES)
Deshmukh y colaboradores demuestran que las formaciones arcillosas no saturadas poseen
una inercia térmica idónea para el almacenamiento estacional de calor:
- **Acoplamiento termohidráulico:** la inyección de calor eleva la temperatura del
  terreno a la vez que aleja la humedad de poro de los intercambiadores de calor de
  sondeo (BHE), provocando desaturación localizada y reduciendo la conductividad térmica
  efectiva ($\lambda$).
- **Optimización heurística:** los algoritmos genéticos (GA) optimizan el espaciado
  entre sondeos ($S/D = 4 - 6$) y los caudales, logrando eficiencias de ciclo completo
  de almacenamiento térmico superiores al 72 % en ciclos anuales de calefacción y
  refrigeración.

---

## 6. Suite de Sensores de Campo para Geotecnia Ambiental

| Sistema de ingeniería | Sensor / diagnóstico primario | Sensor secundario | Magnitud objetivo medida |
| :--- | :--- | :--- | :--- |
| **Subrasante viaria alpina** | Reflectometría en el dominio del tiempo (TDR) | Cadena multinivel de termistores | Profundidad del frente de congelación, contenido de agua no helada |
| **Barrera arcillosa de vertedero** | Tensiómetros de alta capacidad | Resistividad eléctrica in-situ | Succión mátrica ($\psi$), inicio de grietas, intrusión de lixiviados |
| **Bentonita para residuos nucleares** | Células miniatura de presión total | Psicrómetros + termopares | Presión de hinchamiento ($p_s$), succión, temperatura ($T$) |
| **Sitio de precarga al vacío** | Piezómetros de cuerda vibratoria | Galgas perfiladoras + extensómetros magnéticos | Presión de poro negativa ($u$), asentamiento subsuperficial |
| **Arreglo de sondeos geotérmicos** | Cable de fibra óptica DTS | Caudalímetros + sensores de flujo de calor | Registro continuo de temperatura, tasa de inyección de calor |
