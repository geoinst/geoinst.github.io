---
lang: es
lang_alt: reference-manuals/monitoring-dam-performance/chapter-11-data-management/
---

# Capítulo 11 — Adquisición, Gestión de Datos y Bases de Datos

## 11.1 Los datos solo importan si se pueden encontrar después

El objetivo de la gestión de datos es simple: toda lectura se captura, valida,
almacena y es recuperable durante décadas, con contexto suficiente para ser
interpretada por alguien que no estuvo ahí. La pérdida de datos es permanente; una
lectura no guardada bien podría no haberse tomado.

## 11.2 Frecuencia de adquisición

La frecuencia sigue la tasa de cambio y el plan del programa
([Capítulo 4](chapter-04-planning.md)):

- **Estado estable** — mensual a trimestral para variables lentas.
- **Construcción / primer llenado** — diario a semanal.
- **Tras eventos** — de forma intensiva, o continua vía automatización
  ([Capítulo 9](chapter-09-automated.md)).

## 11.3 Validación

Las lecturas en crudo no son datos hasta ser verificadas. La validación incluye:

- **Comprobaciones de rango** —¿es el valor físicamente posible?
- **Razonabilidad** —¿coincide con la tendencia y la estación?
- **Cruces** —¿están de acuerdo los instrumentos correlacionados?
- **Acuerdo manual vs. automatizado** para lecturas puntuales.

Los datos malos deben marcarse, no eliminarse en silencio.

## 11.4 Almacenamiento y bases de datos

Una base de datos de monitoreo debe registrar, para cada lectura:

- Identidad y ubicación del instrumento.
- Marca de tiempo y lector.
- Valor, unidades e incertidumbre.
- Contexto ambiental (nivel de embalse, temperatura, precipitación).

Prefiera formatos abiertos y portables y un sistema con una ruta de migración clara.
Las "cajas negras" propietarias que no pueden exportar son un riesgo a largo plazo.

## 11.5 La línea base como activo gestionado

La línea base de la operación temprana ([Capítulo 2](chapter-02-failure-modes.md))
es un activo gestionado. Almacénela explícitamente para que el "normal" futuro pueda
compararse con el "normal" de hoy a medida que la presa envejece.

## 11.6 Integración con el programa más amplio

Una buena gestión de datos vincula las lecturas al plan de monitoreo (por qué existe
cada instrumento) y a los hallazgos de inspección (para que una anomalía de
instrumento y una observación de campo puedan verse juntas).

## 11.7 Puntos clave

- Capture, valide y almacene toda lectura con contexto completo.
- Fije la frecuencia por la tasa de cambio, no por conveniencia.
- Marque los datos malos; nunca los elimine en silencio.
- Use sistemas portables y exportables; trate la línea base como un activo a largo
  plazo.
