---
lang: es
lang_alt: glossary/
lang_alt_vi: vi/thuat-ngu/
---

# 📖 Glosario de Instrumentación Geotécnica y ADAQS

> Glosario técnico y diccionario de referencia que abarca la instrumentación geotécnica de subsuelo, la física de sensores, los sistemas automatizados de adquisición de datos (ADAS/ADAQS), la telemetría inalámbrica y el monitoreo de campo. Basado en normas internacionales (ISO 18674, ASTM, BS 5930) y en los principios fundamentales de John Dunnicliff.

---

## 1. Sensores de subsuelo y dispositivos de medición

### Piezómetros y presión de poros

* **Piezómetro (Piezómetro)**: Instrumento instalado en suelo, roca o relleno para medir la presión de poros o la elevación del nivel freático.
* **Piezómetro de Cuerda Vibrante (PCV)**: Sensor de diafragma en el que la presión del agua deflexiona una membrana flexible conectada a un alambre de acero tensado. Los cambios en la deflexión alteran la tensión del alambre y su frecuencia de resonancia natural ($f$). Muy resistente al ruido eléctrico y a los largos tendidos de cable.
* **Piezómetro de Tubo Abierto (Casagrande)**: Piezómetro de tubo abierto formado por una punta porosa de cerámica o plástico conectada a una tubería vertical. Mide el nivel de agua hidrostático directamente con un indicador eléctrico de nivel (dip meter). Respuesta hidráulica más lenta en arcillas de baja permeabilidad.
* **Piezómetro Neumático**: Sensor de diafragma accionado por presión de gas. Se bombea gas (normalmente nitrógeno) por un tubo de alimentación hasta equilibrar la presión de poros y abrir una válvula que ventea por un tubo de retorno. Sin cambio de volumen de fluido, con retardo despreciable.
* **Piezómetro de Hinca / Empuje**: Piezómetro robusto de punta afilada, hincado directamente en formaciones de arcilla o limo blando sin perforar un sondeo previo.
* **Filtro de Alta / Baja Presión de Entrada de Aire (HAE / LAE)**:
    * **Cerámica HAE**: Tamaño de poro fino (típicamente 1–2 µm) con alta presión de burbujeo, que evita la entrada de aire bajo presiones de poros negativas (succión) en suelos no saturados.
    * **Carborundo / Polietileno LAE**: Tamaño de poro grueso (típicamente 50 µm), diseñado para una saturación rápida en mediciones estándar de agua subterránea saturada.
* **Matriz de Piezómetros Multinivel**: Varios sensores PCV posicionados a elevaciones discretas dentro de un solo sondeo para captar gradientes hidráulicos verticales, acuíferos colgados y perfiles de filtración.

### Inclinómetros y desplazamiento lateral

* **Tubo de Inclinómetro (Casing)**: Tubo ranurado de plástico (ABS) o aluminio instalado en un sondeo, muro de lechada o terraplén, con guías ortogonales internas que orientan la sonda.
* **Inclinómetro de Sonda de Recorrido**: "Torpedo" rodante con acelerómetros servo o sensores MEMS ortogonales, descendido por el tubing ranurado sobre un cable de control graduado para registrar perfiles de inclinación a intervalos regulares (p. ej. 0,5 m).
* **Inclinómetro In Situ (IPI)**: Cadena de pods articulados de sensores de inclinación suspendidos permanentemente dentro del tubing ranurado a profundidades críticas para un registro continuo y automatizado del desplazamiento lateral.
* **Matriz Flexible 3D (SAA / ShapeArray)**: Cadena articulada de segmentos rígidos miniatura interconectados por juntas flexibles, con acelerómetros MEMS triaxiales que miden perfiles de desplazamiento 3D continuos en tiempo real.
* **Inclinómetro Horizontal**: Sistema de inclinómetro que utiliza tubing ranurado instalado horizontalmente para medir perfiles de asentamiento y heave bajo terraplenes, tanques o rellenos sanitarios.
* **Inspección de Torsión Espiral**: Sonda auxiliar que mide la torsión en las guías del tubing de inclinómetro en sondeos profundos, corrigiendo errores de azimut en los cálculos de deflexión lateral.

### Extensómetros y sistemas de asentamiento

