---
lang: es
lang_alt: reference-manuals/practical-rock-engineering/chapter-01-what-is-rock-engineering/
---

# Capítulo 1 — ¿Qué es la Ingeniería de Rocas?

## 1.1 Contexto histórico y evolución de la disciplina

La ingeniería de rocas surgió como disciplina de ingeniería diferenciada a mediados del
siglo XX. Antes de eso, la minería subterránea y la tunelización se trataban en gran
medida como oficios guiados por reglas empíricas, mientras que las excavaciones
superficiales tomaban prestadas las ideas de la mecánica de suelos sin espíritu crítico.

Las fallas catastróficas de mediados del siglo XX pusieron de manifiesto las carencias
letales de tratar los macizos rocosos como suelos homogéneos:

1. **Falla de la presa de Malpasset (Francia, 1959)**: una presa de arco de hormigón
   delgado colapsó catastróficamente durante su primer llenado, causando 423 muertos. No
   falló el hormigón de la presa: una zona de cizalle de foliación no cartografiada y
   planos de foliación desfavorablemente orientados bajo el estribo izquierdo se
   levantaron por la presión de agua en las grietas del embalse.
2. **Desastre del deslizamiento de Vajont (Italia, 1963)**: una masa rocosa colosal de
   270 millones de $\text{m}^3$ se desprendió a lo largo de intercalaciones arcillosas
   dentro de los planos de estratificación de la caliza, deslizándose al embalse a
   110 km/h. La ola de desplazamiento de 250 m resultante sobrepasó la presa y arrasó
   los valles aguas abajo, con más de 2.000 víctimas.
3. **Colapso de la mina de carbón de Coalbrook (Sudáfrica, 1960)**: un colapso masivo en
   cascada de más de 4.000 pilares de carbón en 3 $\text{km}^2$ atrapó y mató a 437
   mineros en minutos, demostrando que los diseños de pilares por área tributaria sin
   criterios de confinamiento fallan catastróficamente.

Estos desastres obligaron a los ingenieros civiles y de minas a reconocer que **el
comportamiento mecánico de un macizo rocoso no está gobernado por la resistencia del
material rocoso en sí, sino por las discontinuidades estructurales (juntas, fallas,
planos de estratificación) que lo cortan y por las presiones de fluido que actúan en el
interior de esas discontinuidades.**

---

## 1.2 Material rocoso frente a macizo rocoso

El cambio de paradigma central formulado por el Dr. Evert Hoek es la distinción
fundamental entre:

- **Roca intacta (material rocoso)**: el elemento de roca no fracturada entre
  discontinuidades estructurales, normalmente muestreado como cilindros de testigo
  intacto ($\approx 50\text{ mm}$ de diámetro). Se comporta como un sólido continuo,
  frágil y elástico cuya resistencia a compresión está determinada por la unión mineral
  y las microfisuras microscópicas.
- **Macizo rocoso**: el medio estructural in situ formado por bloques de roca intacta
  compartimentados por redes que se cortan de juntas, cizalles, superficies de
  estratificación y fallas. Un macizo rocoso es **discontinuo, anisotropo, no homogéneo
  y no elástico**.

```
+-------------------------------------------------------------------+
|                         MACIZO ROCOSO                             |
|                                                                   |
|   +----------------+      / /      +----------------+             |
|   |  Roca intacta  |     / /       |  Roca intacta  |             |
|   |     Bloque     |    / / Junta  |     Bloque     |             |
|   +----------------+   / /  Plano  +----------------+             |
|          \ \          / /                 \ \                    |
|           \ \  Falla / /                   \ \ Estratificación   |
|   +----------------+      / /      +----------------+             |
|   |  Roca intacta  |     / /       |  Roca intacta  |             |
|   |     Bloque     |    / /        |     Bloque     |             |
|   +----------------+   / /         +----------------+             |
+-------------------------------------------------------------------+
```

---

## 1.3 El efecto de escala en la mecánica de rocas

A medida que aumenta la escala del problema de ingeniería, desde probetas de laboratorio
hasta frentes de banco y envolventes de cavernas profundas, la resistencia a compresión
y el módulo de deformación medidos caen drásticamente.

$$\text{Resistencia}_{\text{Macizo Rocoso}} \ll \text{Resistencia}_{\text{Testigo Intacto de Laboratorio}}$$

- A una escala de $0,05\text{ m}$ (testigo de laboratorio), gobiernan la micromecánica
  de tracción y compresión de la roca intacta.
- A una escala de $1 - 5\text{ m}$ (perímetro de túnel o banco de mina), la estabilidad
  la dictan bloques poliédricos liberables cinemáticamente.
- A una escala de $> 30\text{ m}$ (talud global de mina a cielo abierto o gran cámara
  subterránea de trituración), la roca muy diaclasada se comporta como un
  pseudocontinuo equivalente gobernado por los criterios de macizo rocoso de
  Hoek-Brown.

---

## 1.4 El método observacional en ingeniería de rocas

Como los sondeos de exploración previos a la obra muestrean menos del $0,001\%$ del
volumen del macizo rocoso, un conocimiento geológico completo por anticipado es
matemáticamente imposible. Por ello la ingeniería de rocas se apoya en el **Método
Observacional** (Peck, 1969):

1. Establecer el diseño a partir del modelo geológico y geotécnico más probable.
2. Formular hipótesis explícitas sobre umbrales de deformación aceptables.
3. Instalar arreglos de instrumentación geotécnica (piezómetros, extensómetros, puntos
   de convergencia).
4. Medir de forma continua la respuesta del terreno durante la excavación progresiva.
5. Aplicar los Planes de Respuesta por Umbral de Activación (TARP) previamente previstos
   cuando las velocidades monitoreadas superan los límites de referencia.

---

## 1.5 Terminología canónica

| Español | Inglés | Vietnamita (canónico) | Definición |
| --- | --- | --- | --- |
| Roca intacta | Intact rock | Đá nguyên vẹn | Material rocoso no fracturado entre discontinuidades estructurales |
| Macizo rocoso | Rock mass | Khối đá | Medio in situ compuesto por bloques intactos y sistemas de discontinuidades |
| Discontinuidad | Discontinuity | Mặt bất liên tục | Término general para juntas, estratificación, cizalles y fallas |
| Presión de agua en grietas | Cleft water pressure | Áp lực nước khe nứt | Presión de fluido hidrostática e hidrodinámica que actúa en el interior de las aberturas de las juntas |
| Método Observacional | Observational Method | Phương pháp quan trắc | Metodología de diseño que acopla el avance de la obra con mediciones de campo en tiempo real |
