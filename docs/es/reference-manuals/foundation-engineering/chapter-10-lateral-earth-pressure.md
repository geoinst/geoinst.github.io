---
lang: es
lang_alt: reference-manuals/foundation-engineering/chapter-10-lateral-earth-pressure/
---

# Capítulo 10 — Presión de Tierras Lateral

## 10.1 Los tres estados de presión de tierras

La presión que el suelo ejerce sobre una estructura de contención depende de cuánto
se permita mover la estructura:

- **Presión en reposo** ($K_0$) — el muro no se mueve; el suelo está en su estado
  natural. $K_0 \approx 1 - \sin\phi'$ para suelos normalmente consolidados.
- **Presión activa** ($K_a$) — el muro se mueve *alejándose* del suelo, que se
  expande y relaja hasta su presión mínima. Es la presión *mínima* que un muro debe
  resistir.
- **Presión pasiva** ($K_p$) — el muro se mueve *hacia* el suelo, que se comprime y
  empuja con su resistencia *máxima*. $K_p > K_0 > K_a$.

Los tres coeficientes se relacionan por $K_a = 1/K_p$ para el caso simple sin
fricción, y ambos dependen del **ángulo de fricción** $\phi'$ y de la fricción
muro–suelo $\delta$.

## 10.2 Teorías de Rankine y Coulomb

Dos teorías clásicas dan los coeficientes de presión:

- **Rankine** — supone un muro liso y vertical y relleno horizontal; simple y muy
  usado.
- **Coulomb** — admite fricción de muro y relleno inclinado, dando presiones más
  realistas (y a menudo activas menores); se resuelve gráfica o analíticamente.

Ambas suponen que el suelo alcanza un **estado plástico** y desprecian la rigidez de
interacción muro–suelo, por lo que son límites, no valores exactos.

## 10.3 Sobrecarga, agua y relleno estratificado

Los muros reales soportan más que el peso propio del suelo:

- **Sobrecarga** — cargas uniformes o puntuales tras el muro (tráfico, acopios,
  zapatas vecinas) añaden presión lateral.
- **Presión de agua** — el agua subterránea tras un muro añade presión hidrostática
  plena, a menudo la carga dominante. El **drenaje** es esencial; un muro diseñado
  solo para presión de suelos puede fallar al llenarse de agua.
- **Relleno estratificado e inclinado** — las presiones se calculan capa por capa.

## 10.4 Presión inducida por compactación

Compactar el relleno *detrás* de un muro con rodillos pesados puede fijar **presiones
laterales elevadas** que superan el valor activo, especialmente cerca de la
superficie. Es una causa frecuente de movimientos inesperados del muro y debe
considerarse en el diseño y en el método de compactación.

## 10.5 Puntos clave

- Tres estados: **en reposo, activa, pasiva** — la activa es el mínimo, la pasiva el
  máximo.
- **Rankine** es simple; **Coulomb** admite fricción de muro y relleno inclinado.
- **El agua suele ser la carga dominante** — aporte drenaje.
- La **sobrecarga** tras un muro añade presión; téngala en cuenta.
- La **compactación** puede fijar presiones por encima de la activa — controle el
  método.