* **Extensómetro Multipunto de Sondeo (MPBX)**: Conjunto de anclas fijadas a distintas profundidades dentro de un sondeo, unidas por varillas rígidas o tendones de fibra de vidrio dentro de fundas de protección hasta una cabeza de referencia en superficie. Mide el movimiento axial del suelo y la deformación zonal.
* **Medidor Magnético de Asentamiento**: Tubo de acceso rodeado por imanes arácnidos externos anclados al suelo. Una sonda portátil de interruptor reed baja por el tubo y emite un zumbido al pasar por cada objetivo magnético, dando asentamiento vertical puntual.
* **Celda de Nivel Líquido de Asentamiento**: Sensor de presión diferencial o celda de rebose unida por tubería llena de líquido a un reservorio externo, que mide cambios de elevación vertical de estructuras subterráneas o losas de cimentación.
* **Placa de Asentamiento**: Placa rígida de acero o madera colocada sobre el terreno original antes de colocar el relleno, conectada a una tubería vertical que se prolonga a medida que crece el terraplén.
* **Extensómetro de Cinta**: Cinta de acero de precisión portátil con un cabezal micrómetro de tensado en línea, usada para medir convergencia en muros de túnel y puntales de excavación.

### Monitoreo estructural y de carga

* **Célula de Carga (Anular / de Orificio Pasante)**: Instrumento colocado bajo tuercas de anclaje en tirantes, pernos de roca o puntales de cimentación para medir carga axial de tracción o compresión. Utiliza normalmente varias galgas de cuerda vibrante en paralelo.
* **Galga de Deformación de Cuerda Vibrante (VWSG)**: Sensor soldado a estructuras de acero o empotrado en concreto (barra gemela / galga de empotramiento) para registrar microdeformación ($\mu\varepsilon$) por carga estructural o expansión térmica.
* **Célula de Presión de Tierras (Celda de Presión Total)**: Dos placas circulares o rectangulares de acero soldadas con un fluido hidráulico incompresible entre ellas, conectadas a un transductor de presión. Instalada en la interfaz suelo-estructura o dentro del relleno del terraplén.
* **Tiltímetro (Tiltmeter)**: Instrumento anclado a muros de contención, estructuras históricas o pilas de puentes para detectar rotación angular. Utiliza burbujas electrolíticas o sensores MEMS de alta precisión.
* **Crackmetro / Jointmetro**: Transductor de desplazamiento anclado a través de juntas de concreto o fisuras de roca para monitorear apertura, cierre y corte relativos.

---

## 2. Sistemas Automatizados de Adquisición de Datos (ADAS) y Telemetría

### Acondicionamiento de señal y protocolos

* **ADAS / ADAQS**: Sistema Automatizado de Adquisición de Datos — conjunto autónomo de sensores, registradores, módulos de energía e infraestructura de comunicaciones para monitoreo geotécnico sin supervisión.
* **Excitación por Frecuencia de Punteo**: Método estándar para sensores de cuerda vibrante, en el que una bobina electromagnética aplica un impulso de barrido de frecuencia rápido para hacer vibrar el alambre en resonancia mecánica y luego leer la señal sinusoidal inducida.
* **Análisis Espectral / VSPECT**: Tecnología avanzada de acondicionamiento de señal que realiza Transformadas Rápidas de Fourier (FFT) sobre la señal cruda de retorno de la cuerda vibrante, aislando la frecuencia de resonancia fundamental del ruido eléctrico externo.
* **Bucle de Corriente 4–20 mA**: Estándar de transmisión analógica en el que las señales del sensor se modulan como corriente eléctrica. Muy inmune a la resistencia de cable a larga distancia.
* **RS-485 / Modbus RTU**: Estándar de bus serie diferencial balanceado capaz de redes multidrop con 32+ sensores digitales a distancias de hasta 1.200 metros.
* **SDI-12**: Interfaz digital serie de bajo consumo ampliamente usada en sensores ambientales y geotécnicos a 1200 baudios.
* **Bus CAN / CANopen**: Protocolo de bus digital robusto de grado automotriz adoptado en instrumentación de túneles de alta velocidad y subterráneos.

### Redes inalámbricas y hardware de campo

