---
lang: es
lang_alt: reference-manuals/geovadis-vol2/chapter-03-rock-mechanics-tunnelling/
---

# Mecánica de Rocas e Ingeniería de Tunelización

!!! abstract "Resumen de la Sesión"
    La Sesión 8 de *GeoVadis (GAIC 2025)* presenta avances de vanguardia en caracterización de macizos rocosos, tunelización mecanizada con escudo (TBM), almacenamiento subterráneo de carbono y mitigación del riesgo de desprendimientos. Las contribuciones centrales examinan la geofísica sísmica de sondeo previo al frente, el modelado numérico 3D de interacciones entre túneles múltiples, el retroanálisis de la pérdida de volumen de terreno, el acoplamiento hidromecánico en el secuestro de carbono y las redes de alerta temprana habilitadas por IoT.

---

## 1. Geofísica Sísmica de Sondeo Previo al Frente en Túneles (S.C. Chian, Y.Z. Tan, Y.E. Li, C.H.A. Cheng)

### Prevención de Desastres Geológicos Subterráneos
Los encuentros imprevistos con zonas de cizalla de falla, cavernas kársticas o entradas de agua a alta presión durante la excavación provocan colapsos catastróficos y retrasos de obra. Chian y cols. presentan sistemas avanzados de **Predicción Sísmica en Túnel (TSP)**:
- **Propagación y Reflexión de Ondas:** Las ondas sísmicas de alta frecuencia generadas por microvoladuras o impactos neumáticos en la pared lateral se reflejan en las fronteras de impedancia acústica por delante del frente del túnel.
- **Alcance del Sondeo Previo:** Acelerómetros triaxiales montados sobre el revestimiento procesan los hodogramas de reflexión de ondas P y S, obteniendo imágenes precisas de discontinuidades geológicas y zonas de fractura hasta $100\,\text{m} - 150\,\text{m}$ por delante del frente de excavación.
- **Protocolo de Seguridad:** Las inversiones geofísicas en tiempo real alertan al equipo de excavación para realizar sondeos exploratorios e inyección de consolidación preventiva antes de avanzar hacia zonas de falla acuíferas.

```
       Perfil del Túnel y Geometría Geofísica de Sondeo Previo
       ┌───────────────────────────────┐
       │ Cavidad de Túnel Excavada     │
       │                               │
       │  Sonda Sísmica Emisora        │
       │    (Impacto Lateral / Voladura)│
       │          ●                    │   Ondas Sísmicas P y S Irradian al Frente
       │          │ ╲                  │   ─────────►  ─────────►
       │          │   ╲                │
       │  Arreglo de Acelerómetros     │
       │    de Recepción en Revestimiento│
       │    ▲   ▲   ▲   ▲   ▲          │
       ├───────────────────────────────┤   ◄─── Frente de Excavación
       │                               │
       │      Macizo Rocoso no Excavado│        Zona de Falla / Anomalía de Cavidad
       │                               │        (Caída de Impedancia Acústica)
       │                               │             ║║║║║║║║║║
       │                               │   Ecos      ║║║║║║║║║║
       │                               │   Reflejados║║║║║║║║║║
       └───────────────────────────────┘  ◄──────────║║║║║║║║║║
```

---

## 2. Simulación Numérica 3D de la Tunelización Mecanizada con TBM (J. Agarwal, G. Garg y cols.)

