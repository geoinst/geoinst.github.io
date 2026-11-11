---
lang: es
lang_alt: reference-manuals/tailings-dam-safety/chapter-11-data-management/
---

# Capítulo 11 — Adquisición, Gestión de Datos y Bases de Datos

## 11.1 De la lectura al registro

La salida cruda del sensor no es información. La cadena de datos —adquisición,
validación, almacenamiento y recuperación— determina si las mediciones se convierten en
evidencia defendible del desempeño.

## 11.2 Frecuencia de lectura

La frecuencia la fijan:

- **Dinámica del parámetro** (presión de poros y movimiento durante una tormenta cambian
  rápido; el asentamiento lentamente).
- **Etapa de vida** (puesta en servicio y llenado máximo necesitan más; operación estable
  menos).
- **Categoría de riesgo** (mayor consecuencia → más frecuente, a menudo automatizada).

Una frecuencia mínima se documenta en el plan; los aumentos provocados por eventos
siguen tormentas, sismos o anomalías.

## 11.3 Validación y control de calidad

Antes de entrar al registro, los datos deben verificarse para:

- **Verosimilitud** (dentro del rango, sin saltos salvajes).
- **Continuidad** (huecos explicados, no ocultos).
- **Deriva de calibración** (comparada con controles manuales y calibración de fábrica).
- **Correlación ambiental** (p. ej., efectos de temperatura removidos).

!!! warning "Los huecos también son datos"
    Una lectura faltante es un hallazgo. Investigue y documente los huecos en lugar de
    interpolar en silencio. Un patrón de huecos en un instrumento crítico es en sí mismo
    una alarma.

## 11.4 Bases de datos y recuperación

Una base de datos estructurada (no hojas de cálculo dispersas) respalda:

- Gráficas de serie de tiempo por instrumento y parámetro.
- Gráficas cruzadas (p. ej., movimiento vs. presión de poros).
- Rastro de auditoría y control de acceso.
- Continuidad a largo plazo a medida que el personal y los instrumentos rotan.

## 11.5 Preservación y traspaso

Los registros de monitoreo deben sobrevivir a cualquier individuo o contrato. Archive
datos crudos y procesados, registros de instalación y notas de revisión en una forma que
sobreviva al **cierre y la transferencia de propiedad**. El registro es la memoria de la
instalación.

## 11.6 Puntos clave

- La calidad de la cadena de datos determina si las lecturas se convierten en evidencia.
- Fije la frecuencia por parámetro, etapa de vida y riesgo.
- Valide verosimilitud, continuidad y calibración; documente los huecos.
- Archive a largo plazo, a través del cierre y el cambio de propiedad.