* **Registrador de Datos (Datalogger)**: Instrumento electrónico que alimenta los sensores conectados, digitaliza señales analógicas, procesa polinomios de calibración y almacena registros con marca de tiempo en memoria flash no volátil.
* **Multiplexor de Relés**: Módulo de expansión que utiliza relés de estado sólido o de lengüeta sellados para conmutar secuencialmente múltiples canales de sensor a un solo puerto de medición del registrador.
* **LoRaWAN (Long Range Wide Area Network)**: Protocolo inalámbrico de baja potencia y largo alcance en bandas sub-GHz sin licencia (868 MHz EU, 915 MHz US/Américas, 923 MHz AS). Excelente penetración en entornos urbanos densos y fosos profundos.
* **Red Mallada Inalámbrica**: Topología de red autoformante y autocicatrizante en la que los nodos sensores actúan como repetidores para enrutar paquetes de datos a una pasarela central, dando resiliencia operativa frente a obstrucciones de línea de visión.
* **IoT Celular (NB-IoT y LTE-M)**: Estándares de comunicación celular de baja potencia diseñados para sensores IoT alimentados por batería, transmitiendo pequeños paquetes de datos directamente a servidores en la nube vía torres comerciales.
* **Telemetría Satelital (Iridium SBD)**: Transmisión de datos por satélite en órbita terrestre baja usada en presas remotas críticas y sitios mineros sin cobertura celular terrestre.
* **Módulo Solar y MPPT**: Arreglo fotovoltaico combinado con un controlador de carga de Maximum Power Point Tracking (MPPT) y batería sellada AGM o LiFePO4 para operación de campo autónoma.

---

## 3. Física de sensores y reducciones matemáticas

### Reducciones de cuerda vibrante

* **Ecuación de Frecuencia Natural**: La frecuencia de resonancia fundamental $f$ de un alambre empotrado bajo tensión $\sigma$:

    $$
    f = \frac{1}{2L} \sqrt{\frac{\sigma}{\rho}} = \frac{1}{2L} \sqrt{\frac{E \cdot \varepsilon}{\rho}}
    $$

    Donde $L$ es la longitud del alambre, $\rho$ la densidad, $E$ el módulo de Young y $\varepsilon$ la deformación del alambre.

* **Dígitos (Unidades de Periodo Lineal)**: Parámetro linealizante directamente proporcional a la deformación del alambre:

    $$
    \text{Dígitos} = \frac{f^2}{1000}
    $$

* **Ecuación de Calibración Lineal**:

    $$
    P = G \cdot (R_0 - R)
    $$

    Donde $G$ es el factor de galga (coeficiente lineal calibrado), $R_0$ la lectura base en dígitos y $R$ la lectura actual.

* **Ecuación de Calibración Polinómica (Segundo Orden)**:

    $$
    P = A \cdot R^2 + B \cdot R + C
    $$

    Proporciona mayor precisión de medición en amplios rangos de presión.

* **Compensación Térmica** ($K_T$):

    $$
    P_{corr} = P_{raw} + K_T \cdot (T - T_0)
    $$

    Corrige la expansión térmica diferencial entre la cuerda vibrante y el cuerpo del sensor de acero inoxidable.

* **Compensación Barométrica**:

    $$
    P_{net} = P_{measured} - (B - B_0)
    $$

    Esencial para piezómetros sellados, aísla los cambios reales del agua subterránea de las oscilaciones barométricas atmosféricas ambientales.

### Reducción de datos de inclinómetro

* **Incremento de Deflexión** ($\delta_i$):

    $$
    \delta_i = L \cdot \sin(\theta_i) = C \cdot (A_0 - A_{180})
    $$

    Donde $L$ es la distancia entre ruedas de la sonda (típicamente 500 mm), $\theta_i$ el ángulo de inclinación, y $A_0, A_{180}$ las corridas conjugadas.

* **Suma de Verificación (Cero de Desfase)**:

    $$
    \text{Suma de Verificación} = A_0 + A_{180}
    $$

    Valor constante en todas las profundidades que confirma la estabilidad del instrumento y la ausencia de contaminación mecánica en las ruedas.

* **Desplazamiento Acumulado** ($D_k$):

    $$
    D_k = \sum_{i=1}^k \delta_i
    $$

    Suma de los desplazamientos incrementales calculados desde el ancla estable inferior hacia el collar superficial.

---

## 4. Riesgo de ingeniería y marcos TARP

* **TARP (Plan de Acción y Respuesta ante Umbrales)**: Marco sistemático de gestión de emergencias y riesgos que establece acciones operativas definidas según los umbrales de instrumentación observados:
    * **Nivel 0 (Verde / Base)**: Comportamiento normal dentro de los límites de diseño previstos. Frecuencia de monitoreo estándar.
    * **Nivel 1 (Ámbar / Alerta)**: La medición supera la base estadística o el margen de seguridad inicial. Frecuencia de monitoreo duplicada; se despacha inspección de ingeniería de campo.
    * **Nivel 2 (Naranja / Revisión)**: Aceleración significativa de tendencia o tensión estructural cercana a la tolerancia de diseño. Revisión de ingeniería senior, verificación de instrumentos de respaldo, equipo en espera.
    * **Nivel 3 (Rojo / Acción Requerida)**: Umbral crítico superado; falla estructural inminente o filtración incontrolable. Parada inmediata de trabajos, evacuación del sitio y ejecución de protocolos de remediación de emergencia.
