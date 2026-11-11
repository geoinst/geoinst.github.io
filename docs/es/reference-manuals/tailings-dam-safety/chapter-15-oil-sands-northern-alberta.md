---
lang: es
lang_alt: reference-manuals/tailings-dam-safety/chapter-15-oil-sands-northern-alberta/
---

# Capítulo 15 — Estudio de Caso: Presas de Relaves de Arenas Bituminosas del Norte de Alberta

!!! note "Acerca de este estudio de caso"
    Este capítulo es un **estudio de caso original** escrito para esta referencia.
    Sintetiza la guía de práctica disponible públicamente para la industria de las
    arenas bituminosas del norte de Alberta —principalmente el artículo del Boletín de
    la CDA *"Aplicación de las Guías de Seguridad de Presas de la CDA al Diseño
    Geotécnico de Presas de Relaves de Arenas Bituminosas en el Norte de Alberta"*
    (Eshraghian & Becker, Golder Associates, **Boletín de la Canadian Dam Association,
    Invierno 2016**) y el artículo de conferencia complementario *"Aplicación de
    Instrumentación Geotécnica en el Monitoreo del Desempeño de Diques en Fosa (In-Pit
    Dykes)"* (Soe Moe & Biggar, 2013). Es un **estudio de caso didáctico**, no una
    reproducción de esas fuentes ni un documento de diseño. La región de las arenas
    bituminosas está regulada por el **Alberta Energy Regulator (AER)** bajo la
    *Guía Técnica de Seguridad de Presas*; trabaje siempre a partir de la guía actual
    del AER/CEA.

Las presas de relaves de arenas bituminosas son, en palabras del artículo fuente, *"entre
las terceras reservas de petróleo comprobadas más grandes del mundo"* —una escala que
hace que sus estructuras de contención sean algunas de las presas de relaves más exigentes
en cualquier parte. Sin embargo, **no son presas de retención de agua**, y la distinción
es toda la razón de ser de este estudio de caso: se construyen durante décadas alrededor
de una operación minera activa, contienen un material que puede licuarse, y se rigen por
un régimen de seguridad de presas escrito pensando en las presas de agua. Aplicar ese
régimen inteligentemente —en lugar de mecánicamente— es la historia de ingeniería.

---

## 15.1 El escenario: por qué el norte de Alberta es un caso especial

### 15.1.1 Ubicación y escala

Los depósitos de arenas bituminosas (arenas bituminosas) yacen en el **norte de
Alberta**, dentro de la región del **Athabasca** principalmente, con áreas menores en
**Cold Lake** y **Peace River**. Las condiciones económicas actuales limitan la mayoría
de la minería activa a depósitos dentro de unos **75 m de la superficie**; aproximadamente
el **20 % del recurso es accesible a minería superficial**, el resto por métodos in situ.
La figura siguiente (de datos del Alberta Geological Survey, según Eshraghian & Becker)
muestra las tres áreas de depósito.

> **Referencia de figura.** La Figura 1 del artículo fuente muestra las áreas de
> arenas bituminosas de Athabasca, Cold Lake y Peace River a través de Alberta. (No se
> reproduce aquí.)

### 15.1.2 El proceso de minería y extracción

Las operaciones de arenas bituminosas incluyen **minería, extracción,
upgrading** e infraestructura de soporte. La **secuencia de minería** es una cadena de
perturbaciones:

1. **La capa suprayacente (overburden: arenas, till, arcilla) se retira y apila por
   separado**.
2. **Las arenas bituminosas se extraen** con camión y pala, draga o excavadora de rueda
   de cangilones.
3. **La extracción** usa agua caliente, cáustico y/o diluyente, seguida de
   **hidrotransporte** y **separación primaria y secundaria**.
4. **Los relaves** —arena, finos, agua y bitumen residual— se bombean como **pulpa**
   a las áreas de disposición.

El **cronograma de minería lo dicta la planta de extracción**, no el ingeniero de
presas: arena, finos, capa suprayacente y relaves gruesos se almacenan en diferentes
instalaciones a diferentes tasas, y la secuencia continúa durante décadas.

### 15.1.3 Dos climas, dos historias (el contexto geológico)

El comportamiento geotécnico que importa está dominado por la **glaciación**. El
depósito de Athabasca está **cubierto por depósitos glaciales**: el **till** de baja
plasticidad de la **Formación Murray** (glaciolacustre, más joven que la Formación
Clearwater) y las **arcillas de la Formación Clearwater** debajo, que se entiende están
**sobre-consolidadas glacialmente** y **pre-cizalladas** bajo sucesivos avances de hielo.
Las **fisuras estrechamente espaciadas** de las arcillas pueden controlar la estabilidad
aunque las arcillas sean por lo demás fuertes —una lección de la geología glacial que se
repite en cada talud de la región.

