---
lang: es
lang_alt: reference-manuals/fhwa-mse-walls/chapter-03-soil-reinforcement-principles/
---
# Capítulo 3 — Principios de refuerzo del suelo y propiedades de diseño del sistema

## 3.1 Visión general

Este capítulo es el puente entre elegir un sistema y diseñarlo. Responde dos
preguntas:

1. **¿Por qué funciona el suelo reforzado?** — la mecánica de interacción.
2. **¿Qué propiedades entran en las ecuaciones?** — los parámetros de suelo,
   refuerzo y durabilidad que consumen los capítulos de diseño.

## 3.2 Conceptos de suelo reforzado

Un relleno friccionante puede llevar esfuerzo compresivo y cortante, pero casi nula
tensión. Un elemento de refuerzo puede llevar tensión, pero casi nula compresión.
Combínelos y el compuesto puede llevar un esfuerzo *tensil* que no podría llevar solo
—que es por lo que la masa reforzada se comporta como si tuviera una **cohesión
aparente**, y puede sostenerse a un ángulo más empinado del que permite el ángulo de
fricción del relleno.

Dos mecanismos de transferencia llevan la carga entre el suelo y el refuerzo:

- **Fricción (y adhesión)** a lo largo de la superficie del refuerzo —dominante para
  tiras continuas y geotextiles.
- **Apoyo pasivo** del suelo contra miembros transversales —dominante para mallas,
  mallas de barras y tiras corrugadas, y un contribuyente significativo para las
  georedes.

La consecuencia de diseño es el **mecanismo de arranque**: el refuerzo es retenido por
el suelo a lo largo de una *longitud de empotramiento efectiva* detrás de la superficie
de falla potencial, y la tensión que lleva está limitada por la fricción y el apoyo que
esa longitud puede movilizar.

## 3.3 Interacción suelo–refuerzo usando conceptos normalizados

**Evaluación del desempeño de arranque.** La resistencia de arranque se normaliza
para que diferentes geometrías de refuerzo puedan compararse. La capacidad de arranque
de una capa se expresa como

$$P_r = F^{*}\ \alpha\ \sigma_v\ L_e\ C\ R_c$$

donde $F^{*}$ es el **factor de fricción de arranque** (una medida adimensional de la
interacción suelo–refuerzo), $\alpha$ es un **factor de corrección de escala**,
$\sigma_v$ es el esfuerzo vertical efectivo, $L_e$ es la longitud de empotramiento
efectiva detrás de la superficie de falla, $C$ es el perímetro del refuerzo (o
perímetro efectivo), y $R_c$ es la **relación de cobertura** (la fracción del ancho
del refuerzo que realmente está en contacto con el suelo, menor que 1 para mallas y
georedes con aberturas).

El **factor de fricción de arranque** $F^{*}$ se obtiene empíricamente a partir del
ángulo de fricción del suelo medido y el tipo de refuerzo, o experimentalmente a
partir de ensayos de arranque (Apéndice A):

- **Refuerzo inextensible (acero)** — $F^{*}$ se deriva del ángulo de fricción del
  suelo, con las tiras corrugadas añadiendo un componente de apoyo pasivo.
- **Refuerzo extensible (geosintético)** — $F^{*}$ combina la fricción superficial
  con el apoyo pasivo sobre los miembros transversales; el **factor de corrección de
  escala** $\alpha$ considera que el refuerzo extensible moviliza menos que su fricción
  total sobre longitudes de empotramiento largas. $\alpha = 1.0$ para refuerzo
  inextensible; para geosintéticos se toma 1.0 cerca de la superficie y se reduce con
  la profundidad (un valor por defecto de约 0.8 se usa comúnmente).

**Estimación de la capacidad de arranque en estructuras RSS y MSE.** La misma
expresión de $P_r$ se usa para ambas estructuras, pero la *longitud de empotramiento
efectiva* $L_e$ se mide detrás de una superficie de falla distinta —la superficie de
deslizamiento interno para muros MSE y la superficie de deslizamiento crítica para
taludes reforzados. La resistencia disponible se compara entonces con la tensión
movilizada:

$$FS_{(PO)} = \frac{P_r}{T_{max}}$$

con el factor de seguridad mínimo fijado por los criterios de diseño (comúnmente
$FS_{(PO)} \ge 1.5$).

**Cortante de interfaz.** Donde el refuerzo cruza una superficie de *deslizamiento
directo* o donde la interfaz cara–relleno-reforzado debe transferir carga, gobierna
la **resistencia al cortante de interfaz**. Se caracteriza por un ángulo de fricción de
interfaz, generalmente menor que el ángulo de fricción del propio suelo, y debe usarse
donde el deslizamiento a lo largo de un plano de refuerzo sea un mecanismo creíble.