* **Velocidad de Desplazamiento ($v = \frac{d\delta}{dt}$)**: Tasa de movimiento del suelo en el tiempo. Una aceleración en la velocidad de desplazamiento es el precursor primario de fallas catastróficas de taludes y excavaciones.
* **Línea Freatica (Línea de Filtración)**: El límite superior del flujo de filtración a través del terraplén de una presa de tierra, donde la presión de poros iguala a la presión atmosférica.
* **Tubificación (Erosión Interna)**: Remoción progresiva de partículas de suelo por el flujo de filtración a través de presas de tierra o cimientos, llevando a conductos internos y el rompimiento de la presa.

---

## 5. Buenas prácticas de instalación en campo y lechada

* **Método de Encamisado Total (Mikkelsen / Contreras)**: Técnica de instalación en la que los piezómetros se colocan directamente en el sondeo y se encapsulan completamente en una lechada cemento-bentonita sin paquete filtrante de arena tradicional ni pellets de bentonita. Habilitado por el volumen de desplazamiento extremadamente bajo de los sensores de diafragma modernos.
* **Proporciones de Mezcla de Lechada**: Relación específica de agua a cemento Portland y bentonita sódica en polvo diseñada para igualar la permeabilidad y el módulo de la formación circundante:
    * *Suelo blando*: Agua:Cemento:Bentonita $\approx$ 2,5 : 1,0 : 0,3 a 0,4 en peso.
    * *Roca media a rígida*: Agua:Cemento:Bentonita $\approx$ 1,5 : 1,0 : 0,1 en peso.
* **Sello de Pellets de Bentonita**: Pastillas de bentonita sódica altamente comprimidas hincadas sobre los paquetes de arena en instalaciones Casagrande tradicionales, que se hinchan al hidratarse formando un sello hidráulico impermeable.
* **Acoplamiento Telescópico**: Juntas de deslizamiento colocadas a lo largo de las cadenas de tubing de inclinómetro o asentamiento para evitar la compresión axial y el pandeo cuando ocurren grandes asentamientos verticales.

---

## 6. Instalaciones de Almacenamiento de Relaves y Seguridad de Presas de Relaves

