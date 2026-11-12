---
lang: es
lang_alt: reference-manuals/practical-rock-engineering/chapter-02-intact-rock-strength/
---

# Capítulo 2 — Resistencia de la Roca Intacta y Ensayos de Laboratorio

## 2.1 Ensayos mecánicos de la roca intacta

Conocer la resistencia de la roca intacta aporta la cota superior de referencia para
todas las evaluaciones de resistencia del macizo rocoso. Los principales ensayos de
laboratorio normalizados por la Sociedad Internacional de Mecánica de Rocas (ISRM) y
ASTM son:

1. **Resistencia a compresión uniaxial (UCS / $\sigma_{ci}$)**: se realiza sobre
   probetas cilíndricas de testigo con relación longitud/diámetro $L/D = 2,0 - 2,5$.
   Los extremos deben rectificarse planos con tolerancia de $0,02\text{ mm}$ para evitar
   desconchamientos prematuros en los bordes.

$$\sigma_{ci} = \frac{P_{\text{fail}}}{A}$$

2. **Resistencia a tracción indirecta brasileña ($\sigma_t$)**: comprimir un disco
   circular de roca según su diámetro genera tensiones de tracción uniformes y
   perpendiculares en el centro:

$$\sigma_t = \frac{2 P}{\pi D t}$$

   donde $D$ es el diámetro de la probeta y $t$ el espesor del disco. Para la mayoría
   de las rocas frágiles, la resistencia a tracción uniaxial es aproximadamente $1/10$
   a $1/20$ de su UCS ($\sigma_t \approx 0,05 - 0,10 \sigma_{ci}$).

3. **Ensayo de compresión triaxial**: probetas cilíndricas enfundadas en membranas
   impermeables sometidas a presión de fluido de confinamiento ($\sigma_2 = \sigma_3$)
   mientras se incrementa la carga axial ($\sigma_1$) hasta la falla.

---

## 2.2 El criterio de falla de Hoek-Brown para roca intacta

En 1980, Evert Hoek y E.T. Brown introdujeron un criterio empírico no lineal que
relaciona las tensiones principales mayor y menor en la falla de pico de la roca
intacta:

$$\sigma_1' = \sigma_3' + \sigma_{ci} \left( m_i \frac{\sigma_3'}{\sigma_{ci}} + 1 \right)^{0.5}$$

Donde:
- $\sigma_1'$ = tensión principal mayor efectiva en la falla
- $\sigma_3'$ = tensión principal menor efectiva (presión de confinamiento)
- $\sigma_{ci}$ = resistencia a compresión uniaxial de la roca intacta
- $m_i$ = constante petrográfica del material, reflejo de la mineralogía, el
  trabazón de los granos y la textura de la roca

### Valores típicos de $m_i$ para tipos de roca comunes

| Clase de roca | Tipo de roca | $m_i$ típico $\pm \text{d.e.}$ |
| --- | --- | --- |
| **Ígnea** | Granito | $32 \pm 3$ |
| | Basalto | $25 \pm 5$ |
| | Andesita | $25 \pm 5$ |
| **Sedimentaria** | Arenisca | $17 \pm 4$ |
| | Limolita | $7 \pm 2$ |
| | Lutita | $6 \pm 2$ |
| | Caliza | $12 \pm 3$ |
| **Metamórfica** | Cuarcita | $20 \pm 3$ |
| | Esquisto | $12 \pm 3$ |
| | Gneis | $28 \pm 5$ |
| | Mármol | $9 \pm 3$ |

---

## 2.3 Teoría de fisuras de Griffith e inicio de la fractura frágil

¿Por qué es no lineal la roca en compresión triaxial? A.A. Griffith (1921, 1924)
demostró que la falla frágil se inicia a partir de microfisuras elípticas preexistentes
y vacíos en los límites de grano.

Bajo campos de esfuerzo de compresión:
1. Los esfuerzos cortantes a lo largo de los labios de las microfisuras inducen
   concentraciones locales de tensión de tracción en las puntas de la fisura.
2. Cuando la tensión de tracción local supera la resistencia del enlace molecular,
   aparecen fisuras en ala que se propagan de forma estable en la dirección de la
   tensión principal mayor ($\sigma_1$).
3. **Umbral de iniciación de fisuras ($\sigma_{ci,\text{init}} \approx 0,4 - 0,5 \sigma_{ci}$)**:
   aumentan las emisiones acústicas; la deformación lateral se desvía de la linealidad.
4. **Umbral de daño por fisuración ($\sigma_{cd} \approx 0,7 - 0,85 \sigma_{ci}$)**: las
   microfisuras coalescen en bandas de cizalle macroscópicas y la deformación
   volumétrica pasa de compactación a dilatancia.
5. **Falla de pico ($\sigma_1 = \sigma_{\text{peak}}$)**: rotura por cizalle
   macroscópica completa.

---

## 2.4 Terminología canónica

| Español | Inglés | Vietnamita (canónico) | Definición |
| --- | --- | --- | --- |
| Resistencia a compresión uniaxial (UCS) | Uniaxial compressive strength (UCS) | Cường độ nén đơn trục | Esfuerzo axial de falla de pico sin confinamiento ($\sigma_3 = 0$) |
| Ensayo brasileño de tracción | Brazilian tensile test | Thí nghiệm ép chẻ kéo Brazil | Ensayo de tracción indirecto que comprime diametralmente un disco circular de roca |
| Presión de confinamiento | Confining pressure | Áp lực giam hãm | Tensión principal menor ($\sigma_3$) aplicada lateralmente |
| Parámetro de roca intacta $m_i$ | Intact rock parameter $m_i$ | Thông số vật liệu đá nguyên vẹn $m_i$ | Constante empírica del criterio de Hoek-Brown basada en la génesis de la roca |
| Dilatancia volumétrica | Volumetric dilation | Giãn nở thể tích | Aumento de volumen de la roca bajo cizalle por apertura de microfisuras |
