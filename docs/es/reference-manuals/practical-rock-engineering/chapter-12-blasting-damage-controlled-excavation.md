---
lang: es
lang_alt: reference-manuals/practical-rock-engineering/chapter-12-blasting-damage-controlled-excavation/
---

# Capítulo 12 — Daño por Voladura y Técnicas de Excavación Controlada

## 12.1 Física del daño inducido por voladura en la roca

La voladura fragmenta la roca mediante dos procesos físicos distintos:

1. **Onda de choque de alta velocidad**: un pulso compresivo instantáneo
   ($V_p \approx 3.000 - 6.000\text{ m/s}$) viaja radialmente hacia fuera desde el
   taladro detonado. Al reflejarse en las caras libres como onda de tracción, crea
   extensas microfisuras radiales alrededor del barreno.
2. **Presión de expansión de los gases de explosión**: gases a alta presión y alta
   temperatura ($P_{\text{gas}} \approx 1.000 - 5.000\text{ MPa}$) penetran en las
   fisuras radiales inducidas por el choque, las abren en cuña y empujan la roca
   fragmentada hacia el vacío.

### La zona de daño por voladura:
En voladuras de producción, las cargas con exceso de confinamiento trituran la roca
mucho más allá del contorno de excavación previsto. Esto crea una **envolvente de daño
por voladura** ($0,5 - 2,0\text{ m}$ de profundidad tras muros altos y bóvedas de
túnel) caracterizada por aberturas de juntas dilatadas, puentes de roca intacta
triturados y ángulos de fricción destruidos ($D \to 1,0$ en el criterio de Hoek-Brown),
lo que desencadena desprendimientos severos de roca.

---

## 12.2 Métodos de voladura controlada

Para preservar la competencia estructural de los muros altos finales y de los perímetros
de túnel se emplean técnicas de voladura controlada de contorno:

```
A. PRE-CORTE (Muros altos)                  B. VOLADURA SUAVE (Perímetros de túnel)
   [o] [o] [o] [o] [o]  (Taladro de amortiguación sin carga)  [X]  [X]  (Disparan primero las rondas de producción)
    |   |   |   |   |                                            \   /
   =================== (Fisura de cizalle de separación)       [o]-[o]-[o] (Los taladros de contorno disparan AL FINAL)
   Se dispara ANTES de la ronda de producción                   Cargas amortiguadas recortan el contorno final
```

| Técnica | Configuración de perforación | Carga de explosivo | Secuencia de temporización |
| --- | --- | --- | --- |
| **Pre-corte (pre-splitting)** | Taladros muy próximos ($s \approx 8 - 12 d_{\text{taladro}}$) perforados a lo largo de la línea de contorno de diseño | Cargas ligeras desacopladas y amortiguadas (con cámara de aire o cordones de explosivo de traza) | Se disparan **simultáneamente ANTES** de que detone cualquier taladro de producción |
| **Voladura suave (voladura de contorno)** | Taladros de contorno muy próximos ($s \approx 15 - 16 d_{\text{taladro}}$) con relación burden/espaciamiento $B/s \approx 1,2 - 1,5$ | Cartuchos ligeros desacoplados | Se disparan en el **ÚLTIMO intervalo de retardo**, después de excavada toda la roca de burden interior |
| **Voladura amortiguada (recorte)** | Fila única de taladros de recorte perforada junto al muro final | Carga ligera con amortiguadores de retacado | Se dispara tras retirar el escombro principal para recortar bordes de banco irregulares |

---

## 12.3 Velocidad Pico de Partícula (PPV) y umbrales de daño

Las ondas de vibración que viajan por la roca se cuantifican mediante la **Velocidad Pico
de Partícula (PPV)**, medida con sismógrafos de velocidad de 3 ejes (geófonos):

### Ley empírica de distancia escalada de vibración del USBM:

$$\text{PPV} = K \left( \frac{R}{\sqrt{Q}} \right)^{-B}$$

donde $R$ es la distancia al punto de voladura ($\text{m}$), $Q$ la carga máxima de
explosivo por retardo ($\text{kg}$) y $K, B$ constantes de transmisión del sitio.

### Criterios de daño al macizo rocoso:
- **$\text{PPV} < 50\text{ mm/s}$**: riesgo despreciable para roca fresca; aceptable para
  revestimientos de hormigón próximos e infraestructura de ingeniería.
- **$\text{PPV} \approx 100 - 250\text{ mm/s}$**: inicio de apertura menor de juntas y
  desgranamiento de bloques clave sueltos en techos sin soportar.
- **$\text{PPV} \approx 400 - 700\text{ mm/s}$**: umbral crítico de daño permanente;
  se inician nuevas fracturas de tracción en puentes de roca intacta.
- **$\text{PPV} > 1.000\text{ mm/s}$**: trituración total de la roca intacta; equivalente
  a la zona de machaqueo alrededor de los taladros de explosivo.

---

## 12.4 Arreglos de monitoreo de vibración por voladura

Para evitar dañar muros altos y cavernas subterráneas circundantes:
- Instalar arreglos de geófonos triaxiales en la cresta de los bancos de mina a cielo
  abierto para asegurar que la voladura de contorno no supera $\text{PPV} \le 150\text{ mm/s}$.
- Vincular los sismógrafos a pasarelas digitales ADAQS para generar informes de
  conformidad instantáneos y optimizar las secuencias de detonadores electrónicos de
  retardo (intervalos de temporización de milisegundos).

---

## 12.5 Terminología canónica

| Español | Inglés | Vietnamita (canónico) | Definición |
| --- | --- | --- | --- |
| Pre-corte / voladura de tajo previo | Pre-splitting | Nổ mìn tạo khe trước / Nổ tách trước | Disparo simultáneo de taladros de contorno desacoplados antes de la voladura de producción |
| Voladura suave | Smooth blasting | Nổ mìn tạo biên nhẵn | Disparo de cargas ligeras de contorno en el último retardo para producir una bóveda limpia |
| Carga desacoplada | Decoupled charge | Lượng thuốc nổ không tiếp xúc thành lỗ | Carga de explosivo cuyo diámetro es menor que el del taladro |
| Velocidad Pico de Partícula (PPV) | Peak Particle Velocity (PPV) | Vận tốc dao động hạt cực đại (PPV) | Velocidad máxima de las partículas de vibración del terreno durante el paso de la onda |
| Distancia escalada | Scaled distance | Khoảng cách tỷ lệ | Razón geométrica que relaciona la distancia con la raíz cuadrada de la carga de explosivo |
