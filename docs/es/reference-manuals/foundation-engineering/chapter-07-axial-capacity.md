---
lang: es
lang_alt: reference-manuals/foundation-engineering/chapter-07-axial-capacity/
---

# Capítulo 7 — Cimentaciones Profundas: Capacidad Axial

## 7.1 La ecuación de capacidad

La **capacidad axial última** de un pilote individual es la suma de la resistencia
del fuste y de la punta:

$$Q_{ult} = Q_s + Q_p - W$$

donde $Q_s$ es la **resistencia de fuste (fricción)**, $Q_p$ la **resistencia de
apoyo en punta** y $W$ el peso del pilote (a menudo despreciado). La **capacidad
admisible** es $Q_{ult}$ dividida por un factor de seguridad, y además debe satisfacer
el criterio de asentamiento.

## 7.2 Resistencia de fuste en arcilla

En arcilla, la resistencia de fuste se calcula normalmente con el **método de
esfuerzo total (α)**:

$$Q_s = \alpha \, c_u \, A_s$$

donde $c_u$ es la resistencia al corte no drenada, $A_s$ el área del fuste y $\alpha$
un factor de adhesión (típicamente ~0,5, decreciente con $c_u$). También se usa el
**método de esfuerzo efectivo (β)**, especialmente para condiciones a largo plazo.

## 7.3 Resistencia de fuste en arena

En arena, la resistencia de fuste se calcula con el **método de esfuerzo efectivo
(β)**:

$$Q_s = \beta \, \sigma'_v \, A_s = K \tan\delta \, \sigma'_v \, A_s$$

donde $\sigma'_v$ es el esfuerzo vertical efectivo, $K$ el coeficiente de presión de
tierras lateral y $\delta$ el ángulo de fricción pilote–suelo. Los métodos **λ** y
**α** son alternativas para condiciones específicas.

## 7.4 Apoyo en punta

El apoyo en punta depende de si la punta descansa sobre roca, arena densa o arcilla:

- **En arcilla:** $Q_p = 9 \, c_u \, A_p$ (con $c_u$ en la base).
- **En arena:** $Q_p = q'N_q A_p$ (o correlaciones con SPT/CPT), limitado para
  tener en cuenta la profundidad reducida en la que se moviliza la presión de apoyo.
- **Sobre roca:** capacidad a partir de la resistencia a compresión simple de la
  roca con factores de reducción.

## 7.5 Capacidad a partir de ensayos in-situ

El análisis estático se comprueba y a menudo se calibra con ensayos de campo:

- **Correlaciones SPT y CPT** — capacidad estimada de la resistencia a la
  penetración.
- **Ensayos de carga estática de pilotes** — la medición definitiva, con la carga
  aplicada por incrementos y el asentamiento registrado.
- **Ensayo dinámico (PDA)** — ensayos dinámicos de gran deformación durante el
  hincado dan capacidad e integridad.
- **Statnamic y ensayos de carga rápida** — alternativas cuando el ensayo estático
  es impracticable.

## 7.6 Ensayos de carga instrumentados

Los ensayos de carga más informativos están **instrumentados**: galgas
extensométricas o **barras hermanas** a lo largo del fuste y **testigos** o
**extensómetros** miden la distribución de carga entre fuste y punta, separando
directamente ambas componentes (véase la referencia [FHWA](../fhwa/index.md),
Capítulo 8, y los ejemplos del **Apéndice D**).

## 7.7 Factores de seguridad y LRFD

El diseño por esfuerzos admisibles usa un factor de seguridad sobre la capacidad
última (comúnmente 2,5–4 para cargas de trabajo). **LRFD** aplica en cambio
**factores de resistencia** por separado a las componentes de fuste y punta,
reflejando su distinta fiabilidad.

## 7.8 Puntos clave

- **$Q_{ult} = Q_s + Q_p$** — fricción de fuste más apoyo en punta.
- Use los **métodos α/β/λ** para el fuste y **9$c_u$ / $q'N_q$** para la punta.
- **Calibre** el análisis estático con **ensayos de carga, correlaciones SPT/CPT y
  ensayos dinámicos**.
- Los **ensayos de carga instrumentados** separan fuste de punta — el patrón de
  referencia.
- Esfuerzos admisibles usa un **factor de seguridad**; LRFD usa **factores de
  resistencia**.
