---
lang: es
lang_alt: reference-manuals/dunnicliff/chapter-11-calibration/
---

# Capítulo 11 — Calibración y Mantenimiento

## 11.1 Calibración: el punto de referencia

La lectura de un sensor no significa nada sin una relación conocida entre su salida y
la cantidad física. La **calibración** establece y mantiene esa relación.

## 11.2 Calibración de fábrica y de campo

- **Calibración de fábrica** proporciona la conversión tal como se entrega y un certificado de trazabilidad.
- **Calibración / verificación de campo** confirma que el instrumento aún funciona tras el transporte, la instalación y la exposición —porque las condiciones de campo desplazan la relación.

La recalibración periódica (o al menos la verificación contra una referencia) captura
la deriva antes de que corrompa el registro.

## 11.3 Programas de mantenimiento

Un plan de mantenimiento aborda:

- **Unidades de lectura y adquisidores** — función, reloj, energía.
- **Cables y conectores** — continuidad, ingreso de agua, daño por roedores.
- **Cero y span del sensor** — verificados contra lecturas manuales o de referencia.
- **Protección ambiental** — UV, corrosión, congelamiento.

## 11.4 Guías para clima frío

El congelamiento es una causa mayor de pérdida de datos:

- Enterre o caliente cables y sensores donde se necesite.
- Use anticongelante o gabinetes calefaccionados para tubos abiertos y lecturas.
- Documente un plan estacional, incluyendo apagado seguro y respaldo a lecturas manuales.

## 11.5 Documentación

Toda acción de calibración y mantenimiento se registra: fecha, método, resultado,
persona y cualquier cambio a los factores de conversión. Esto preserva la
defensibilidad de los datos durante la vida del instrumento.

!!! warning "La deriva es silenciosa"
    Un sensor no calibrado rara vez falla ruidosamente; deriva en silencio, corrompiendo
    tendencias hasta que alguien nota una lectura físicamente imposible. Programe la
    verificación; no espere el número imposible.

![Figure: dunnicliff-calibration](../../assets/figures/dunnicliff-calibration.svg)

**Figura.** Calibración. La relación entrada-salida (pendiente = factor de calibración), con cero, span e histéresis (Dunnicliff, caps. 7 y 16).

## 11.6 Puntos clave

- La calibración vincula la salida a la cantidad física; verifíquela en campo.
- Mantenga en un programa: lecturas, cables, cero, ambiente.
- Planee explícitamente para congelamiento y efectos estacionales.
- Registre toda acción de calibración y mantenimiento.
