---
lang: es
lang_alt: reference-manuals/practical-rock-engineering/chapter-03-discontinuity-shear-strength/
---

# Capítulo 3 — Resistencia al Corte de las Discontinuidades

## 3.1 Mecánica del cizalle a lo largo de superficies de junta

En macizos rocosos con familias de juntas persistentes, las fallas estructurales
(deslizamientos de banco, caída de cuñas, bloques por vuelco) ocurren por deslizamiento
a lo largo de discontinuidades preexistentes y no por fractura a través de la sustancia
de roca intacta.

La resistencia al corte ($\tau$) a lo largo de una junta rocosa no cementada está
gobernada por tres factores:
1. **Esfuerzo normal ($\sigma_n'$)**: esfuerzo de compresión efectivo que mantiene
   apretados los labios de la junta.
2. **Ángulo de fricción básico ($\phi_b$)**: ángulo de fricción entre granos medido sobre
   superficies lisas, planas y aserradas de la misma roca (típicamente
   $25^\circ - 35^\circ$).
3. **Rugosidad superficial y dilatancia de las asperezas**: ondulaciones geométricas
   (asperezas) que obligan a las paredes opuestas de la junta a cabalgar una sobre otra
   (dilatar) durante el cizalle, o a cizallar las asperezas cuando el esfuerzo normal es
   alto.

---

## 3.2 Modelo bilinear de Patton

F.D. Patton (1966) mostró que asperezas regulares en forma de diente inclinadas un
ángulo $i$ producen una envolvente de resistencia al corte bilineal:

### Esfuerzo normal bajo ($\sigma_n' < \sigma_T$): deslizamiento sobre las asperezas
El desplazamiento de corte obliga a los bloques a dilatar verticalmente sobre los
dientes de las asperezas:

$$\tau = \sigma_n' \tan(\phi_b + i)$$

### Esfuerzo normal alto ($\sigma_n' \ge \sigma_T$): cizalle a través de las asperezas
El esfuerzo normal suprime la dilatancia; los dientes de las asperezas se cortan por su
raíz:

$$\tau = c_j + \sigma_n' \tan(\phi_r)$$

donde $c_j$ es la cohesión aparente por corte de la raíz de las asperezas y $\phi_r$ el
ángulo de fricción residual.

---

## 3.3 Criterio no lineal de resistencia al corte de Barton-Bandis

Como las juntas rocosas reales tienen rugosidad irregular y multiescala, y no dientes
uniformes, Nick Barton y S. Bandis (1976, 1982, 1990) establecieron el criterio empírico
no lineal:

$$\tau = \sigma_n' \tan \left[ \text{JRC} \cdot \log_{10} \left( \frac{\text{JCS}}{\sigma_n'} \right) + \phi_b \right]$$

Donde:
- $\text{JRC}$ = Coeficiente de Rugosidad de Junta, que varía de $0$ (lisa como un
  espejo) a $20$ (muy rugosa y ondulada).
- $\text{JCS}$ = Resistencia a Compresión de la Pared de la Junta, determinada con
  martillo de rebote Schmidt directamente sobre la pared de junta meteorizada o sin
  meteorizar.
- $\phi_b$ = Ángulo de fricción básico de superficies de roca planas y sin meteorizar.
- $\sigma_n'$ = Esfuerzo normal efectivo a través de la abertura de la junta.

### Corrección de escala para juntas de campo
Los ensayos de caja de corte de laboratorio ($L_0 = 100\text{ mm}$) sobreestiman la
rugosidad frente a discontinuidades de campo en bloques ($L_n = 1 - 5\text{ m}$):

$$\text{JRC}_n = \text{JRC}_0 \left( \frac{L_n}{L_0} \right)^{-0,02 \text{JRC}_0}$$

$$\text{JCS}_n = \text{JCS}_0 \left( \frac{L_n}{L_0} \right)^{-0,03 \text{JRC}_0}$$

---

## 3.4 Juntas rellenas y rellenos de harina de falla

Cuando la meteorización o el cizalle de falla deposita relleno de grano fino (harina de
falla arcillosa, talco, clorita) entre las paredes de la junta, se pierde el
trabazón de las asperezas.

- Si el espesor de relleno $t < \text{altura de aspereza } a$, el contacto roca–roca
  sigue contribuyendo a la resistencia al corte.
- Si el espesor de relleno $t \ge 1,5 a$, la resistencia al corte cae a la del propio
  material de harina de falla, drenado o sin drenar ($\phi' \approx 8^\circ - 18^\circ$
  para arcillas esmectíticas). Estos son los planos de deslizamiento críticos
  responsables de deslizamientos históricos como el desastre de Vajont.

---

## 3.5 Terminología canónica

| Español | Inglés | Vietnamita (canónico) | Definición |
| --- | --- | --- | --- |
| Resistencia al corte de discontinuidades | Discontinuity shear strength | Sức kháng cắt của mặt bất liên tục | Resistencia al corte a lo largo de juntas, estratificación y fallas |
| Ángulo de fricción básico $\phi_b$ | Basic friction angle $\phi_b$ | Góc ma sát cơ bản $\phi_b$ | Ángulo de fricción sobre superficies lisas, planas y aserradas |
| Aspereza | Asperity | Mấu nhám | Ondulación geométrica de micro y macroescala en la cara de una junta |
| Coeficiente de Rugosidad de Junta (JRC) | Joint Roughness Coefficient (JRC) | Hệ số độ nhám khe nứt (JRC) | Índice adimensional (0–20) que cuantifica el perfil de la superficie de la junta |
| Resistencia a Compresión de la Pared de la Junta (JCS) | Joint Wall Compressive Strength (JCS) | Cường độ nén thành vách khe nứt (JCS) | Resistencia a compresión uniaxial de la superficie rocosa que forma la pared de la junta |
| Harina de falla | Fault gouge | Sét dập vỡ đứt gãy / Vữa đứt gãy | Material arcilloso blando y muy cizallado que rellena una zona de falla |
