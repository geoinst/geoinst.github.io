---
lang: es
lang_alt: reference-manuals/practical-rock-engineering/chapter-07-structural-instability-tunnels/
---

# Capítulo 7 — Inestabilidad Controlada por la Estructura en Túneles

## 7.1 Liberación cinemática de cuñas poliédricas

En túneles de profundidad somera a intermedia excavados en macizos rocosos bloqueados y
diaclasados, la falla rara vez se produce por trituración de la roca intacta. El peligro
dominante son más bien **las caídas por gravedad de cuñas rocosas poliédricas**
delimitadas por discontinuidades que se cortan.

Para que una cuña se desprenda y caiga o deslice al vacío del túnel deben cumplirse dos
condiciones:
1. **Factibilidad cinemática**: la geometría de los planos de junta que se cortan debe
   formar una cuña tetraédrica o pentaédrica cerrada cuyo vértice apunte en dirección
   contraria al vacío de la excavación, y cuya dirección de deslizamiento que aflora
   hacia la apertura esté físicamente despejada.
2. **Inestabilidad por equilibrio límite**: las fuerzas motoras (peso gravitatorio de la
   cuña $W$ y presiones de agua en grietas de junta $U$) deben superar a las resistentes
   (cohesión de junta $c_j$, fricción $\sigma_n' \tan\phi_j$ y capacidad de los pernos
   de roca instalados $T$).

---

## 7.2 Proyección estereográfica y análisis cinemático

Las redes estereográficas (proyecciones de Wulff de ángulo igual o de Schmidt de área
igual) representan datos de orientación 3D (buzamiento $\psi$ y dirección de buzamiento
$\alpha$) sobre un plano 2D:

- **Círculos máximos**: representan planos de discontinuidades y frentes de excavación
  del túnel.
- **Polos**: vectores normales perpendiculares a los planos de discontinuidad.
- **Intersecciones ($\vec{I}_{12}$)**: el buzamiento ($\beta$) y el rumbo ($\theta$) de la
  recta de intersección formada por dos planos de junta:

$$\vec{I}_{12} = \vec{n}_1 \times \vec{n}_2$$

### Modos de deslizamiento:
- **Caída directa (desprendimientos de bóveda)**: el vértice de la cuña queda
  verticalmente sobre la clave; todos los planos que la delimitan buzan más que sus
  ángulos de fricción.
- **Deslizamiento en un solo plano**: la recta de intersección aflora, pero la cuña
  desliza por el más inclinado de los dos planos de junta mientras se separa del
  segundo.
- **Deslizamiento en dos planos**: la cuña desliza según la recta de intersección
  $\vec{I}_{12}$, manteniendo contacto simultáneo en ambas caras de junta.

```
          Bóveda del túnel
     +-------------------------+
      \        CUÑA           /
       \     (Peso W)        /
        \       /\          /
         \     /  \        /   Plano de junta 2
          \   /    \      /    (Buzamiento psi_2)
 Plano 1   \ /      \    /
 (Buz. psi_1)        v
             VECTOR DE DESLIZAMIENTO (Recta de intersección)
```

---

## 7.3 Cálculo por equilibrio límite: el método UNWEDGE

Para una cuña que desliza según la recta de intersección del Plano 1 y el Plano 2, con
buzamiento $\beta$:

### Fuerza motora ($F_{\text{motor}}$):

$$F_{\text{motor}} = W \sin\beta$$

### Fuerzas normales en las caras de junta ($N_1, N_2$):
Se resuelven por equilibrio de la cuña perpendicularmente a la recta de intersección:

$$N_1 + N_2 = W \cos\beta \cdot f(\text{geometría de la cuña})$$

### Fuerza resistente ($F_{\text{resist}}$):

$$F_{\text{resist}} = (c_1 A_1 + N_1' \tan\phi_1) + (c_2 A_2 + N_2' \tan\phi_2) + \sum T_b \cos\theta_b$$

donde $A_1, A_2$ son las áreas de las caras, $N'$ las fuerzas normales efectivas
reducidas por presiones de agua en grietas de poros, y $T_b$ la capacidad a tracción de
los pernos de roca que interceptan la cuña, orientados un ángulo $\theta_b$ respecto del
vector de deslizamiento.

$$FS = \frac{F_{\text{resist}}}{F_{\text{motor}}}$$

---

## 7.4 Diseño del soporte para cuñas de bóveda y hastiales

1. **Regla de soporte por peso propio**: los pernos de roca en retícula deben anclar el
  volumen máximo de cuña anticipado de vuelta a roca estable más allá de la envolvente
  de falla, con una longitud de empotramiento del anclaje $\ge 1,5 - 2,0\text{ m}$.
2. **Espaciamiento de pernos**: el espaciamiento $s$ debe ser menor que la dimensión
  mínima de la cara de cuña esperada para evitar que pequeños bloques caigan entre
  pernos:

$$s \le \frac{1}{2} \text{Dimensión de la cuña}$$

3. **Integración con shotcrete**: el shotcrete reforzado con malla o con fibra de acero
  (SFRS) aporta contención superficial inmediata, evitando que pequeños bloques clave
  se desgranen y desestabilicen cuñas mayores.

---

## 7.5 Terminología canónica

| Español | Inglés | Vietnamita (canónico) | Definición |
| --- | --- | --- | --- |
| Análisis cinemático | Kinematic analysis | Phân tích động học | Evaluación geométrica que determina si una cuña rocosa puede desprenderse físicamente |
| Proyección estereográfica | Stereographic projection | Phép chiếu lập thể cực | Representación gráfica 2D de orientaciones 3D de planos y rectas |
| Recta de intersección | Line of intersection | Đường giao tuyến | Vector formado por la intersección de dos planos de discontinuidad |
| Falla por cuña | Wedge failure | Phá hoại trượt nêm | Desprendimiento de un bloque rocoso poliédrico delimitado por juntas que se cortan |
| Bloque clave | Keyblock | Khối nêm khóa | Bloque superficial crítico cuya extracción desestabiliza los macizos rocosos adyacentes |