Dos hechos geológicos más impulsan el diseño:

- **Karst** — la **Formación Devónica Waterways** inferior incluye **caliza y
  anhidrita**; la **disolución** (karst) puede controlar la estabilidad geotécnica de las
  presas de relaves. (El área de **Fort McMurray** es el sitio de una característica de
  colapso activa, la **"subsidencia de 3 km"** documentada en el trabajo regional de
  peligro sísmico.)
- **Sismicidad** — la región de Athabasca está a hasta **~600 km del cinturón sísmico de
  las Montañas Rocosas canadienses**, por lo que los movimientos del terreno son
  **regionales**, no de campo cercano. El **Krinitzsky–Chang (1996)**, **Estudio de
  Peligro Sísmico de la Región de McMurray**, proporciona los parámetros sísmicos en los
  que se basa el diseño moderno, y la evaluación del **Geological Survey of Canada**
  coloca la **región de Fort McMurray entre las áreas de menor probabilidad de peligro
  sísmico de Canadá** (Código Nacional de Construcción de Canadá, Open File 4459).

---

## 15.2 Dos tradiciones de presas: retención de agua vs. arenas bituminosas

La idea organizadora del artículo fuente es que las **guías de la CDA fueron escritas
para presas de retención de agua**, y las presas de relaves de arenas bituminosas
difieren de formas que hacen inapropiada la aplicación directa. Importan cuatro
contrastes:

| Dimensión | Presa de retención de agua | Presa de relaves de arenas bituminosas |
|---|---|---|
| **Período de construcción** | Corto (semanas a ~3 años) | **Décadas** (20–50+ años de operación) |
| **Vida operativa** | Dada, decenas de años | Continúa tanto como viva la **operación** (vida de diseño 25–40 a, a menudo más) |
| **Base de diseño** | **Usa el nivel de agua del embalse** como caso de carga | **No tiene nivel de agua normal**; la superficie freática **se mueve** a medida que cambian la playa y la laguna |
| **Consecuencia de falla** | Inundación por agua almacenada | **Movimiento de relaves** (con o sin agua libre) —consecuencia ambiental y de rehabilitación |

Estas diferencias se cascada en cómo se tratan el **diseño de crecida**, el
**coronamiento** y las **condiciones de carga**. Una presa de relaves no tiene un "nivel
de agua normal" en el sentido de la presa de agua; el diseño debe en cambio seguir la
**vida operativa de la presa de arena**, manteniendo la superficie freática durante toda
esa vida.

---

## 15.3 Depósitos de relaves y tipos de presa

Los relaves se descargan como **pulpa** en un área de disposición. La **fracción
gruesa (arena) se asienta rápido**, construyendo una **playa de arena**; los **finos se
asientan lentamente** y se acumulan en la **laguna de relaves**. Según el **método de
deposición** (spigotting, sub-aéreo, sub-acuático), se reconocen cuatro tipos de depósito:

- **Relaves de arena** — la playa y los diques gruesos.
- **Relaves finos** (fluid fine tailings, FFT — ver [Capítulo 2](chapter-02-facilities-and-failures.md)).
- **Relaves compuestos** — arena y finos mezclados para **resistencia y rehabilitación
  rápida**.
- **Relaves blandos** — los depósitos finos, blandos y de baja densidad en el centro de la
  laguna.

Las **presas de relaves** mismas se construyen por las **técnicas convencionales de
terraplén** del Capítulo 2 —rociando (spigotting) la arena y construyendo diques por
**elevación secuencial**— pero con una restricción ajena a la mayoría de la práctica de
relaves: el **relleno a menudo se coloca como pulpa** y la **arena de playa a menudo se
usa tal como se coloca** en lugar de secarse y compactarse, por lo que el "relleno" se
parece mucho más a un material depositado y saturado que a un terraplén compactado.

> **Depositación cíclica.** Las estructuras de mayor consecuencia aguas abajo son
> típicamente los **diques externos de relaves** —presas aguas arriba más grandes y
> altas que contienen **relaves totales** (relaves finos y arena). Durante los **primeros
> años**, un dique aguas arriba de relaves **no puede soportar la carga completa**, por lo
> que se gestionan la relación finos-a-arena y la depositación.

---

## 15.4 Qué falla, y por qué: los modos de falla

