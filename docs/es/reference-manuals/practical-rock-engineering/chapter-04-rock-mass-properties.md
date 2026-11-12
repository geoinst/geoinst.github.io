---
lang: es
lang_alt: reference-manuals/practical-rock-engineering/chapter-04-rock-mass-properties/
---

# Capítulo 4 — Propiedades del Macizo Rocoso y el Índice de Resistencia Geológica (GSI)

## 4.1 El criterio de falla generalizado de Hoek-Brown (edición 2002)

En macizos rocosos muy fracturados, donde los bloques estructurales individuales son
pequeños frente a la huella de la excavación, el macizo se comporta como un
pseudocontinuo equivalente e isótropo. Hoek, Carranza-Torres y Corkum (2002)
formularon la envolvente de falla generalizada de Hoek-Brown:

$$\sigma_1' = \sigma_3' + \sigma_{ci} \left( m_b \frac{\sigma_3'}{\sigma_{ci}} + s \right)^a$$

Donde:
- $\sigma_{ci}$ = resistencia a compresión uniaxial de la roca intacta
- $m_b$ = valor reducido de la constante de material $m_i$ para el macizo rocoso:

$$m_b = m_i \exp \left( \frac{\text{GSI} - 100}{28 - 14D} \right)$$

- $s$ y $a$ son constantes empíricas que describen la fracturación y el trabazón del
  macizo rocoso:

$$s = \exp \left( \frac{\text{GSI} - 100}{9 - 3D} \right)$$

$$a = \frac{1}{2} + \frac{1}{6} \left( e^{-\text{GSI}/15} - e^{-20/3} \right)$$

- $D$ es el **factor de disturbio** ($0,0 \le D \le 1,0$), que tiene en cuenta la
  microfracturación inducida por voladura y la relajación de esfuerzos durante la
  excavación.

---

## 4.2 El sistema del Índice de Resistencia Geológica (GSI)

El Índice de Resistencia Geológica (GSI) sustituye a los sistemas de clasificación
cuantitativos (RMR, Q), que se degradaban en macizos rocosos muy pobres y débiles
($RMR < 25$). El GSI se apoya en dos observaciones geológicas visuales:

1. **Estructura del macizo rocoso (trabazón a macroescala)**:
   - *Intacto o masivo*: pocas discontinuidades, muy espaciadas.
   - *En bloques*: bloques cúbicos bien trabados formados por tres familias de juntas
     ortogonales que se cortan.
   - *Muy bloqueado*: cuatro o más familias de juntas que crean bloques angulosos
     multifacetados.
   - *Disturbado / plegado*: macizo plegado, cizallado o fallado con bloques angulosos.
   - *Desintegrado*: fragmentos de tamaño grava mal trabados y muy triturados.
2. **Calidad superficial de las discontinuidades (estado de la pared de la junta)**:
   - Se evalúa desde *Muy buena* (paredes rugosas, sin meteorizar, frescas) hasta *Muy
     pobre* (superficies pulidas por cizalle, relleno de harina arcillosa blanda).

```
+----------------------------------------------------------------------------------------------+
|                          ÍNDICE DE RESISTENCIA GEOLÓGICA (GSI)                             |
+----------------------+--------------------+--------------------+---------------------------+
| ESTRUCTURA           | Superficie buena   | Superficie regular | Superficie pobre / arcilla |
+----------------------+--------------------+--------------------+---------------------------+
| EN BLOQUES           |   GSI = 60 - 80    |   GSI = 50 - 65    |      GSI = 35 - 50        |
| MUY BLOQUEADO        |   GSI = 50 - 65    |   GSI = 40 - 55    |      GSI = 25 - 40        |
| DISTURBADO / FALLADO |   GSI = 35 - 50    |   GSI = 25 - 40    |      GSI = 15 - 30        |
| DESINTEGRADO         |   GSI = 20 - 35    |   GSI = 15 - 25    |      GSI < 15             |
+----------------------+--------------------+--------------------+---------------------------+
```

---

## 4.3 Parámetros equivalentes de Mohr-Coulomb ($c', \phi'$)

Como la mayoría de los programas numéricos geotécnicos (FLAC, PLAXIS, RS2) exigen
parámetros de Mohr-Coulomb, Hoek y otros derivaron la cohesión ($c'$) y el ángulo de
fricción ($\phi'$) equivalentes ajustando rectas tangentes a la curva no lineal de
Hoek-Brown sobre un rango superior de esfuerzos $\sigma_{3,\max}'$:

$$\phi' = \arcsin \left[ \frac{6 a m_b (s + m_b \sigma_{3n}')^{a-1}}{2(1 + a)(2 + a) + 6 a m_b (s + m_b \sigma_{3n}')^{a-1}} \right]$$

$$c' = \frac{\sigma_{ci} \left[ (1 + 2a)s + (1 - a)m_b \sigma_{3n}' \right] (s + m_b \sigma_{3n}')^{a-1}}{(1 + a)(2 + a) \sqrt{1 + \left( 6 a m_b (s + m_b \sigma_{3n}')^{a-1} \right) / \left( (1 + a)(2 + a) \right)}}$$

---

## 4.4 Módulo de deformación del macizo rocoso ($E_{rm}$)

Estimar el módulo de deformación del macizo rocoso es crucial para calcular la
convergencia de las paredes del túnel y el asentamiento de cimentaciones. La ecuación
empírica de Hoek-Diederichs (2006) da:

$$E_{rm} = E_i \left( 0,02 + \frac{1 - D/2}{1 + e^{(60 + 15D - \text{GSI})/11}} \right)$$

donde $E_i$ es el módulo de Young de la roca intacta ($\text{MPa}$). Si no se dispone de
$E_i$ de laboratorio, puede aproximarse a partir de la Relación de Módulos ($MR$):
$E_i = MR \cdot \sigma_{ci}$.

---

## 4.5 Terminología canónica

| Español | Inglés | Vietnamita (canónico) | Definición |
| --- | --- | --- | --- |
| Índice de Resistencia Geológica (GSI) | Geological Strength Index (GSI) | Chỉ số Cường độ Địa chất (GSI) | Índice (10–100) basado en la estructura de la roca y el estado de las juntas |
| Factor de disturbio $D$ | Disturbance factor $D$ | Hệ số tổn thương do nổ mìn $D$ | Factor (0–1) que reduce la resistencia del macizo por daño de voladura |
| Continuo equivalente | Equivalent continuum | Môi trường tựa liên tục tương đương | Modelo continuo que representa macizos rocosos muy diaclasados |
| Módulo de deformación | Deformation modulus | Mô đun biến dạng khối đá | Módulo elástico que representa la deformación total del macizo rocoso |
