---
lang: es
lang_alt: reference-manuals/practical-rock-engineering/chapter-05-in-situ-stresses/
---

# Capítulo 5 — Esfuerzos In-Situ e Inducidos alrededor de Excavaciones Subterráneas

## 5.1 El campo de esfuerzos virgen in-situ

Antes de crear una excavación, el macizo rocoso subterráneo está sometido a un estado de
equilibrio natural denominado **campo de esfuerzos virgen (o in-situ)**.

### Esfuerzo vertical ($\sigma_v$)
El esfuerzo vertical lo genera el peso gravitatorio de la columna de roca suprayacente
(profundidad de sobrecarga $z$, peso unitario $\gamma \approx 0,027\text{ MN/m}^3$):

$$\sigma_v = \int_0^z \gamma(z)\, dz \approx \gamma z \approx 0,027 z \quad (\text{MPa para } z \text{ en metros})$$

### Relación de esfuerzo horizontal ($k_0$)
Los movimientos de placas tectónicas, la contracción térmica y la historia erosiva hacen
que los esfuerzos horizontales ($\sigma_h, \sigma_H$) se desvíen marcadamente de las
hipótesis hidrostáticas simples:

$$k_0 = \frac{\sigma_h}{\sigma_v}$$

Según mediciones mundiales compiladas por Hoek y Brown, a profundidades someras
($< 500\text{ m}$), $k_0$ supera con frecuencia $1,5$ a $3,5$ por esfuerzos residuales
tectónicos atrapados:

$$\frac{100}{z} + 0,3 \le k_0 \le \frac{1500}{z} + 0,5$$

---

## 5.2 La solución analítica de Kirsch para túneles circulares

Excavar una cavidad subterránea elimina las tracciones internas y obliga a los esfuerzos
a fluir alrededor del vacío. Para un túnel circular de radio $a$ en un medio elástico
isótropo sometido a esfuerzo vertical $p$ y esfuerzo horizontal $k p$:

### Esfuerzo tangencial (circunferencial, $\sigma_\theta$)

$$\sigma_\theta = \frac{p}{2} \left[ (1 + k)\left(1 + \frac{a^2}{r^2}\right) - (1 - k)\left(1 + 3\frac{a^4}{r^4}\right)\cos 2\theta \right]$$

### Esfuerzo radial ($\sigma_r$)

$$\sigma_r = \frac{p}{2} \left[ (1 + k)\left(1 - \frac{a^2}{r^2}\right) + (1 - k)\left(1 - 4\frac{a^2}{r^2} + 3\frac{a^4}{r^4}\right)\cos 2\theta \right]$$

### En el contorno del túnel ($r = a$):
- El esfuerzo radial es nulo: $\sigma_r = 0$.
- Bóveda / contrabóveda ($\theta = \pi/2$): $\sigma_{\theta,\text{bóveda}} = p (3k - 1)$.
- Hastiales ($\theta = 0$): $\sigma_{\theta,\text{hastial}} = p (3 - k)$.

```
Caso A: esfuerzo hidrostático (k = 1,0)
Esfuerzo tangencial en el contorno: sigma_theta = 2p en todo el perímetro (concentración 2x).

Caso B: esfuerzo tectónico horizontal alto (k = 2,0)
Bóveda:  sigma_theta = p(3(2) - 1) = 5p  (trituración / desconchamiento compresivo severo).
Hastial: sigma_theta = p(3 - 2) = 1p.

Caso C: esfuerzo horizontal bajo (k = 0,25)
Bóveda:  sigma_theta = p(3(0,25) - 1) = -0,25p (apertura por tracción / caída de bloques).
Hastial: sigma_theta = p(3 - 0,25) = 2,75p.
```

---

## 5.3 Concentración de esfuerzos y modos de falla alrededor de cavernas

Cuando el esfuerzo tangencial inducido $\sigma_\theta$ supera la resistencia a
compresión del macizo rocoso ($\sigma_{cm}$):
1. **Desconchamiento / lajeado frágil**: en roca dura masiva ($UCS > 100\text{ MPa}$) se
   desprenden de forma estable láminas delgadas paralelas al contorno de la excavación.
2. **Zona de fluencia plástica**: se desarrolla un anillo plástico circular de radio
   $r_p > a$ alrededor de la apertura, que redistribuye los esfuerzos de pico desde el
   perímetro hacia el interior sólido.
3. **Descompresión por tracción**: en zonas de techo en tracción, la fricción de juntas
   cae a cero ($\sigma_n' \le 0$), lo que hace caer por gravedad los bloques no
   cementados si no se aseguran con pernos de roca en retícula.

---

## 5.4 Métodos de medición de esfuerzos in-situ

| Técnica | Principio de funcionamiento | Rango de profundidad |
| --- | --- | --- |
| **Sobremuestreo (celda CSIRO HI)** | Mide las deformaciones de liberación de esfuerzos cuando un sondeo piloto se sobreperfora con un barril de diamante mayor | Hasta $30 - 50\text{ m}$ desde frentes subterráneos |
| **Fracturamiento hidráulico (hydrofrac)** | Aísla un tramo de sondeo con obturadores dobles y lo presuriza con agua hasta que la roca se fractura perpendicularmente a $\sigma_3$ | Sondeos de superficie $> 1.000\text{ m}$ |
| **Análisis de desconchamientos de sondeo** | Registros de calibre y televisor acústico detectan desconchamientos compresivos alineados diametralmente con la dirección de esfuerzo horizontal mínimo | Sondeos de exploración profundos |

---

## 5.5 Terminología canónica

| Español | Inglés | Vietnamita (canónico) | Definición |
| --- | --- | --- | --- |
| Esfuerzo in-situ / esfuerzo virgen | In-situ stress / Virgin stress | Ứng suất nguyên sinh | Campo de esfuerzos natural existente antes de la excavación |
| Esfuerzo inducido | Induced stress | Ứng suất kích ứng | Campo de esfuerzos redistribuido alrededor de una cavidad excavada |
| Solución de Kirsch | Kirsch solution | Lời giải Kirsch | Ecuaciones elásticas cerradas de esfuerzos alrededor de un sondeo circular |
| Esfuerzo tangencial / circunferencial | Tangential stress / Hoop stress | Ứng suất tiếp vòng biên | Esfuerzo que actúa tangente al perímetro de la excavación |
| Sobremuestreo | Overcoring | Phương pháp khoan chụp đo biến dạng giải phóng | Técnica de medición de esfuerzos que perfora por encima de un testigo piloto instrumentado |