El artículo clasifica los modos de falla de presas de relaves de arenas bituminosas en
**dos familias**:

1. **Falla interna de la presa** — superficie de falla **desde dentro de la presa** y
   **continuando a través** de la presa y su cimentación, **hacia los relaves**.
2. **Inestabilidad de talud aguas arriba** — superficie de falla **desde la coronación
   de la presa hacia la laguna**, con el depósito **actuando como masa resistente**;
   durante la construcción temprana, **una superficie freática alta cerca de la coronación
   de la presa** puede causar esto.

A esto se añaden los modos comunes a todas las presas de relaves (Capítulo 2):

- **Sobrevertimiento**, **erosión externa**, **licuefacción estática** de playa y capas
  de arena sueltas, **licuefacción sísmica** (aunque la región tiene baja sismicidad), y
  **erosión interna y tubificación**.
- **Inestabilidad por karst** donde la caliza/anhidrita devónica inferior se disuelve.

La implicación de diseño clave del artículo: **el depósito mismo debe incluirse en los
análisis de estabilidad**, porque la **laguna y la playa de relaves imponen una carga y
un campo de presión de poros** sobre la presa. Una presa de retención de agua se analiza
con agua a un lado; una presa de relaves debe analizarse con **un material heterogéneo,
cambiante y potencialmente licuable** a un lado.

---

## 15.5 Aplicar las guías de la CDA: qué transfiere, qué debe cambiar

El artículo mapea sistemáticamente los **casos de carga de las Guías CDA (2007)** contra
lo que realmente experimentan las presas de arenas bituminosas. El resultado es el corazón
práctico del estudio de caso.

| Caso CDA (2007) | Presa de agua | Presa de arenas bituminosas | Comentario |
|---|---|---|---|
| **Durante y fin de construcción** | Carga estática + estática de base operativa durante la elevación de la presa | **1.3 / 1.3** | La presa debe resistir cargas estáticas **durante la construcción y operación por efecto de la gravedad** aplicada a la presa |
| **Largo plazo** | Superficie piezométrica al máximo (operación a largo plazo) | **1.5 / 1.5** | El diseño a largo plazo asume **que la superficie freática revierte a un nivel natural (sin agua libre)** —no hay embalse permanente |
| **Vaciado rápido total o parcial** | 1.2–1.3 / 1.2–1.3 | **No aplicable** | Las presas de arenas bituminosas **no tienen mecanismo** para un vaciado controlado del embalse, por lo que este caso no aplica |
| **Sísmico (pseudo-estático / post-sísmico)** | 1.0 / 1.0 | 1.2–1.3 / 1.2–1.3 | Menor probabilidad pero **alta consecuencia**; el diseño asume relaves **susceptibles de licuefacción** |

**Consideraciones de filtración (el §4.3 del artículo).** Como el depósito y los diques
están saturados, el artículo trata la **filtración** como segunda en importancia solo
después de la estabilidad:

- Se analiza la **filtración en estado estacionario** a través de la presa, los diques y
  la cimentación con **redes de flujo o métodos numéricos**.
- Se proveen y mantienen **drenajes inferiores, drenajes y sistemas de recolección**.
- Una **superficie freática alta** puede desarrollar **filtración activa y reducir la
  estabilidad**; una **superficie freática baja** reduce ese riesgo.
- El **método de llenado de la laguna** (deposición sub-acuática) en sí **reduce la
  filtración**.

**Consideraciones sísmicas.** Aunque la región de Athabasca tiene **baja sismicidad**,
la **alta consecuencia de falla** significa que son justificados análisis pseudo-estáticos
y post-sísmicos. El artículo señala que un **análisis de estabilidad por equilibrio
límite es adecuado** para la mayoría del diseño de presas, y que el **factor mínimo
objetivo de seguridad** para cada caso se fija en consecuencia —pero que pueden necesitarse
**métodos más sofisticados** (y **ensayos in situ** para estimar la susceptibilidad) para
depósitos propensos a licuefacción.

> **Factores de seguridad aceptables.** La Tabla 1 del artículo (reproducida en concepto
> arriba) da los **factores mínimos objetivo de seguridad** para presas de agua y de relaves
> de arenas bituminosas lado a lado. Nótese la afirmación explícita de que **las presas de
> arenas bituminosas construidas con métodos de colocación de relleno no se analizan usando
> el mismo factor de seguridad que las presas de retención de agua**, y que los factores son
> **mínimos objetivo**, no garantías.

---

## 15.6 Desafíos operativos: el enfoque observacional

