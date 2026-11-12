---
lang: es
lang_alt: reference-manuals/practical-rock-engineering/chapter-10-large-underground-caverns/
---

# Capítulo 10 — Diseño de Grandes Cavernas Subterráneas

## 10.1 Geometría y secuencia de excavación en cavernas subterráneas

Las grandes cavernas subterráneas (casas de máquinas hidroeléctricas, salas de
transformadores, cámaras de trituración de minas subterráneas e instalaciones de
defensa) presentan luces superiores a $20 - 35\text{ m}$ y alturas de muro que alcanzan
$40 - 60\text{ m}$.

A esas dimensiones, la excavación en una sola pasada es imposible. Las cavernas deben
desarrollarse mediante avance y banqueo secuencial en varias etapas:

```
Paso 1: Galería piloto de avance superior (avance con pernos de roca y shotcrete en bóveda)
Paso 2: Ensanches de bóveda (ampliar la clave a toda la luz; instalar cable-pernos)
Paso 3: Excavación del banco 1 (banco central descendiendo 3-5 m; soporte en retícula de hastiales)
Paso 4: Bancos 2 a N (banqueo secuencial descendente, manteniendo el soporte de hastiales)
Paso 5: Excavación de contrabóveda y conexión de la galería de drenaje
```

---

## 10.2 Orientación del eje de la caverna frente a esfuerzos in-situ y familias de juntas

La orientación de la caverna es la decisión de diseño más importante:

1. **Alineación con el esfuerzo horizontal mayor ($\sigma_H$)**:
   - El eje longitudinal de la caverna debe disponerse paralelo (o dentro de
     $15^\circ - 20^\circ$) a la dirección de la tensión principal horizontal máxima
     ($\sigma_H$).
   - Esto minimiza los esfuerzos de compresión elevados que actúan transversalmente a
     los hastiales de la caverna, evitando pandeo masivo de hastiales y zonas de cizalle
     profundas.
2. **Alineación relativa a las familias de juntas dominantes**:
   - El eje de la caverna debe evitar disponerse paralelo a familias de juntas
     persistentes de buzamiento empinado o a fallas.
   - Si una falla corre paralela a un hastial alto y largo, se forman bloques en cuña de
     miles de toneladas que exigen un reforzamiento con anclas de cable antieconómico.

---

## 10.3 Diseño de cable-pernos pretensados para cavernas

Los pernos de roca estándar ($3 - 5\text{ m}$ de longitud) son insuficientes para
reforzar las zonas de fluencia plástica profundas ($6 - 15\text{ m}$ de profundidad) que
rodean las cavernas grandes. Son obligatorios cable-pernos pretensados de alta capacidad
($15 - 25\text{ m}$ de longitud, $500 - 1.000\text{ kN}$ de capacidad):

### Componentes del ancla de cable:
- **Tendón**: varios cordones de acero de alta resistencia de 7 alambres ($15,2\text{ mm}$
  de diámetro, capacidad última $260\text{ kN}$ por cordón).
- **Longitud de adherencia (zona de anclaje)**: tramo fijo inyectado con resina o cemento
  ($5 - 8\text{ m}$) anclado en roca virgen elástica más allá de la zona de fluencia.
- **Longitud libre**: tramo enfundado o sin adherencia que permite el alargamiento
  elástico durante el tesado.
- **Cabeza de anclaje y placa de reparto**: placa de acero de gran tamaño que distribuye
  el esfuerzo sobre almohadillas de shotcrete reforzado.

$$\text{Carga de trabajo de diseño } T_{\text{work}} \le 0,60 - 0,70 T_{\text{ult}}$$

---

## 10.4 Arreglos de instrumentación 3D en cavernas grandes

El monitoreo durante el banqueo de la caverna aporta el bucle de realimentación que
valida los modelos numéricos (análisis por elementos de frontera y elementos finitos):

| Instrumento | Ubicación y arreglo | Objetivo principal del monitoreo |
| --- | --- | --- |
| **Extensómetros multipunto de sondeo (MPBX)** | Abanicos radiales desde bóveda y hastiales altos ($10, 20, 30\text{ m}$ de profundidad) | Mide la profundidad de dilatancia de la roca y verifica que las longitudes de adherencia de las anclas de cable permanezcan ancladas en roca inmóvil |
| **Medidores de esfuerzo de sondeo (cuerda vibrante)** | Celdas biaxiales instaladas en pilares rocosos de hastiales | Mide concentraciones de esfuerzo entre cavernas adyacentes de casa de máquinas y transformadores |
| **Células de carga en cable-pernos** | Bajo las placas de reparto de las cabezas de anclaje | Registra de forma continua si la dilatancia de la roca está sobrecargando los tendones hacia la rotura a tracción |
| **Dianas de convergencia (RTS óptica)** | Puntos en retícula sobre bóveda y hastiales de la caverna | Mide vectores de cierre 3D durante voladuras sucesivas de bancos inferiores |

---

## 10.5 Terminología canónica

| Español | Inglés | Vietnamita (canónico) | Definición |
| --- | --- | --- | --- |
| Caverna subterránea | Underground cavern | Buồng ngầm quy mô lớn | Excavación subterránea de gran luz y gran altura de muro |
| Cable-perno pretensado | Pre-stressed cablebolt | Cáp neo dự ứng lực | Ancla larga de cordones de acero de alta capacidad, pretensada contra la roca |
| Longitud libre | Free length | Đoạn tự do của neo | Tramo sin adherencia de un ancla que se alarga elásticamente |
| Longitud de adherencia | Bond length | Đoạn neo bầu / Chiều dài đoạn ngàm | Tramo fijo inyectado que transmite la carga al macizo rocoso |
| Banqueo secuencial | Sequential benching | Đào hạ tầng giật cấp | Método de excavación descendente que retira roca en bancos horizontales progresivos |
