---
lang: es
lang_alt: reference-manuals/monitoring-dam-performance/chapter-09-automated/
---

# Capítulo 9 — Sistemas de Monitoreo Automatizado, Remoto y en Tiempo Real

## 9.1 Cuándo automatizar

La automatización vale la pena cuando:

- La presa es **remota o peligrosa** de visitar con frecuencia.
- Se necesitan datos de **alta frecuencia** (durante el llenado, tras sismos/
  inundaciones).
- Importa la **captura de eventos** (una tormenta o evento sísmico que ningún
  inspector podría atender).
- Las **alarmas** deben dispararse de inmediato al superar un umbral.

## 9.2 Componentes del sistema

Un sistema automatizado moderno tiene cuatro capas:

1. **Sensores** — los instrumentos de los [Capítulos 5–8](chapter-05-instruments.md).
2. **Adquisidores de datos** — exploran los sensores, sellan con marca de tiempo y
   almacenan lecturas.
3. **Telemetría** — celular, satelital, radio o fibra transportan los datos fuera del
   sitio.
4. **Software** — almacena, valida, grafica y alerta.

## 9.3 Energía y comunicaciones

Los sitios remotos necesitan energía (solar + batería es común) y una ruta de
comunicación. Cada uno añade modos de falla: baterías muertas, pérdida de cobertura
celular y cables dañados por roedores son rutinarios. Diseñe con **redundancia y
autodiagnóstico**.

## 9.4 Umbrales y alarmas

La automatización es más valiosa cuando **alerta**. Un buen sistema de alarma define:

- **Niveles de acción** — valores o tasas de cambio que disparan revisión.
- **Escalamiento** — a quién se notifica y cómo.
- **Gestión de falsas alarmas** — filtrar picos de tendencias reales para mantener la
  confianza en el sistema.

!!! warning "Las alarmas que gritan lobo se ignoran"
    Las alarmas demasiado sensibles entrenan a los operadores para ignorarlas.
    Calibre los umbrales a cambios significativos y suprima fuentes de ruido conocidas
    (temperatura, marea, caídas de energía).

## 9.5 Validación de datos en el borde

Los sistemas automatizados deben marcar datos obviamente malos —fuera de rango,
congelados (sin cambio) o con caídas— antes de que lleguen al ingeniero. Las reglas
de validación detectan fallas de sensor y comunicaciones a tiempo.

## 9.6 Tiempo real durante eventos

Durante una inundación o un sismo, los datos en tiempo real permiten al propietario
operar el embalse y despachar inspección donde los datos muestran movimiento —
convirtiendo una emergencia a ciegas en una gestionada.

## 9.7 Puntos clave

- Automatice por remotía, frecuencia, captura de eventos y alarmas.
- Un sistema tiene sensores, adquisidores, telemetría y software —cada uno un punto
  de falla.
- Diseñe umbrales que alerten ante cambios reales sin gritar lobo.
- Valide datos en el borde y use datos en tiempo real para gestionar eventos.