## 3.4 Propiedades de ingeniería de la exploración y ensayo del sitio

**Suelos de cimentación.** La cimentación bajo la masa reforzada lleva el peso de toda
la estructura y debe satisfacer capacidad de carga, deslizamiento, asentamiento y
estabilidad global. Propiedades requeridas: peso unitario, resistencia al corte
(drenada y no drenada), compresibilidad y la profundidad a un estrato de apoyo
competente.

**Suelo de relleno reforzado.** El relleno reforzado es un **material estructural**,
no solo relleno. Debe ser friccionante y de drenaje libre. La especificación limita
típicamente:

- **Contenido de finos** e **índice de plasticidad** (los finos plásticos reducen la
  fricción y drenan mal).
- **Granulometría** (para asegurar drenaje y trabajabilidad).
- **Compactación** (para desarrollar el ángulo de fricción de diseño y limitar el
  asentamiento).

Un relleno granular típico podría tener un ángulo de fricción de 34°–40°; el valor de
diseño debe justificarse con ensayos, no asumirse.

**Relleno retenido.** El suelo detrás de la zona reforzada genera la presión de tierra
que la estructura resiste. Su peso unitario y ángulo de fricción son datos de entrada
para la estabilidad externa, y su drenaje determina si deben añadirse presiones
hidrostáticas.

**Propiedades electroquímicas.** Para el refuerzo de **acero**, la corrosividad del
relleno de respaldo gobierna el espesor de sacrificio y el requisito de recubrimiento;
el manual limita pH, resistividad, cloruros, sulfatos y contenido orgánico. Para el
refuerzo **geosintético**, la química gobierna la durabilidad del polímero, y también
se imponen límites. Estos límites son por lo que "cualquier relleno granular" no es
suficiente.

## 3.5 Establecimiento de propiedades de diseño estructural

**Características geométricas.** Ancho de refuerzo, espaciamiento (vertical y
horizontal), longitud, área de sección transversal y (para mallas) la geometría de
abertura y las dimensiones de las nervaduras. Para el acero, la sección transversal se
reduce a lo largo de la vida de diseño por la corrosión (ver abajo).

**Propiedades de resistencia.** La resistencia de diseño del refuerzo es su resistencia
**a largo plazo**, no su resistencia última de corto plazo:

- **Acero** — la resistencia tensil de diseño es la resistencia de fluencia de la
  sección *restante* tras deducir la **pérdida por corrosión de sacrificio** a lo largo
  de la vida de diseño. Deben considerarse tanto la pérdida del recubrimiento galvanizado
  como la del acero al carbono, a tasas que dependen de las propiedades electroquímicas
  del relleno de respaldo.
- **Geosintéticos** — la resistencia tensil admisible es la resistencia última reducida
  por factores parciales:

$$T_{allow} = \frac{T_{ult}}{RF_{CR}\ \cdot\ RF_{ID}\ \cdot\ RF_{D}}$$

donde $RF_{CR}$ es el factor de reducción por **fluencia**, $RF_{ID}$ el factor de
**daño por instalación** y $RF_{D}$ el factor de **durabilidad** (envejecimiento
químico/biological). El manual proporciona valores por defecto (Tabla 11) que solo
pueden usarse cuando el refuerzo y el relleno cumplen requisitos mínimos especificados;
de lo contrario los factores deben establecerse por ensayo —fluencia por extrapolación
de ruptura por tensión (Apéndice B), daño por instalación por ensayos de daño en campo,
y durabilidad por ensayos de inmersión.

**Resistencia de conexión.** Donde el refuerzo se conecta mecánicamente a la cara,
gobierna la **resistencia de conexión** (que puede ser menor que la del propio
refuerzo), y debe establecerse por ensayos de conexión —ver el
[Capítulo 4](chapter-04-design-mse-walls.md) y el Apéndice A.

## 3.6 Puntos clave

- El compuesto funciona porque la **fricción y el apoyo pasivo** aseguran el refuerzo;
  toda ecuación de resistencia es una afirmación sobre ese aseguramiento.
- Normalice el arranque como $P_r = F^{*}\alpha\sigma_v L_e C R_c$, y verifique
  $FS_{(PO)} = P_r/T_{max}$ contra el mínimo de diseño.
- El **relleno reforzado es un material estructural** —especifique su granulometría,
  plasticidad, compactación y electroquímica.
- Use resistencia de refuerzo a **largo plazo**: el acero pierde sección por
  corrosión; los geosintéticos pierden resistencia por fluencia, daño por instalación y
  envejecimiento.
- Establezca los factores de reducción por **ensayo** salvo que se cumplan las
  condiciones previas de los valores por defecto.