El §5 del artículo trata sobre la **práctica operativa**, y es donde un estudio de caso de
diseño se vuelve un estudio de caso de monitoreo.

### 15.6.1 El caso del enfoque observacional

Como la **vida operativa y las tasas de elevación de las presas de arenas bituminosas**
cambian a lo largo del largo período de construcción, el artículo argumenta que el
**enfoque observacional** (el método "aprender sobre la marcha" formalizado por Peck,
1969) es **más apropiado para las presas de arenas bituminosas que para las presas de
retención de agua**. El enfoque maximiza la eficiencia de diseño al **actualizar los
análisis a partir del desempeño medido**; a diferencia de la mayoría de las presas de
retención de agua, cuyas condiciones cambian poco tras la construcción, las condiciones de
arenas bituminosas **cambian continuamente**.

Los prerrequisitos del método son exigentes: el ingeniero debe identificar **por
adelantado qué sucederá y por qué**, predefinir el **plan de acción para cada desviación
creíble**, y **revisar continuamente** el monitoreo contra ese plan.

### 15.6.2 Monitoreo del desempeño

El artículo enfatiza que el monitoreo debe ser *"en buen detalle y frecuentemente
consistente con el diseño"* —y señala la trampa de que el **monitoreo observacional para
presas durante el llenado inicial no siempre se ha hecho bien**. El plan de monitoreo
debe:

- **Confirmar el diseño** — verificar cada supuesto de seguridad.
- **Suplementar** — detectar desviaciones temprano.
- **Ajustarse a la línea de tiempo** — ser apropiado al **ritmo planeado** de la presa
  (llenado inicial, operación temprana, largo plazo).
- **Relacionarse con el enfoque observacional** — vinculado a una **metodología de
  evaluación de riesgo** para que la gerencia pueda actuar.

### 15.6.3 Desarrollo de la licuefacción de relaves y los rellenos/consecuencias

El artículo conecta el **método de deposición con la licuefacción**. Donde los relaves se
depositan **sub-acuáticamente**, la laguna está **saturada y suelta**, y la
**licuefacción estática** es posible para el material **frágil y de baja densidad**. Cualquiera
que sea el método de deposición, el **monitoreo de la presión de poros** y de la **densidad
del depósito** es el núcleo del control de licuefacción (Capítulo 6).

### 15.6.4 Ensayos in situ para verificar el diseño

El §5.4 del artículo es una contribución práctica: los **ensayos in situ** (CPT, CPTu,
cono sísmico, etc.) para **verificar el estado del depósito** (densidad, resistencia,
susceptibilidad de licuefacción) **son esenciales** y se hacen **durante las operaciones**,
no solo en el diseño. Como dice el artículo: *"El propósito de los ensayos in situ es
verificar el diseño y los supuestos... y construir confianza en que la base de diseño y los
supuestos pueden alcanzarse."* Este es el enfoque observacional aplicado al **depósito** tanto
como a la **presa**.

---

## 15.7 La experiencia de los diques en fosa: monitoreo en la práctica (Albian)

El artículo complementario —*"Aplicación de Instrumentación Geotécnica en el Monitoreo del
Desempeño de Diques en Fosa (In-Pit Dykes)"* (Soe Moe & Biggar, 2013)— reporta cómo se
ejecuta este manual en los **diques en fosa (in-pit dykes) Albian** de CNRL en la región de
Athabasca. Este es lo más cercano a un **estudio de caso a nivel de sitio** disponible en el
registro público, y muestra la teoría en operación:

- **Instrumentación acoplada a modos de falla.** Piezómetros (típicamente de cuerda
  vibratoria) para seguir **presión de poros y superficie freática**; **inclinómetros y
  medidores de asentamiento** para seguir **deformación**; **monolitos de referencia** para
  el movimiento superficial —todo vinculado a los modos de falla identificados e informado
  contra umbrales.
- **Los diques en fosa** se construyen **dentro de la fosa minada** y se elevan con la
  operación, por lo que su comportamiento está íntimamente acoplado a la **secuencia de
  deposición** y a la **geología del piso de la fosa**.
- **El monitoreo como control de construcción.** Como el relleno se deposita y el depósito
  cambia, el monitoreo no es mera verificación —es **parte del método de construcción**,
  indicando al operador cuándo avanzar, pausar o modificar la deposición.
- **El enfoque observacional requiere que el monitoreo sea lo suficientemente rápido** para
  detectar una desviación **a tiempo para actuar** —un punto que el artículo de la CDA hace
  explícito.

