---
lang: es
lang_alt: reference-manuals/soil-mechanics/chapter-11-stiffness/
---

# Capítulo 11 — Rigidez y Esfuerzo–Deformación

## 11.1 Por qué importa la rigidez

La **rigidez** —cuánto se deforma un suelo ante un cambio de esfuerzo dado— gobierna
el **asentamiento**, la **distribución de carga** entre elementos estructurales y el
**movimiento** alrededor de excavaciones. Se mide con un **módulo** y, a diferencia de
la resistencia, es **altamente no lineal** y **dependiente de la deformación**.

## 11.2 Los parámetros elásticos

Para deformaciones pequeñas, el suelo se describe con:

- **Módulo de Young** $E$ — la pendiente esfuerzo–deformación en la dirección de
  carga.
- **Relación de Poisson** $\nu$ — la razón entre deformación lateral y axial
  (típicamente 0,2–0,5; 0,5 en condiciones no drenadas).
- **Módulo de corte** $G = E / [2(1+\nu)]$ — la resistencia a la distorsión por
  corte, a menudo el parámetro más útil para problemas dinámicos y de pequeña
  deformación.
- **Módulo volumétrico** $K$ — resistencia al cambio de volumen.

## 11.3 No linealidad y nivel de deformación

La rigidez del suelo **disminuye** al aumentar la deformación:

- **Deformación muy pequeña** ($< 0{,}001\%$) — rigidez máxima $G_0$ o $E_0$, medida
  por **métodos sísmicos** (bender element, CPT sísmico, MASW).
- **Deformación pequeña** — relevante para cimentaciones de maquinaria y carga
  dinámica.
- **Deformación de trabajo** ($0{,}01–1\%$) — relevante para la mayoría de
  asentamientos de cimentación; la rigidez es una fracción de $G_0$.
- **Gran deformación** — cercana a la falla; relevante para estabilidad.

El diseño debe usar el módulo **apropiado al nivel de deformación** del problema —una
fuente común de error es usar un único «módulo» para todos los casos.

## 11.4 Obtención de valores de módulo

- **Laboratorio** — los ensayos triaxiales o edométricos dan $E$ o el módulo
  confinado en un rango de deformación.
- **Campo** — presurómetro, dilatómetro, ensayo de placa de carga y métodos
  **sísmicos** dan valores in-situ, a menudo preferibles porque evitan la alteración
  de la muestra.
- **Correlaciones** — con el $N$ del SPT o la resistencia de punta del CPT, útiles
  como primera estimación.

## 11.5 Puntos clave

- La **rigidez gobierna el asentamiento** y la distribución de carga.
- La rigidez del suelo es **no lineal y dependiente de la deformación** — $G_0$ a
  pequeña deformación, mucho menor cerca de la falla.
- Use el módulo **apropiado al nivel de deformación** del problema.
- Los **métodos sísmicos** dan el módulo de pequeña deformación; los **ensayos de
  campo** dan valores de trabajo.
- Las **correlaciones** con SPT/CPT son un punto de partida, no un sustituto del
  ensayo.
