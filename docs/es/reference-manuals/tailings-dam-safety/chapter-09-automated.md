---
lang: es
lang_alt: reference-manuals/tailings-dam-safety/chapter-09-automated/
---

# Capítulo 9 — Sistemas Automatizados, Remotos y en Tiempo Real

## 9.1 Por qué automatizar

Las instalaciones de relaves operan continuamente y pueden fallar entre lecturas
manuales. Los sistemas automatizados proveen datos **continuos, sin atención** y
pueden disparar alarmas cuando nadie está en el sitio —esenciales para instalaciones
de mayor consecuencia.

## 9.2 Componentes de un sistema automatizado

- **Sensores** — piezómetros VW, inclinómetros in situ, prismas, sensores de nivel.
- **Adquisidores de datos** — exploran sensores, aplican conversión, sellan con marca
  de tiempo y almacenan datos.
- **Telemetría** — celular, satelital, radio o fibra para mover datos fuera del sitio.
- **Base de datos y tablero central** — donde los datos se validan, grafican y
  revisan ([Capítulo 11](chapter-11-data-management.md)).
- **Motor de alarma** — compara lecturas con niveles de disparo/acción y notifica a los
  respondedores ([Capítulo 13](chapter-13-decisions.md)).

## 9.3 Radar satelital (InSAR)

La Interferometría de Radar de Apertura Sintética (InSAR / A-DInSAR) desde satélites
mide el desplazamiento del terreno sobre toda la instalación y sus alrededores con
precisión milimétrica, sin instrumentos en sitio. Es ideal para:

- Detectar movimiento **regional o inesperado**.
- Cubrir instalaciones remotas o grandes económicamente.
- Proveer una verificación independiente de los instrumentos puntuales.

Sus limitaciones —intervalos de revisita de días, sensibilidad principal a movimiento
vertical y en la dirección de mira, efectos de vegetación— significan que **complementa**,
no reemplaza, los instrumentos de terreno.

## 9.4 Alerta y umbrales en tiempo real

Los sistemas automatizados solo son útiles si **alertan**. Diseñe:

- Niveles de disparo y acción claros por parámetro.
- Rutas de comunicación redundantes (un módem celular fallido es un punto ciego).
- Rutas de escalamiento y responsabilidad de guardia.
- Pruebas periódicas de la ruta de alarma (no descubra que está rota durante un evento).

!!! warning "La automatización necesita mantenimiento"
    Los sistemas automatizados fallan en silencio si se descuidan: baterías muertas,
    sensores obstruidos, cables rotos, SIM vencidas. Un plan de mantenimiento
    ([Capítulo 10](chapter-10-iom.md)) y pruebas periódicas de alarma de extremo a
    extremo son obligatorios.

## 9.5 Independencia y resiliencia

Para instalaciones de alta consecuencia, los reguladores esperan cada vez más
monitoreo **independiente** —sistemas y rutas de datos no dependientes del sistema de
control operativo— de modo que una caída en todo el sitio no deje también ciega a la
vigilancia.

## 9.6 Puntos clave

- La automatización da cobertura continua, sin atención y con alarmas.
- El InSAR añade cobertura de toda la instalación a escala mm sin sensores en sitio.
- Diseñe niveles de disparo reales, rutas redundantes y escalamiento probado.
- Sistemas independientes y mantenidos son esperados para instalaciones de alta
  consecuencia.