### Tunelización con Escudo Multietapa en Estratos Estratificados
Mediante MIDAS GTS-NX, Agarwal y su equipo realizan simulaciones 3D por elementos finitos totalmente acopladas del avance de una TBM de Equilibrio de Presión de Tierras (EPB) a través de arenas estratificadas y arcillas rígidas:
- **Presión de Sostenimiento del Frente:** La presión de frente se calibra para contrarrestar la presión de tierras horizontal in situ y la presión de agua de poros ($p_{face} = K_0 \sigma'_v + u_w$), evitando la extrusión del frente y los socavones catastróficos en superficie.
- **Anillo de Inyección y Empuje del Revestimiento:** La simulación modela la inyección presurizada de lechada en el hueco de cola ($p_{grout} \approx 200 - 300\,\text{kPa}$), el rozamiento por conicidad del escudo de la TBM y los empujes de los gatos hidráulicos sobre los anillos de dovelas prefabricadas.
- **Cubeta de Asentamiento Transversal:** Los perfiles de asentamiento superficial se ajustan estrechamente a la distribución gaussiana de error de Peck:
  $$S(x) = S_{max} \cdot \exp\left( -\frac{x^2}{2 i^2} \right)$$
  donde el parámetro de anchura de cubeta $i = K \cdot z_0$ se captura con precisión a través de estratos alternos de arcilla y arena.

---

## 3. Respuestas Estructurales de Túneles Existentes frente a Nuevas Perforaciones Adyacentes (J.Q. Lin, J.H. Zhang, X.S. Chen y cols.)

### Tunelización por Proximidad en Espacio Urbano de Alta Densidad
La excavación de túneles gemelos o que se intersectan induce una relajación asimétrica de tensiones en torno a túneles operativos preexistentes:
- **Mecanismos de Deformación:** La redistribución de tensiones provoca distorsión diametral (alargamiento horizontal y achatamiento vertical) de los anillos de dovelas existentes.
- **Apertura de Juntas y Tracción en Pernos:** El corte diferencial entre anillos de dovelas induce apertura circunferencial de juntas y picos agudos de tensión de tracción en los pernos radiales de unión.
- **Protocolos de Mitigación:** La preinyección del pilar de suelo entre túneles y el ajuste de las velocidades de avance limitan la convergencia del túnel existente dentro de los estrictos umbrales de operación ferroviaria ($< 5\,\text{mm}$).

---

## 4. Acoplamiento Hidromecánico en el Secuestro de $\text{CO}_2$ en Acuíferos Salinos (S.M. Chiang, M.C. Weng, H.K. Le y cols.)

### Integridad de la Roca Sello y Reactivación de Fallas
La inyección de dióxido de carbono supercrítico ($\text{scCO}_2$) en acuíferos salinos profundos ($> 1,000\,\text{m}$ de profundidad) incrementa la presión de poros del yacimiento, alterando el campo de tensiones local:
- **Análisis Acoplado Filtración-Tensión:** Chiang y cols. formulan modelos de elementos finitos hidromecánicamente acoplados que gobiernan el flujo bifásico de fluidos y la deformabilidad de la roca porosa.
- **Potencial de Deslizamiento de Falla:** La presión de poros inducida por la inyección reduce la tensión normal efectiva ($\sigma'_n$) sobre las fallas limítrofes, pudiendo desencadenar su reactivación y eventos sísmicos si la presión de inyección supera los umbrales críticos:
  $$\tau \le c' + (\sigma_n - u_{pore})\tan\phi'$$
- **Verificación del Sellado de la Roca Sello:** El estudio cuantifica los caudales máximos sostenibles de inyección que mantienen las tensiones de tracción de la roca sello por debajo de su resistencia a tracción ($f_t$), garantizando cero fugas ascendentes de $\text{CO}_2$.

---

## 5. Sistemas IoT de Alerta en Tiempo Real de Desprendimientos y Flujos de Escombros (R. Budhbhatti, R.R. Mahajan, D. Paldino)

### Redes de Alerta Temprana con Computación en el Borde
Los corredores de autopistas y ferrocarriles que atraviesan taludes rocosos empinados del Himalaya y de zonas alpinas afrontan impactos súbitos de desprendimientos y flujos rápidos de escombros. Budhbhatti y cols. presentan un sistema IoT de monitoreo desplegado en campo:
- **Despliegue de Nodos Sensores:** Inclinómetros MEMS (micro-electro-mecánicos) y células de carga instalados en barreras flexibles de red anular registran impulsos dinámicos de impacto ($E > 500\,\text{kJ}$).
- **Protocolos de Alarma Automatizada (TARP):** Pasarelas inalámbricas LoRaWAN transmiten telemetría a servidores en la nube; cuando la tensión del cable de la barrera o la velocidad de inclinación del poste superan los umbrales de Nivel 3 del Plan de Respuesta por Acción Disparadora (TARP), señales automáticas activan luces de advertencia junto a la vía para detener los trenes que se aproximan.

---

## 6. Suite de Instrumentación de Campo para Mecánica de Rocas y Tunelización

| Aplicación Subterránea / Rocosa | Sensor Primario de Monitoreo | Sensor Redundante Secundario | Parámetro Crítico Monitorizado |
| :--- | :--- | :--- | :--- |
| **Avance del Escudo TBM** | Dianas Láser de Convergencia en Túnel | Extensómetros Multiprofundidad en Sondeo | Ovalización del túnel, cubeta de asentamiento $S(x)$ |
| **Riesgo Geológico Previo al Frente**| Arreglo de Acelerómetros Triaxiales en Túnel | Sondas de Testificación Horizontal | Hodograma de reflexión P/S, proximidad de fallas |
| **Perforación Próxima a Túnel Existente**| Sister Bars / Galgas de Cuerda Vibratoria| Estación Total Robótica de Alta Precisión | Apertura de juntas de dovelas, deformación de flexión del revestimiento |
| **Inyección en Acuífero Salino de $\text{CO}_2$**| Manómetros de Cuarzo en Fondo de Pozo | Red de Monitoreo Microsísmico | Presión de poros del yacimiento, eventos de deslizamiento de falla |
| **Red de Barreras Flexibles contra Desprendimientos**| Inclinómetros MEMS Inalámbricos y Células de Carga | Escáneres LiDAR de Alta Resolución | Carga de impacto en barrera, pérdida de tensión de cable, fluencia del talud |
