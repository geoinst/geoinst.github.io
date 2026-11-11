---
lang: es
lang_alt: reference-manuals/fhwa-mse-walls/chapter-09-field-inspection-monitoring/
---
# Capítulo 9 — Inspección de campo y monitoreo de desempeño

## 9.1 Revisiones previas a la construcción

Antes de la construcción, revise los **planos, especificaciones y presentaciones** contra
la intención de diseño: el tipo y disposición del refuerzo, la especificación del relleno,
los detalles de cara y el sistema de drenaje. Confirme que cualquier diseño de proveedor
haya sido aprobado y que el relleno especificado esté realmente disponible en el préstamo
del proyecto —una fuente muy común de problemas es un relleno especificado que ninguna
fuente local puede cumplir.

## 9.2 Inspección de materiales prefabricados

Inspeccione el **refuerzo** (tipo, resistencia, dimensiones, recubrimiento y libertad de
daño), las **unidades de cara** (paneles o bloques, dimensiones y puntos de conexión del
refuerzo), los **conectores** y los **materiales de drenaje y filtro** contra la
especificación. Los materiales dañados o fuera de especificación se rechazan antes de que
se construyan en la estructura, donde ya no pueden verse.

## 9.3 Control de construcción

El manual plantea los puntos de control para cada etapa de construcción:

- **Preparación de cimentación** — excave al nivel de diseño, proof-roll, y verifique el
  suelo de cimentación y la almohadilla de nivelación.
- **Erección de cara** — controle la **verticalidad**, el **alineamiento horizontal** y
  los **anchos de junta** de la cara; estas son las tolerancias más visibles en la
  estructura terminada y las más omitidas.
- **Colocación del refuerzo** — verifique la **longitud**, **orientación**, **elevación**
  y **espaciamiento** de cada capa, que no esté dañado, que se coloque sobre relleno
  compactado (no sobre relleno suelto o un talud), y que la conexión a la cara se haga
  correctamente.
- **Colocación y compactación del relleno de respaldo** — coloque el relleno en capas y
  compacte a la densidad especificada. Dentro de unos **1 m de la cara**, use solo
  **equipo de compactación ligero** para no perturbar la cara y la conexión del refuerzo
  (Figura 84); se permite equipo mayor más lejos de la cara.
- **Tolerancias** — el manual da condiciones fuera de tolerancia y sus causas probables
  (Tabla 16), para que el inspector diagnostique un problema en lugar de solo registrarlo.
  La Tabla 15 es la **lista de verificación de inspección de campo**.

## 9.4 Programas de monitoreo de desempeño

**Propósito de un programa de monitoreo.** El monitoreo confirma que la estructura se
comporta como el diseño predijo —que la deformación de cara, la tensión del refuerzo y el
asentamiento se mantienen dentro de los valores asumidos— y da alerta temprana si no lo
hacen. Aplica el **Método Observacional**: se hacen predicciones, se comparan las
mediciones con ellas, y siguen acciones pre-planificadas.

**Programa de monitoreo limitado.** Para estructuras rutinarias: **inspección visual** de
la cara por agrietamiento, abombamiento o apertura de junta, más **topografía del
movimiento de cara** y asentamiento de la corona del muro. Barato, y suficiente para un
muro bien comprendido sobre una cimentación competente.

**Programa de monitoreo integral.** Para muros altos, estribos, muros sobre cimentaciones
blandas o estructuras críticas, el programa añade instrumentación:

- **Inclinómetros** — movimiento lateral de la cara y del terreno detrás de ella.
- **Plataformas de asentamiento y puntos de topografía** — movimiento vertical de la
  cimentación y la masa reforzada.
- **Galgas de deformación o celdas de carga en el refuerzo** — la tensión realmente
  movilizada en capas seleccionadas, para comparar con $T_{max}$.
- **Celdas de presión** — esfuerzo de contacto en la base y detrás de la cara.
- **Piezómetros** — presiones de poro en el relleno reforzado y la cimentación, que
  revelan si el drenaje está funcionando.

La Tabla 17 lista los instrumentos posibles y lo que mide cada uno.

**Implementación del programa.** Defina las **ubicaciones de los instrumentos**, las
**frecuencias de lectura** (frecuentes durante la construcción, reduciendo después), los
**valores disparador (trigger)**, y las **acciones** a tomar si se excede un disparador —
todo antes de que comience la construcción.

**Interpretación de datos.** Grafique cada medición contra el tiempo y contra la etapa de
construcción, y compárela con la predicción de diseño. Una sola lectura significa poco; la
**tendencia** y la **tasa** son lo que importa —el mismo principio que gobierna el
monitoreo de presas y excavaciones en otras partes de esta base de conocimientos.

## 9.5 Puntos clave

- **Inspeccione los materiales antes de que se entierren** — el refuerzo y el drenaje no
  pueden inspeccionarse después.
- Las tolerancias que más importan son la **verticalidad de cara, el alineamiento y el
  ancho de junta**, y la **longitud y elevación del refuerzo**.
- **Compacte ligeramente dentro de 1 m de la cara**; equipo más pesado más lejos.
- Elija el programa de monitoreo por **riesgo**: limitado (visual + topografía) para
  muros rutinarios, integral (instrumentado) para estructuras altas, de suelo blando o
  críticas.
- Instrumente el **propio refuerzo** si quiere conocer la tensión movilizada real —y fije
  **valores disparador y acciones por anticipado**.

## 9.6 Dónde encaja esto

Este capítulo es el puente del manual al núcleo de instrumentación del sitio. Para las
familias de instrumentos y sus principios de funcionamiento, vea el
[Manual de Referencia de Instrumentación Geotécnica FHWA](../fhwa/index.md) y
[Dunnicliff](../dunnicliff/index.md); para cómo las lecturas se convierten en
decisiones, vea [Monitoreo del Desempeño de Presas](../monitoring-dam-performance/index.md)
y el marco de monitoreo automatizado [ADAQS](../../../vi/adaqs/index.md).
