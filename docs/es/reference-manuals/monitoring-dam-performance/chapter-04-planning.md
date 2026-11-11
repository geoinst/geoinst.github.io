---
lang: es
lang_alt: reference-manuals/monitoring-dam-performance/chapter-04-planning/
---

# Capítulo 4 — Planificación de un Programa de Monitoreo de Presas

## 4.1 La planificación es el eje del programa

Un programa de monitoreo es tan bueno como el pensamiento que hay detrás. El error
más costoso es instalar instrumentos que no responden a las preguntas que importan.
La planificación debe ser un proceso deliberado y documentado.

## 4.2 El enfoque sistemático

Un proceso práctico de planificación sigue estos pasos:

1. **Conformar el equipo** — propietario, ingeniero de presas, geólogo, especialista
   en instrumentos.
2. **Caracterizar la presa** — tipo, geometría, cimentación, historial, consecuencias.
3. **Identificar los modos de falla potenciales (PFM)** — las formas creíbles en que
   la presa podría fallar ([Capítulo 2](chapter-02-failure-modes.md)).
4. **Definir las preguntas de desempeño** — para cada PFM, *¿qué necesitaríamos
   observar para detectar un avance hacia la falla?*
5. **Seleccionar indicadores y ubicaciones** — las mediciones y sus mejores posiciones.
6. **Elegir los instrumentos** — acordes al indicador, el ambiente y la precisión
   requerida.
7. **Definir frecuencias y umbrales** — con qué frecuencia leer y qué dispara la
   revisión ([Capítulo 9](chapter-09-automated.md), [Capítulo 12](chapter-12-evaluation.md)).
8. **Planificar la instalación y validación** — quién instala y cómo se verifican las
   lecturas.
9. **Planificar la operación y el mantenimiento** — mantener los instrumentos
   funcionando durante décadas.
10. **Planificar la gestión y evaluación de datos** — almacenamiento, validación,
    reportes.
11. **Documentar el programa** — un plan de monitoreo que el siguiente ingeniero
    pueda heredar.

## 4.3 Defina primero las preguntas de desempeño

Los buenos planes invierten el instinto habitual. En lugar de *"instalemos
piezómetros"*, la pregunta es *"¿cómo detectaríamos la erosión interna en esta
cimentación?"* — lo cual luego dicta piezómetros en ubicaciones y profundidades
específicas.

| Pregunta de desempeño | Indicador | Instrumento |
|-----------------------|-----------|-------------|
| ¿Aumenta o se vuelve erosiva la filtración? | Caudal y turbidez de la filtración | Vertederos, observaciones, piezómetros |
| ¿Se está estabilizando o moviendo el talud aguas abajo? | Movimiento superficial e interno | Topografía, inclinómetro, extensómetro |
| ¿Amenaza la presión de levantamiento a una presa de gravedad? | Presión de poros en la base | Piezómetros de levantamiento, medidores de juntas |

## 4.4 Emparejar el instrumento con la necesidad

Para cada indicador, seleccione una familia de instrumentos cuya precisión, rango y
durabilidad se ajusten a la tarea. Vea el [Capítulo 5](chapter-05-instruments.md)
para el menú. Evite sobre-especificar (la precisión innecesaria eleva el costo y la
tasa de falla) y sub-especificar (la resolución insuficiente oculta la señal).

## 4.5 Frecuencia y disparadores

La frecuencia de lectura debe reflejar la tasa de cambio esperada:

- Variables **estacionales** (embalse, presión de poros) → mensual a trimestral en
  estado estable.
- **Construcción o llenado** → diario a semanal.
- **Tras un evento** (inundación, sismo, anomalía) → de forma intensiva, incluso
  continua.

Los umbrales convierten lecturas en acción. Un *umbral* es un valor o tasa de cambio
que, al superarse, requiere revisión ([Capítulo 13](chapter-13-decisions.md)).

## 4.6 Costo de ciclo de vida, no solo costo inicial

El costo de un programa de monitoreo está dominado por décadas de operación,
mantenimiento y manejo de datos — no por el hardware inicial. Planifique desde el
inicio repuestos, calibración, recambio de personal y obsolescencia de los sistemas
de datos.

!!! example "Un plan documentado da frutos"
    Un plan de monitoreo por escrito permite que el programa sobreviva a los cambios
    de personal, respalda las revisiones de los reguladores y deja claro *por qué*
    existe cada instrumento — lo cual es precisamente cuando los recortes
    presupuestarios amenazan a los equivocados.

## 4.7 Puntos clave

- Planee a partir de modos de falla y preguntas de desempeño, no de una lista de
  compras.
- Seleccione instrumentos que emparejen el indicador, la ubicación y la precisión
  requerida.
- Establezca deliberadamente frecuencias de lectura y umbrales.
- Presupueste el ciclo de vida completo y escriba el plan.
