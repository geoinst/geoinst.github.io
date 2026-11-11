---
lang: es
lang_alt: reference-manuals/fhwa-mse-walls/chapter-05-complex-geometries/
---
# Capítulo 5 — Muros MSE con geometrías complejas

## 5.1 Estribos de puente

Un **estribo MSE** lleva las cargas de apoyo del puente además del empuje de tierra, y
esas cargas entran a la masa reforzada en la parte superior —donde el refuerzo es menos
capaz de redistribuirlas. Esta es la aplicación MSE más exigente, y el manual la trata en
detalle.

**Estribos MSEW sobre zapatas corridas.** La zapata descansa sobre el relleno reforzado
(o sobre la cimentación detrás de él), y sus cargas (vertical, horizontal y momento) se
llevan a la masa reforzada y la cimentación. El diseño debe verificar:

- **Capacidad de carga** bajo la zapata, incluyendo la excentricidad de las cargas del
  puente.
- **Estabilidad interna** con la carga de zapata añadida como gran sobrecarga —la
  tensión en las capas superiores de refuerzo sube abruptamente.
- **Deslizamiento** de la masa reforzada bajo la carga horizontal del puente.
- **Estabilidad global** a través del estribo y su cimentación.
- **Asentamiento** de la zapata y del aproche, y la **tolerancia** para el movimiento
  diferencial entre el asiento del puente y la losa de aproximación.

**Estribos MSEW sobre cimentaciones de pilotes.** Donde la cimentación es demasiado
débil para una zapata corrida, el estribo se apoya en **pilotes**, y el muro MSE se
construye a su alrededor. Esto desacopla el asentamiento del puente del del muro pero
crea sus propios problemas: los pilotes interrumpen el refuerzo, la cabezal de pilotes
genera cargas concentradas, y el diseño debe asegurar que el refuerzo no se dañe por el
hincado de pilotes ni por el movimiento de la cabezal.

## 5.2 Muros superpuestos (escalonados)

Donde dos o más muros MSE se apilan con un berma entre ellos, el muro inferior lleva la
sobrecarga del superior. El manual da **reglas de diseño** para muros superpuestos: el
desplazamiento entre muros, las longitudes de refuerzo en cada uno, y la forma en que la
carga del muro superior se esparce sobre el inferior. Ignorar la interacción —
diseñar cada muro como si estuviera solo— es un error clásico.

## 5.3 Muros con longitudes de refuerzo desiguales

Donde la longitud del refuerzo debe variar a lo largo del muro (por obstrucciones,
geometría o cargas variables), el diseño debe seguir proveyendo una masa reforzada
**continua** y verificar las zonas de transición donde cambia la longitud, porque las
secciones más cortas atraen menos resistencia de arranque y pueden actuar como puntos
débiles.

## 5.4 Muros frente a frente (back-to-back)

Donde dos muros se enfrentan con una masa de suelo estrecha entre ellos, las zonas
reforzadas pueden **solaparse**. El manual distingue los casos por la relación entre la
separación y la altura del muro:

- **Separación amplia** — cada muro se diseña independientemente.
- **Separación estrecha** — las zonas reforzadas se solapan y los muros actúan como un
  compuesto único; el diseño debe tratar la masa como una.
- **Separación muy estrecha** — las dos caras forman efectivamente un muro único con
  refuerzo cruzando todo el ancho.

## 5.5 Detalles

Los detalles específicos de estribo incluyen el **asiento del puente**, la conexión de
la **losa de aproximación**, la disposición de la **almohadilla de apoyo**, y el
**drenaje** detrás y a través del estribo —todos los cuales deben tolerar la deformación
hacia afuera del muro sin distrés.

## 5.6 Ejemplo de diseño, estribo de puente

El manual desarrolla un diseño de estribo completo —geometría, cargas del puente,
estabilidad externa, estabilidad interna con la sobrecarga de zapata, y la disposición
de refuerzo resultante— por manual y por programa de computadora.

## 5.7 Puntos clave

- Un **estribo es un muro más una carga concentrada superior** —la ruta de carga al
  refuerzo y a la cimentación debe ser explícita.
- Los **estribos sobre pilotes** desacoplan el asentamiento pero interrumpen el refuerzo;
  detalle bien la interfaz.
- Los **muros superpuestos y frente a frente interactúan** —diseñe el sistema, no los
  muros individuales.
- Las **longitudes de refuerzo desiguales** crean zonas de transición que deben
  verificarse.
- Tolere la **deformación y el asentamiento diferencial** en el asiento del puente, o la
  aproximación se agrietará.
