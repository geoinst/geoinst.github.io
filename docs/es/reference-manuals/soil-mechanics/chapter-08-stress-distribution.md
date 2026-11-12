---
lang: es
lang_alt: reference-manuals/soil-mechanics/chapter-08-stress-distribution/
---

# Capítulo 8 — Distribución de Esfuerzos en el Suelo

## 8.1 El problema

Una carga de cimentación se reparte en el terreno, de modo que el **incremento de
esfuerzo** $\Delta\sigma$ a una profundidad es *menor* que la presión aplicada y se
distribuye sobre un área *más amplia*. Cuantificar $\Delta\sigma$ con la profundidad
es esencial para los cálculos de **asentamiento**
([Capítulo 9](chapter-09-consolidation.md)) y para la **capacidad de carga**.

## 8.2 Teoría de Boussinesq

La **solución de Boussinesq** da el incremento de esfuerzo en un semiespacio
homogéneo, elástico e isótropo debido a una **carga puntual** en la superficie. A
partir de ella se construyen soluciones para:

- **zapatas corridas uniformemente cargadas** (deformación plana);
- **zapatas rectangulares y circulares**; y
- **cualquier forma**, por superposición o cartas de influencia.

El incremento de esfuerzo vertical bajo el **centro** de una carga circular flexible
de radio $R$ a profundidad $z$ es un resultado estándar, y las soluciones para
zapatas rectangulares se tabulan como **factores de influencia**.

## 8.3 El método 2:1 y reglas aproximadas

Una aproximación simple y muy usada es el **método 2:1**, que reparte la carga con
una pendiente de 2 en vertical por 1 en horizontal:

$$\Delta\sigma = \frac{Q}{(B+z)(L+z)}$$

Es burda pero útil para una primera estimación; para estructuras importantes se
prefieren soluciones más rigurosas.

## 8.4 Cartas de influencia de Newmark

La **carta de influencia de Newmark** es una herramienta gráfica: el área cargada se
dibuja a escala sobre la carta y el número de divisiones cubiertas da el factor de
influencia. Maneja formas irregulares que no tienen solución cerrada.

## 8.5 Bulbos de esfuerzo y profundidad de influencia

El **bulbo de esfuerzo** (o bulbo de presión) es el contorno dentro del cual
$\Delta\sigma$ supera una fracción elegida de la presión aplicada (p. ej., 10 % o
20 %). Muestra:

- la **profundidad de influencia significativa** — hasta dónde explorar y hasta qué
  estrato debe calcularse el asentamiento;
- la **extensión lateral** — hasta dónde pueden verse afectadas estructuras o
  servicios vecinos.

Como regla, la profundidad de influencia es del orden de **2 a 4 veces el ancho de la
zapata**.

## 8.6 Puntos clave

- Las cargas de cimentación **se reparten y atenúan** con la profundidad.
- La teoría de **Boussinesq** y los factores de influencia dan $\Delta\sigma$ para
  formas comunes.
- El **método 2:1** es una aproximación burda pero útil.
- Las **cartas de Newmark** manejan formas irregulares.
- El **bulbo de esfuerzo** fija la profundidad de exploración y de cálculo de
  asentamiento (típicamente **2–4 B**).
