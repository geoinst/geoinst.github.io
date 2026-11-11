---
lang: es
lang_alt: reference-manuals/dunnicliff/chapter-05-uncertainty/
---

# Capítulo 5 — Incertidumbre de Medición y Sistemas de Adquisición de Datos

## 5.1 Toda medición es incierta

Ninguna lectura es exacta. Entender y gestionar la **incertidumbre de medición** es
lo que separa el monitoreo confiable de la precisión engañosa.

## 5.2 Conceptos clave

- **Exactitud** — cercanía al valor verdadero.
- **Precisión / repetibilidad** — cercanía de lecturas repetidas entre sí.
- **Histéresis** — la salida depende de la dirección del cambio (carga vs. descarga).
- **Ruido** — fluctuación aleatoria que enmascara la señal.
- **Presupuesto de error** — la suma de las incertidumbres individuales (sensor,
  cable, lectura, ambiente) que acota la incertidumbre total.

Un instrumento pequeño, preciso pero inexacto puede ser más engañoso que uno mayor y honesto.

## 5.3 Transductores: cómo "hablan" los instrumentos

La mayoría de los instrumentos modernos son **transductores** que convierten una
cantidad física en una señal eléctrica o neumática. Tipos comunes:

- **Cuerda vibratoria** — salida de frecuencia, robusta, muy usada.
- **Eléctrico (galga extensométrica, resistencia, capacitancia)** — versátil, sensible a efectos de cable.
- **Neumático** — equilibrio de presión de gas, sin energía.
- **Hidráulico** — equilibrio de columna líquida, método consolidado.

## 5.4 Sistemas de adquisición de datos (ADAS)

Un sistema de adquisición de datos escanea sensores, aplica conversión, marca
horario y almacena lecturas. Para monitoreo automatizado incluye telemetría y una
base de datos. La selección considera cantidad de canales, tasa de escaneo, energía,
endurecimiento ambiental y formatos de datos.

## 5.5 Gestión de la incertidumbre en la práctica

- Elija instrumentos cuya exactitud coincida con la decisión, no con la especificación máxima.
- Establezca y documente el presupuesto de error.
- Calibre y verifique (Capítulo 11).
- Reporte lecturas con su incertidumbre, no como decimales de falsa precisión.

!!! warning "La precisión no es exactitud"
    Una lectura que muestra `12.3456 kPa` no es más verdadera que `12.3 kPa`. Reporte
    a la resolución que el instrumento y la instalación realmente soportan.

## 5.6 Puntos clave

- Toda lectura lleva incertidumbre; gestione el presupuesto de error.
- Exactitud ≠ precisión; ambas importan, ninguna basta sola.
- Ajuste la exactitud del instrumento a la decisión, no al folleto.
- Los sistemas automatizados necesitan ADAS, telemetría y manejo de datos robustos.
