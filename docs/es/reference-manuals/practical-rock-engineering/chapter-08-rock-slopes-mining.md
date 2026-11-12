---
lang: es
lang_alt: reference-manuals/practical-rock-engineering/chapter-08-rock-slopes-mining/
---

# Capítulo 8 — Taludes de Roca en Ingeniería Civil y Minería a Cielo Abierto

## 8.1 El espectro de escala de los taludes de mina

Los taludes rocosos de minas a cielo abierto operan en tres escalas geométricas bien
diferenciadas:

1. **Escala de banco ($10 - 30\text{ m}$ de altura)**: la estabilidad está controlada por
   fallas cinemáticas planares, en cuña y por vuelco a lo largo de superficies de junta
   individuales. Su función principal es proporcionar el ancho de berma de captación
   ($b \ge 0,2 H + 4,5\text{ m}$) que retiene la roca que se desgrana.
2. **Escala de interrampa ($50 - 200\text{ m}$ de altura)**: gobernada por la
   persistencia de fallas, las presiones de agua subterránea tras el frente y la
   integridad de las pistas de acarreo.
3. **Escala de talud global ($300 - 1.000\text{ m}$ de profundidad)**: estabilidad
   global masiva gobernada por falla de corte no lineal del macizo rocoso (criterio de
   Hoek-Brown), zonas de falla regionales y recarga de acuíferos regionales.

---

## 8.2 Mecanismos principales de falla en taludes de roca

```
A. DESLIZAMIENTO PLANO      B. DESLIZAMIENTO EN CUÑA     C. FALLA POR VUELCO
    |  /                        |   / \                     | ||||
    | / (Buz. psi_p)            |  /   \ (Intersecc.)       | |||| (Juntas empinadas
    |/                          | /     \                   |/////  buzando al interior)
```

### 1. Falla planar
Ocurre a lo largo de una única junta persistente con rumbo paralelo ($\pm 20^\circ$) a la
cara del talud y buzamiento que aflora ($\phi < \psi_p < \psi_f$):

$$FS = \frac{c A + (W \cos\psi_p - U - V \sin\psi_p) \tan\phi}{W \sin\psi_p + V \cos\psi_p}$$

Donde:
- $W$ = peso del bloque de roca deslizante
- $A$ = área de la base de deslizamiento
- $U$ = fuerza de subpresión de agua de poros sobre el plano de deslizamiento:
  $U = \frac{1}{2} \gamma_w z_w A$
- $V$ = fuerza hidrostática horizontal del agua en grietas que actúa en las grietas de
  tracción tras la cresta: $V = \frac{1}{2} \gamma_w z_w^2$

### 2. Falla en cuña
Ocurre a lo largo de la recta de intersección de dos planos de junta que buzan más
suave que la cara del talud, pero más empinado que su ángulo de fricción combinado.

### 3. Falla por vuelco
Ocurre cuando familias de juntas buzan empinadamente *hacia el interior* de la cara del
talud ($\psi_d + \psi_f \ge 90^\circ + \phi$). El momento gravitatorio hace que columnas
altas de roca se inclinen hacia fuera, abriendo juntas transversales de base y volcando
ladera abajo.

### 4. Falla circular / compuesta del macizo rocoso
Ocurre en macizos muy fracturados, muy meteorizados o alterados ($GSI < 40$), donde la
fábrica estructural no impone una trayectoria de deslizamiento planar preferente. Se
analiza mediante Bishop, Morgenstern-Price o modelado numérico por reducción de la
resistencia al corte (SSR).

---

## 8.3 El papel catastrófico del agua subterránea

El agua subterránea es el mayor factor motor de los colapsos de taludes de mina a cielo
abierto:
1. **Reduce el esfuerzo efectivo**: la presión de poros del fluido ($u$) se resta
   directamente del esfuerzo normal de apriete: $\sigma' = \sigma - u$.
2. **Fuerza hidrostática en grietas ($V$)**: la lluvia que llena las grietas de tracción
   tras la cresta del tajo introduce enormes fuerzas laterales motoras sin resistencia
   de fricción alguna.
3. **Acelera la alteración química**: la meteorización del relleno de harina arcillosa
   reduce los ángulos de fricción residual de $25^\circ$ a $8^\circ$.

### Diseño de drenaje de descompresión
- Sondeos de drenaje subhorizontales ($75 - 100\text{ mm}$ de diámetro, entubado de PVC
  perforado) perforados $50 - 150\text{ m}$ dentro de los muros altos hacen descender la
  línea freática y elevan el Factor de Seguridad del talud entre un $20 - 40\%$ sin
  mover roca.

---

## 8.4 Monitoreo de taludes de mina a cielo abierto

| Sistema de instrumentación | Parámetro medido | Papel en la alerta temprana |
| --- | --- | --- |
| **Radar terrestre (SSR)** | Desplazamiento según la línea de visión (LOS) | Escanea todo el tajo 24/7; aporta mapas de calor en tiempo real de velocidad acelerada ($mm/h$) |
| **Estaciones totales robotizadas (RTS)** | Vector de coordenadas 3D $(x,y,z)$ | Monitoreo de alta precisión de prismas instalados en pistas de acarreo y crestas |
| **Piezómetros de cuerda vibrante (VWP)** | Presión de agua de poros profunda ($u$) | Verifica la eficacia de los drenes horizontales y de los pozos de bombeo de desagüe |
| **Inclinómetros in situ (IPI)** | Desplazamiento de cizalle profundo frente a profundidad | Identifica la profundidad exacta de la superficie basal de cizalle bajo el fondo del tajo |

---

## 8.5 Terminología canónica

| Español | Inglés | Vietnamita (canónico) | Definición |
| --- | --- | --- | --- |
| Berma de captación | Catch berm | Cơ tầng lưu giữ đá rơi | Banca horizontal dejada entre taludes empinados para capturar roca caída |
| Falla planar | Planar failure | Phá hoại trượt phẳng | Deslizamiento de un bloque rocoso a lo largo de un único plano continuo |
| Falla por vuelco | Toppling failure | Phá hoại trượt lật | Vuelco rotacional de columnas rocosas empinadas que buzan hacia el talud |
| Grieta de tracción | Tension crack | Vết nứt tách đỉnh | Rotura por tracción que se abre tras la cresta antes del deslizamiento |
| Dren de descompresión | Depressurization drain | Lỗ khoan tháo khô hạ áp | Sondeo subhorizontal perforado en la roca para hacer descender el nivel freático |
