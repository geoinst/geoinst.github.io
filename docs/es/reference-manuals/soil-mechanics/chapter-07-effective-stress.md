---
lang: es
lang_alt: reference-manuals/soil-mechanics/chapter-07-effective-stress/
---

# Capítulo 7 — Esfuerzo Efectivo y Presión de Poros

## 7.1 El principio del esfuerzo efectivo

El **principio de Terzaghi** es el fundamento de la mecánica de suelos:

$$\sigma' = \sigma - u$$

donde $\sigma$ es el **esfuerzo total** en un punto, $u$ es la **presión de agua en
los poros** y $\sigma'$ es el **esfuerzo efectivo** soportado por el esqueleto
sólido. **Todo aspecto del comportamiento del suelo —resistencia, rigidez y cambio
de volumen— depende del esfuerzo efectivo, no del esfuerzo total.**

## 7.2 Cálculo del esfuerzo total

El esfuerzo total a una profundidad es la suma de los pesos de todo lo que hay
encima:

$$\sigma_v = \sum \gamma_i h_i$$

usando el peso unitario apropiado para cada estrato —**bruto** por encima del nivel
freático, **saturado** por debajo.

## 7.3 Presión de poros

La presión de poros se mide con **piezómetros** (véanse las referencias
[Dunnicliff](../dunnicliff/index.md) y [FHWA](../fhwa/index.md)). Dos estados
importan:

- **Hidrostática (estacionaria)** — $u = \gamma_w z$, creciente con la profundidad
  bajo el nivel freático.
- **Exceso de presión de poros** — generado por carga o descarga más rápida de lo que
  el agua puede drenar; se disipa con el tiempo (consolidación).

## 7.4 Perfiles de esfuerzo efectivo

Combinando ambos se obtiene el **perfil de esfuerzo efectivo**. Observaciones clave:

- Bajo el nivel freático, el esfuerzo efectivo aumenta con el peso unitario
  **sumergido**, no con el saturado.
- Un gradiente de **filtración ascendente** reduce el esfuerzo efectivo; uno
  **descendente** lo aumenta.
- Donde el esfuerzo efectivo llega a **cero**, el suelo pierde toda resistencia
  (licuefacción, levantamiento, ebullición).

## 7.5 Por qué importa

El esfuerzo efectivo explica:

- **Consolidación** — asentamiento por disipación del exceso de presión de poros
  ([Capítulo 9](chapter-09-consolidation.md));
- **Resistencia al corte** — gobernada por $\sigma'$
  ([Capítulo 10](chapter-10-shear-strength.md));
- **Licuefacción** — pérdida de esfuerzo efectivo bajo carga cíclica; y
- **Estabilidad frente a filtración** — subpresión y tubificación
  ([Capítulo 6](chapter-06-seepage.md)).

## 7.6 Puntos clave

- **$\sigma' = \sigma - u$** — el principio central de la mecánica de suelos.
- El esfuerzo total es la **suma de pesos de estratos**; la presión de poros proviene
  de **piezómetros**.
- Bajo el nivel freático use el peso unitario **sumergido** para el esfuerzo
  efectivo.
- La **filtración cambia** el esfuerzo efectivo — el flujo ascendente lo reduce.
- El esfuerzo efectivo gobierna **consolidación, resistencia y licuefacción**.
