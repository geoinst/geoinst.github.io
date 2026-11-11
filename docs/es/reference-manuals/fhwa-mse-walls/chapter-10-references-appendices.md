---
lang: es
lang_alt: reference-manuals/fhwa-mse-walls/chapter-10-references-appendices/
---
# Capítulo 10 — Referencias y apéndices

## Referencias

La lista de referencias del manual abarca la literatura del suelo reforzado: el trabajo
original de tierra reforzada de Vidal; los volúmenes *Reinforced Soil Structures* de FHWA;
las *Bridge Design Specifications* de AASHTO; las guías de diseño geosintético; y la
literatura de investigación sobre arranque, fluencia, durabilidad y resistencia de
conexión. Es el punto de partida para cualquier parámetro que deba justificarse más allá
de las propias tablas del manual.

## Apéndice A — Determinación de los factores de resistencia de arranque

**A.1 Procedimientos empíricos para determinar $F^{*}$ y $\alpha$.** Para diseño
rutinario, el factor de fricción de arranque $F^{*}$ y el factor de corrección de escala
$\alpha$ se obtienen del ángulo de fricción del suelo y el tipo de refuerzo, usando las
gráficas empíricas del manual. Esta es la ruta por defecto cuando no se justifican
ensayos de arranque.

**A.2 Procedimientos experimentales para determinar $F^{*}$ y $\alpha$.** Donde la
combinación suelo–refuerzo es inusual, o donde los valores empíricos no son conservadores,
se realizan **ensayos de arranque**: el refuerzo se empotra en el relleno candidato y se
extrae bajo un esfuerzo normal conocido, y $F^{*}$ (y, para refuerzo extensible, $\alpha$)
se retro-calcula a partir de la resistencia medida. El apéndice da la configuración del
ensayo, la interpretación y la normalización.

**A.3 Resistencia y capacidad de conexión.** La conexión entre refuerzo y cara puede ser el
**eslabón más débil** del sistema. El apéndice describe ensayos de conexión para conexiones
de bloque segmentado/reforzamiento de fricción parcial y total, y cómo derivar la
resistencia de conexión de diseño a partir de los datos de carga–desplazamiento y ruptura.

## Apéndice B — Determinación del factor de reducción por fluencia

**B.1 Antecedentes.** El refuerzo geosintético fluye —se deforma continuamente bajo carga
sostenida— por lo que su resistencia a largo plazo es menor que su resistencia de corto
plazo. El **factor de reducción por fluencia** $RF_{CR}$ cuantifica la pérdida.

**B.2 Procedimientos paso a paso para extrapolar datos de ruptura por tensión.** Como una
estructura debe funcionar durante décadas, la resistencia a largo plazo no puede medirse
directamente. El apéndice da el procedimiento estándar: corra **ensayos de ruptura por
tensión** a temperaturas elevadas, use **superposición tiempo–temperatura** (factores de
desplazamiento) para construir una curva maestra, y **extrapole** hasta la vida de diseño
para encontrar la carga límite por fluencia.

**B.3 Uso de datos de fluencia de productos "similares".** Donde no hay datos específicos
del producto, pueden usarse datos de polímeros y estructuras similares con justificación.

**B.4 Ejemplos de extrapolación de fluencia.** Dos extrapolaciones totalmente desarrolladas
—una para un geosintético **PET** (poliéster) y otra para uno **poliolefínico**
(polipropileno/polietileno)— llevan datos de ruptura por tensión crudos a través del
desplazamiento y extrapolación a una carga límite por fluencia, y de ahí a $RF_{CR}$.

## Apéndice C — Rango de costo aproximado de geotextiles y georedes

Rangos de costo desactualizados para refuerzo geosintético, para estimación de orden de
magnitud. Reexpresar a precios locales actuales antes del uso.

## Apéndice D — Dimensiones típicas de refuerzos de acero

Secciones transversales, dimensiones y áreas estándar de las tiras de acero, mallas de
barras y mallas de alambre usadas en sistemas de refuerzo metálico —los datos tabulados
detrás del cálculo de margen por corrosión en el
[Capítulo 3](chapter-03-soil-reinforcement-principles.md).

## Apéndice E — Ejemplo de análisis de talud de suelo reforzado con el programa de computadora RSS

Un análisis de talud reforzado completo con el programa RSS de FHWA: geometría y
propiedades del suelo de entrada, la disposición del refuerzo, la búsqueda de la
superficie crítica, y el factor de seguridad resultante —el contraparte computacional de
los ejemplos manuales del [Capítulo 7](chapter-07-design-rss.md).

## Puntos clave

- Los **factores de arranque** vienen de gráficas por defecto, de **ensayos** cuando la
  combinación es inusual —Apéndice A.
- La **resistencia por fluencia** debe **extrapolarse** de ensayos acelerados, no asumirse
  —Apéndice B.
- La **resistencia de conexión** puede gobernar; ensáyela —Apéndice A.3.
- Los datos de costo (Apéndice C) y las dimensiones estándar (Apéndice D) son **datos de
  referencia desactualizados** —reexpresar y reverificar antes del uso.
- El Apéndice E es el **análisis computacional desarrollado** que cierra el ciclo de diseño.

---

## Lecturas relacionadas en esta base de conocimientos

- [Manual de Referencia de Instrumentación Geotécnica FHWA](../fhwa/index.md) — las
  familias de instrumentos entre las que selecciona el programa de monitoreo del Capítulo 9.
- [Dunnicliff — Instrumentación Geotécnica](../dunnicliff/index.md) — la filosofía de
  planificación sistemática detrás del programa de monitoreo.
- [Ingeniería de Cimentaciones](../foundation-engineering/index.md) — empuje de tierra,
  muros de contención y estabilidad de talud del corpus de dominio público USACE/FHWA.
- [Ingeniería de Rocas Práctica](../practical-rock-engineering/index.md) — la
  contraparte del lado de la roca para taludes de roca, anclas y concreto lanzado.
- [Monitoreo del Desempeño de Presas](../monitoring-dam-performance/index.md) — cómo los
  datos de movimiento y presión de poro se vuelven decisiones.
- [ADAQS (VI)](../../../vi/adaqs/index.md) — monitoreo automatizado y niveles disparador
  para vigilancia a largo plazo.