* **Relaves**: Los sólidos de desecho finamente molidos que quedan tras extraer metales o minerales del mineral, transportados y depositados como pulpa.
* **Instalación de Almacenamiento de Relaves (TSF)**: El sistema completo de embalse — terraplén(es), relaves depositados, estanque sobrenadante, desaguadero y obras de recuperación — que almacena los relaves mineros.
* **Presa de Relaves**: El terraplén ingenieril que retiene el depósito de relaves; a menudo elevado incrementalmente durante la vida de la mina y frecuentemente construido con los propios relaves.
* **Alzado de Corona (Elevación de la Presa)**: Adición incremental a la altura de un terraplén de relaves, colocada por el método aguas abajo, línea central o aguas arriba.
* **Método de Construcción Aguas Abajo**: Cada alzado se coloca aguas abajo del anterior, de modo que la mayor parte de la estructura descansa sobre la cimentación — generalmente el método más robusto.
* **Método de Construcción Línea Central**: Los alzados se colocan sobre la línea central original; riesgo intermedio.
* **Método de Construcción Aguas Arriba**: Cada alzado se coloca en el lado aguas arriba (deposicionado), de modo que el terraplén descansa sobre relaves sueltos y saturados — el método de mayor riesgo, propenso a licuación.
* **Playa (de relaves)**: La superficie ligeramente inclinada de los relaves depositados entre el punto de descarga y el estanque sobrenadante.
* **Geometría de la Playa**: La pendiente y longitud de la playa, que controlan dónde se sitúa la superficie freática y cuánto libre borda se retiene.
* **Estanque Sobrenadante**: El cuerpo de agua clarificada sobre los relaves asentados, del que se recupera o desagua el agua.
* **Desaguadero (Torre de Decantación / Sistema de Decantación)**: La estructura y tubería usadas para retirar el agua sobrenadante y controlar el nivel del estanque y el libre borda.
* **Libre Borda (Freeboard)**: La distancia vertical entre la superficie del estanque y el punto más bajo de la corona del terraplén; una salvaguarda primaria contra el rebalse.
* **Riego por Aspersión / Deposición**: Descarga de la pulpa de relaves desde la corona del terraplén para construir la playa por deposición hidráulica.
* **Relaves Espesados / Pasta / Filtrados**: Relaves deshidratados (contenido de sólidos progresivamente mayor) que reducen el agua libre y el riesgo de licuación.
* **Almacenamiento en Foso / Recinto**: Almacenamiento de relaves en un pozo minado o en un recinto de dique anular en lugar de un embalse en valle.
* **Licuación (Liquefaction)**: Pérdida de resistencia al corte cuando un suelo saturado y suelto (contractivo) es cargado o sacudido y la presión de poros se eleva hacia una tensión efectiva cercana a cero.
* **Licuación Estática**: Licuación provocada por una carga estática (un alzado, subida rápida del estanque o debilidad de cimentación) en lugar de un sismo — el mecanismo catastrófico dominante en fallas de relaves.
* **Licuación Sísmica**: Licuación provocada por sacudidas sísmicas cíclicas.
* **Relación de Presión de Poros ($r_u$)**: La relación entre la presión de poros medida y la tensión vertical efectiva inicial ($r_u = u / \sigma'_v$); valores crecientes señalan licuación inminente.
* **Presión de Poros Excedente**: Presión de poros por encima del valor en estado estacionario (hidrostático), generada por carga, construcción o sacudidas.
* **Falla por Flujo / Corrida (Run-out)**: Masa licuada que fluye rápidamente y recorre largas distancias, causando daño extremo aguas abajo.
* **Drenaje de Pie**: Zona o dren permeable en el pie aguas abajo que recolecta y controla la filtración, manteniendo baja la superficie freática.
* **Filtración Turbia**: Filtración que transporta partículas finas de suelo (descarga turbia) — señal de alerta de erosión interna (tubificación).
* **Categoría de Consecuencia**: Clasificación de una instalación por el impacto potencial aguas abajo de una falla (a menudo A/B/C), que fija la intensidad del monitoreo y la revisión.
* **Cierre (de mina)**: La fase postoperacional en la que la instalación se da de baja y se asegura, requiriendo vigilancia continua hasta demostrar el estado estacionario a largo plazo.
* **InSAR / A-DInSAR (Interferometría Radar Satelital)**: Técnica de teledetección que usa pasadas satelitales repetidas para medir desplazamiento del suelo a escala milimétrica en toda la instalación sin instrumentos en sitio.

---

## 7. Monitoreo de Desempeño de Presas (alcance ASCE MOP-135)

* **Desempeño de Presa**: El comportamiento observado de una presa, su cimentación y estructuras anexas comparado con el comportamiento esperado.
* **Comportamiento Esperado vs. Medido**: La comparación central del monitoreo; una diferencia grande, inexplicada o tendencial es una anomalía.
* **Señal de Desempeño**: La diferencia entre el comportamiento medido y el esperado usada para juzgar si la presa se desempeña de forma aceptable.
* **Modo de Falla Potencial**: Una forma creíble en que una presa podría fallar (p. ej. rebalse, erosión interna, inestabilidad de taludes, filtración de cimentación); la base para elegir los instrumentos.
* **Sobrelevación (Uplift)**: Presión de agua ascendente que actúa en la base de una presa de concreto o dentro de la cimentación, reduciendo la estabilidad.
* **Estructuras Anexas**: Obras auxiliares como vertederos, obras de descarga y desaguaderos que apoyan la presa principal.
* **Asentamiento / Desplazamiento de Coronamiento**: Movimiento vertical u horizontal de la corona de la presa, un indicador clave de deformación.
* **Plan de Vigilancia**: El programa documentado que indica qué se monitorea (visualmente y por instrumento), con qué frecuencia y la respuesta a cada anomalía.
* **Revisión Independiente**: Revisión periódica de los datos de monitoreo y del programa por una parte independiente del equipo operativo, para detectar tendencias normalizadas.

---

## 8. Planificación de Programas de Monitoreo y Confiabilidad (Dunnicliff)

* **Instrumentación Geotécnica**: La medición del comportamiento de suelo, roca, cimentación y estructuras para confirmar el desempeño y detectar cambios.
* **Enfoque de Planificación Sistemática**: El proceso estructurado de Dunnicliff (el "eje") que define primero las preguntas geotécnicas y luego selecciona parámetros, instrumentos, ubicaciones y frecuencia.
* **Pregunta Geotécnica**: Una pregunta específica que el monitoreo debe responder (p. ej. "¿excederá el muro el movimiento admisible?"), que dicta qué se mide y la decisión que se apoya.
* **La Cadena de 25 Eslabones**: La metáfora de Dunnicliff de que el éxito del monitoreo es una cadena desde definir la necesidad del proyecto hasta una lectura que informa una decisión; rompa un eslabón y la cadena falla.
* **Receta de Confiabilidad**: El conjunto de ingredientes (selección, adquisición, instalación, calibración, lectura, mantenimiento, manejo de datos, personas) que hacen confiable al monitoreo.
* **Método de Observación**: Un enfoque de diseño en el que el diseño se refina durante la construcción según el desempeño monitoreado.
* **Transductor**: Dispositivo que convierte una magnitud física (presión, desplazamiento, carga) en una señal eléctrica o neumática.
* **Exactitud vs. Precisión**: La exactitud es la cercanía al valor verdadero; la precisión (repetibilidad) es la cercanía de lecturas repetidas entre sí. Ninguna por sí sola garantiza una buena medición.
* **Histéresis**: La dependencia de la salida de un instrumento de la dirección del cambio (carga vs. descarga).
* **Presupuesto de Error**: El efecto combinado de todas las incertidumbres individuales (sensor, cable, lectura, entorno) que acota la incertidumbre total de medición.
* **Factor de Calibración / Cero / Span**: La pendiente de la relación entrada–salida (factor de calibración), la lectura a entrada cero y el rango a escala completa (span).
* **Lectura Base**: La lectura(es) de referencia tomada tras la instalación y el asentamiento, contra la cual se juzga todo cambio futuro.
* **Carga Piezométrica**: La elevación equivalente de la superficie del agua correspondiente a una presión de poros medida.
* **Retardo Hidráulico**: El retardo de la respuesta de un piezómetro a un cambio de presión de poros, gobernado por la permeabilidad y geometría del suelo y filtro circundantes.
* **Saturación / Desaireación**: El procedimiento de remover el aire del filtro y tubo de conexión de un piezómetro para que responda correctamente a la presión de poros; un paso de instalación crítico, a menudo descuidado.
* **Convergencia**: El acortamiento (cierre) de la distancia entre puntos en un túnel o excavación, que indica movimiento del suelo.
* **Testigo de Desplazamiento (Telltale)**: Dispositivo simple que indica movimiento relativo a través de una junta o sección.
* **Barra Gemela (Sister Bar)**: Galga de cuerda vibrante adosada paralela a una barra de refuerzo para medir la deformación de la barra cuando se empotra en concreto.
* **Sobrecorazón (Overcoring)**: Técnica de alivio de tensión en la que un instrumento de sondeo se aísla mediante sobrecorazón para retrocalcular el estado de tensión in situ de la roca.
* **Gato Plano (Flat Jack)**: Gato hidráulico delgado insertado en una ranura en la roca para medir el alivio de tensión y estimar la tensión in situ.
* **Célula de Presión de Sondeo (BPC)**: Dispositivo embebido en un sondeo para monitorear cambios de tensión en la roca alrededor de una excavación.
* **Célula de Presión de Contacto**: Célula de presión colocada a ras de la interfaz suelo–estructura para medir la tensión de contacto.

## 9. Instrumentación Vial FHWA (alcance FHWA-HI-98-034)

* **Regla de Oro (instrumentación)**: Todo instrumento debe seleccionarse y ubicarse para responder a una pregunta geotécnica específica — si no hay pregunta, no debe haber instrumentación.
* **Cadena de 31 Eslabones**: Los 21 eslabones de planificación más 10 de ejecución que deben sostenerse todos para que un programa de monitoreo tenga éxito; un eslabón débil puede romper la cadena.
* **Célula de Presión de Tierras Empotrada**: Celda plana llena de fluido empotrada en el suelo para medir la tensión total normal a su cara.
* **Relación de Aspecto (célula)**: La relación diámetro-espesor de una célula de presión de tierras; una relación alta reduce el error de medición.
* **Relación de Rigidez Suelo/Célula**: La relación que gobierna cuánto redistribuye una célula de presión de tierras el esfuerzo local, y por tanto su error de medición.
* **Pozo de Observación**: Tubo abierto sin sello subsuperficial; crea una conexión vertical entre estratos y rara vez es adecuado para monitoreo de desempeño.
* **Piezómetro de Tubo Abierto (Casagrande)**: Tubo de punta filtrante; confiable pero con largo retardo hidrodinámico.
* **Piezómetro Neumático**: Diafragma equilibrado por presión de gas mediante tubos gemelos; retardo corto, sin congelamiento, pero dependiente del operador.
* **Piezómetro de Cuerda Vibrante (VW)**: Instrumento de diafragma rígido leído por el cambio de frecuencia del alambre; retardo corto y listo para registrador.
* **Piezómetro Multipunto**: Un solo sondeo con varios sensores para perfilar la presión con la profundidad.
* **Plataforma de Asentamiento**: Placa superficial (a menudo con tubería vertical) que registra el asentamiento del relleno a medida que se construye el terraplén.
* **Punto de Asentamiento Subsurface**: Ancla a profundidad (hincada/lechada o Borros) que registra el asentamiento de una capa enterrada.
* **Medidor de Nivel Líquido**: Tubo y celda llenos de líquido que miden asentamiento o heave por el cambio de presión o nivel de líquido.
* **Extensómetro en Serie**: Pila de anclas en un sondeo que resuelve la deformación en incrementos entre anclas adyacentes.
* **Inclinómetro Horizontal**: Inclinómetro que recorre un tubing horizontal para dar un perfil de asentamiento.
* **Inclinómetro Fijo (In Situ)**: Cadena de sensores dejados en el tubing para monitoreo continuo y automatizado.
* **Indicador de Plano de Cizalla**: Dispositivo que detecta la profundidad a la que se cizalla el tubing del inclinómetro.
* **Monitoreo de Emisión Acústica (EA)**: Detección del sonido de alta frecuencia por deslizamiento y rotura de granos como alerta temprana de inestabilidad en desarrollo.
* **Medidor Demec**: Galga mecánica de deformación superficial que mide el cambio de distancia entre dos discos de referencia.
* **Gato Hidráulico Calibrado**: Gato de orificio pasante usado para aplicar y medir carga en tesado; debe calibrarse porque las lecturas de presión de fluido llevan error por fricción.
* **Célula de Presión de Contacto**: Célula que mide tensión o carga en la interfaz suelo-estructura, en la punta de una pila o en la base de un fuste.
* **Transferencia de Carga (cimentaciones profundas)**: La distribución de carga axial entre fricción de fuste y resistencia en punta, resuelta por galgas de deformación, barras gemelas y testigos.
* **Mejora de Suelos**: Modificación in situ de las propiedades del suelo — por lechada, densificación o drenaje — para hacerlo apto para la construcción.
* **Ensayo de Aceptación (pre-/post-instalación)**: Ensayo que confirma que un instrumento cumple la especificación antes de la instalación y sobrevive tras ella.
* **Hoja de Registro de Instalación**: El registro "as-built" de posición, profundidad, sello y valores de calibración vigentes — el registro permanente que hace interpretables los datos.
* **Gráfico Causa-Efecto**: Gráfico del cambio medido contra un factor influyente (carga, lluvia, altura de relleno) para revelar relaciones.
* **Implementación (eslabón final)**: Actuar sobre los datos interpretados — el paso que hace valioso el monitoreo.

## 10. Ingeniería de Cimentaciones y Mecánica de Suelos (alcance de dominio público USACE / FHWA)

* **Tensión Efectiva ($\sigma'$)**: La tensión llevada por el esqueleto del suelo — tensión total menos presión de poros; la tensión que realmente controla la resistencia y la deformación.
* **Presión de Poros ($u$)**: La presión del agua en los vacíos; positiva bajo el nivel freático y negativa (succión) sobre él.
* **Tensión Total ($\sigma$)**: La tensión llevada por el esqueleto del suelo y el agua de los poros juntos; $\sigma = \sigma' + u$.
* **Índice de Vacíos ($e$)**: El volumen de vacíos por unidad de volumen de sólidos.
* **Porosidad ($n$)**: El volumen de vacíos por unidad de volumen total.
* **Grado de Saturación ($S$)**: La fracción del volumen de vacíos llena con agua.
* **Límites de Atterberg ($LL$, $PL$, $SL$)**: Los contenidos de agua que marcan las transiciones entre los estados sólido, plástico y líquido de un suelo de grano fino.
* **Índice de Plasticidad ($PI$)**: El rango de contenido de agua en el que un suelo es plástico; $PI = LL - PL$.
* **SUCS (Sistema Unificado de Clasificación de Suelos)**: La clasificación de ingeniería de dos letras de los suelos (p. ej. CL, SP, GW) basada en gradación y plasticidad.
* **Curva de Compactación**: El gráfico del peso unitario seco contra el contenido de agua; su pico define el contenido de humedad óptimo.
* **Contenido de Humedad Óptimo (CHO)**: El contenido de agua al que un esfuerzo de compactación dado produce el máximo peso unitario seco.
* **Ensayo Proctor (Estándar / Modificado)**: El ensayo de compactación de laboratorio que define la relación humedad–densidad usada para el control de campo.
* **Ley de Darcy**: La relación lineal entre la velocidad de filtración y el gradiente hidráulico, $v = ki$.
* **Coeficiente de Permeabilidad ($k$)**: La constante que vincula la velocidad de flujo con el gradiente hidráulico para un suelo dado.
* **Red de Flujo**: Solución gráfica de la ecuación de Laplace, dibujada como líneas de flujo y equipotenciales ortogonales.
* **Gradiente de Salida**: El gradiente hidráulico en la superficie aguas abajo; si excede el valor crítico, comienza la tubificación.
* **Estado de Licuación / Tubificación**: El estado en el que la filtración ascendente reduce la tensión efectiva a cero y el suelo hierve.
* **Consolidación**: La compresión dependiente del tiempo de un suelo saturado a medida que el agua de poros drena y la tensión efectiva aumenta.
* **Coeficiente de Consolidación ($c_v$)**: El parámetro que gobierna la tasa de consolidación primaria.
* **Índice de Compresión ($C_c$)**: La pendiente de la porción virgen de la curva $e$–$\log\sigma'$.
* **Presión de Preconsolidación ($\sigma'_p$)**: La máxima tensión efectiva que un suelo ha soportado nunca.
* **Relación de Sobreconsolidación ($OCR$)**: La presión de preconsolidación dividida por la tensión efectiva presente; $OCR = 1$ es normalmente consolidado.
* **Criterio de Mohr–Coulomb**: Falla cuando la tensión de corte alcanza $\tau = c' + \sigma'\tan\phi'$.
* **Cohesión ($c'$)**: La intersección de resistencia al corte del envelope de falla a tensión normal efectiva cero.
* **Ángulo de Fricción Interna ($\phi'$)**: La pendiente del envelope de Mohr–Coulomb, reflejando la fricción interpartícula y el entrelazamiento.
* **Resistencia al Corte No Drenada ($c_u$ / $s_u$)**: La resistencia al corte de una arcilla saturada medida sin drenaje.
* **Capacidad de Carga ($q_{ult}$)**: La presión máxima que el suelo de cimentación puede llevar antes de la falla por corte.
* **Presión de Apoyo Admisible ($q_{all}$)**: La presión de diseño obtenida tras aplicar un factor de seguridad y límites de asentamiento.
* **Asentamiento**: El movimiento vertical descendente de una cimentación bajo carga.
* **Asentamiento Diferencial**: La diferencia de asentamiento entre puntos de una estructura; gobierna la distorsión y el daño.
* **Fricción de Piel**: La resistencia al corte desarrollada a lo largo del fuste de una pila o pilote perforado.
* **Resistencia en Punta**: La resistencia movilizada en la base de una cimentación profunda.
* **Fricción Negativa (Downdrag)**: Arrastre descendente sobre un pilote cuando el suelo circundante se asienta relativo a él.
* **Eficiencia de Grupo de Pilotes**: La relación entre la capacidad de un grupo de pilotes y la suma de las capacidades de los pilotes individuales.
* **Empuje de Tierras (En Reposo / Activo / Pasivo)**: La tensión horizontal que un suelo ejerce sobre una estructura de contención — mínima cuando el muro cede (activo) y máxima cuando se empuja contra el suelo (pasivo).
* **Coeficiente de Empuje de Tierras ($K_0$, $K_a$, $K_p$)**: La relación entre la tensión horizontal y vertical efectiva en los estados en reposo, activo y pasivo.
* **Coeficiente de Seguridad (talud)**: La relación entre la resistencia al corte disponible y la tensión de corte requerida para el equilibrio.
* **Ensayo de Penetración Estándar ($SPT$, valor $N$)**: Un ensayo de cuchara partida hincada cuyo recuento de golpes indexa la densidad y resistencia del suelo.
* **Ensayo de Penetración de Cono ($CPT$)**: Un cono empujado que da resistencia de punta y fricción de camisa continuas con la profundidad.
* **Licuación**: Pérdida de resistencia en arena suelta saturada bajo carga cíclica cuando la presión de poros se acerca a la tensión total.
* **Suelo Expansivo**: Arcilla que se hincha al humedecerse y se contrae al secarse, causando heave y agrietamiento.
* **Suelo Colapsable**: Suelo que sufre reducción de volumen súbita al humedecerse a carga constante.

---

*Véase también: [Marco Normativo (LatAm / España)](../compliance/decree-114-tcvn-9398.md) · [Sandbox Interactivo](../visualizer.md) · [Monitoreo de Presas (Aplicaciones)](../applications/dam-monitoring.md)*
