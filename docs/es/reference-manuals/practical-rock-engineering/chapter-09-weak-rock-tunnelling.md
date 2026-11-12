---
lang: es
lang_alt: reference-manuals/practical-rock-engineering/chapter-09-weak-rock-tunnelling/
---

# Capítulo 9 — Túneles en Roca Débil y Terreno de Aprisionamiento

## 9.1 Mecánica del terreno de aprisionamiento (squeezing)

Cuando túneles profundos se excavan en macizos rocosos débiles (lutitas, filitas,
esquistos, arcillolitas o harina de falla muy cizallada), los esfuerzos tangenciales
inducidos en el contorno ($\sigma_\theta$) superan la resistencia a compresión del
macizo rocoso ($\sigma_{cm}$).

En esas condiciones la roca no falla por desconchamiento frágil, sino que experimenta
**aprisionamiento dúctil dependiente del tiempo**: grandes deformaciones de corte
plásticas que fluyen hacia el interior de la apertura, produciendo convergencia severa
($> 5\% - 20\%$ del diámetro del túnel), pandeo de marcos de acero y rotura por cizalle
de revestimientos rígidos de hormigón.

### Índice de aprisionamiento de Hoek:
Hoek y Marinos (2000) correlacionaron la relación entre la resistencia a compresión del
macizo rocoso y el esfuerzo de sobrecarga in-situ ($\sigma_{cm} / \gamma H$) con la
deformación diametral esperada del túnel ($\epsilon = \Delta D / D$):

$$\frac{\sigma_{cm}}{\gamma H} = \frac{\sigma_{ci} \cdot s^a}{\gamma H}$$

| Relación $\sigma_{cm} / \gamma H$ | Deformación del túnel $\Delta D / D$ | Categoría de severidad e impacto operativo |
| --- | --- | --- |
| $> 1,0$ | $< 1\%$ | Pocos problemas de soporte; pernos de roca y malla estándar |
| $0,5 - 1,0$ | $1\% - 2,5\%$ | Aprisionamiento menor; marcos de acero ligeros o pernos en retícula con shotcrete |
| $0,3 - 0,5$ | $2,5\% - 5\%$ | Aprisionamiento moderado; soporte pesado instalado cerca del frente |
| $0,15 - 0,3$ | $5\% - 10\%$ | Aprisionamiento severo; arcos de acero cedentes, paraguas de micropilotes de avance |
| $< 0,15$ | $> 10\%$ | Aprisionamiento muy severo; colapso del frente, juntas cedentes en el shotcrete |

---

## 9.2 El método de convergencia-confinamiento (CCM)

El método de convergencia-confinamiento es el marco analítico de diseño estándar que
acopla tres curvas fundamentales:

```
Presión de soporte interna pi
      ^
  p_0 |  \ Curva de Reacción del Terreno (GRC)
      |    \
      |      \        Curva Característica del Soporte (SCC)
 p_eq |------- \-----/
      |         \   /
      |          \ / (Punto de equilibrio: u_eq, p_eq)
      |           v
      +-------------------------> Convergencia radial u_r
                 u_0  u_eq
```

1. **Curva de Reacción del Terreno (GRC)**: muestra el descenso de la presión de
   soporte interna $p_i$ necesaria para mantener el equilibrio a medida que la
   convergencia radial de las paredes $u_r$ crece desde el estado inicial
   ($p_i = p_0, u_r = 0$) hasta el estado sin confinamiento ($p_i = 0, u_r = u_{\max}$).
2. **Perfil de Deformación Longitudinal (LDP)**: relaciona la convergencia radial
   $u_r(x)$ con la distancia al frente de avance del túnel $x$. Aproximadamente el
   $25 - 35\%$ de la convergencia total ocurre *por delante* del frente, antes de que
   pueda instalarse el soporte.
3. **Curva Característica del Soporte (SCC)**: representa la respuesta carga–deformación
   elastoplástica del soporte instalado (pernos de roca, shotcrete, arcos de acero). El
   soporte debe instalarse con una convergencia inicial $u_0$ correspondiente a la
   distancia de retraso respecto del frente.

---

## 9.3 Filosofía de soporte rígido frente a soporte cedente

Intentar detener el aprisionamiento en terreno severo con revestimientos ultra rígidos
es imposible: el empuje inmenso del macizo rocoso ($p_0 = \gamma H$) triturará cualquier
cáscara de hormigón económicamente viable.

### La estrategia moderna de soporte cedente:
1. **Elementos cedentes dúctiles**: marcos de acero con uniones deslizantes por fricción
   (arcos TH) o cartuchos de acero cedentes (cilindros LSC) que se deforman
   plásticamente bajo una fuerza de resistencia controlada ($200 - 400\text{ kN}$).
2. **Juntas longitudinales en el shotcrete**: huecos dejados en el revestimiento de
   shotcrete paralelos al eje del túnel permiten el cierre radial sin provocar
   trituración compresiva en la cáscara. Una vez estabilizada la convergencia, las
   juntas se rellenan con hormigón.
3. **Pernos de roca cedentes (Swellex, D-Bolts)**: se deforman hasta $15 - 20\%$ de
   deformación unitaria sin rotura a tracción, manteniendo confinamiento continuo sobre
   el anillo plástico fracturado.

---

## 9.4 Terminología canónica

| Español | Inglés | Vietnamita (canónico) | Definición |
| --- | --- | --- | --- |
| Terreno de aprisionamiento | Squeezing ground | Đất đá ép lún | Deformación plástica inward dependiente del tiempo de la roca bajo sobreesfuerzo elevado |
| Método de Convergencia-Confinamiento (CCM) | Convergence-Confinement Method (CCM) | Phương pháp đường cong phản ứng nền (CCM) | Marco analítico que equilibra la convergencia de la roca con la reacción del soporte |
| Curva de Reacción del Terreno (GRC) | Ground Reaction Curve (GRC) | Đường cong phản ứng nền (GRC) | Relación entre la presión de soporte interna y el desplazamiento radial de las paredes |
| Perfil de Deformación Longitudinal (LDP) | Longitudinal Deformation Profile (LDP) | Biểu đồ biến dạng theo trục dọc hầm (LDP) | Convergencia radial de las paredes en función de la distancia al frente de avance |
| Soporte cedente | Yielding support | Kết cấu chống giữ dẻo hấp thu biến dạng | Soporte dúctil diseñado para deformarse plásticamente sin fallar |