---

## 15.8 El arco de rehabilitación (lo que hace distinto a las arenas bituminosas)

Subyace a todo esto un propósito que una presa de agua no comparte: la **rehabilitación
(reclamation)**. Como muestra la Figura 2 del artículo, una presa de relaves está destinada
en última instancia a convertirse en un **"paisaje rehabilitado"** —la **superficie de la
laguna de relaves** es parte del diseño de cierre, y la **presa misma se vuelve una forma
de terreno (landform)**. Por eso:

- El **comportamiento a largo plazo del depósito** (consolidación, ganancia de resistencia,
  densidad) importa tanto como el de la presa.
- Se usan **relaves compuestos** y **acondicionamiento de playa** para construir resistencia
  para **rehabilitación rápida**.
- El encuadre de **"no es presa de retención de agua"** no es solo un detalle legal —la
  estructura no está destinada a retener un embalse permanente al cierre.

---

## 15.9 Lecciones para cualquier ingeniero de relaves

Incluso fuera del norte de Alberta, el estudio de caso enseña lecciones transferibles:

1. **Sepa qué guía está heredando.** El caso CDA muestra que una norma de seguridad de
   presas respetable puede necesitar *interpretación* antes de encajar en una instalación de
   relaves —y que **no todos los casos de carga aplican**.
2. **Deje que la realidad operativa moldee el diseño.** La construcción de décadas, la
   depositación controlada por tasa y una superficie freática móvil son insumos de diseño,
   no detalles.
3. **Incluya el depósito en su análisis.** La "carga" de una presa de relaves es un material
   cambiante, a menudo licuable —analícelo, y **verifique su estado por ensayos in situ**.
4. **La filtración es segunda solo tras la estabilidad.** Drenajes inferiores, drenajes y
   gestión de laguna son estructurales, no cosméticos.
5. **Adopte el enfoque observacional deliberadamente** —con acciones predefinidas,
   monitoreo lo suficientemente rápido y revisión continua.
6. **La instrumentación es control de construcción**, no solo cumplimiento.
7. **Diseñe para el cierre desde el día uno** —la presa se vuelve la forma de terreno.

---

## 15.10 Puntos clave

- Las presas de relaves de arenas bituminosas del norte de Alberta son **grandes,
  operadas durante décadas, estructuras dirigidas por la operación** —no presas de
  retención de agua.
- **Las guías de la CDA aplican, pero requieren interpretación**: los casos de crecida,
  coronamiento y **vaciado** no transfieren; la calificación la fija los **casos de carga
  reales de la presa**.
- **La licuefacción de relaves, la filtración y el karst** son las preocupaciones
  geotécnicas de control; **la sismicidad es baja pero la consecuencia es alta**.
- El **enfoque observacional** es más apropiado aquí que para las presas de agua porque
  las condiciones cambian continuamente.
- **Los ensayos in situ y el monitoreo del desempeño** verifican el diseño y sustentan el
  enfoque observacional.
- Los **diques en fosa Albian** demuestran el monitoreo usado como **control de
  construcción**.
- La **rehabilitación** es el propósito que el diseño debe servir.

---

## Fuentes

- **Eshraghian, A. & Becker, D.E. (Golder Associates)** — *Aplicación de las Guías de
  Seguridad de Presas de la CDA al Diseño Geotécnico de Presas de Relaves de Arenas
  Bituminosas en el Norte de Alberta*, **Boletín de la Canadian Dam Association, Invierno
  2016**, pp. 26–41.
- **Soe Moe, K.W. & Biggar, K.W. (2013)** — *Aplicación de Instrumentación Geotécnica en
  el Monitoreo del Desempeño de Diques en Fosa (In-Pit Dykes)*, artículo de conferencia
  (CNRL Albian).
- **Canadian Dam Association (2007)** — *Guías de Seguridad de Presas* y *Boletín Técnico:
  Diseño Geotécnico de Presas*.
- **Alberta Energy Regulator** — *Guía Técnica de Seguridad de Presas* y *Guía para la
  Gestión de Instalaciones de Relaves* (con MAC).
- **Krinitzsky & Chang (1996)** — *Estudio de Peligro Sísmico de la Región de McMurray*.
- **Geological Survey of Canada** — *Peligro sísmico del Código Nacional de Construcción
  de Canadá*, Open File 4459.

> **Vigencia regulatoria.** La Guía Técnica de Seguridad de Presas del AER y las guías de
> la CDA se revisan periódicamente. Verifique la **edición actual** antes de cualquier
> diseño o presentación.
