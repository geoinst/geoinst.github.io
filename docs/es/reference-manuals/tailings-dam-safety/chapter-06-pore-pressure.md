---
lang: es
lang_alt: reference-manuals/tailings-dam-safety/chapter-06-pore-pressure/
---

# Capítulo 6 — Monitoreo de la Presión de Poros y del Potencial de Licuefacción

## 6.1 Por qué la presión de poros es el parámetro central

Los mecanismos dominantes de falla de relaves —**licuefacción estática y sísmica**—
están gobernados por la presión de poros. Cuando relaves sueltos y saturados llevan
una presión de poros alta (bajo esfuerzo efectivo), pueden perder resistencia de forma
catastrófica. Por ello, monitorear la presión de poros es la piedra angular de la
vigilancia de relaves.

## 6.2 Tipos de piezómetros

| Tipo | Principio | Mejor para |
|------|-----------|------------|
| **Cuerda vibratoria (VW)** | Cambio de frecuencia de un alambre tensado | Monitoreo automatizado a largo plazo; robusto |
| **Neumático** | La presión de gas equilibra la presión del agua | Remoto, sin energía necesaria |
| **Tubo abierto (standpipe)** | Nivel de agua en un tubo | Simple, directo, pero lento para equilibrarse |
| **Hidráulico (de doble tubo)** | Equilibrio de columna de líquido | Varios puntos, método establecido |

## 6.3 Indicadores del potencial de licuefacción

El monitoreo de presión de poros respalda la evaluación de licuefacción mediante:

- **Relación de presión de poros** $r_u = u / \sigma'_v$ — la relación entre la presión
  de poros y el esfuerzo vertical efectivo inicial; un $r_u$ alto o creciente señala
  resistencia perdida.
- **Presión de poros en exceso** generada durante o después de eventos sísmicos, medida
  por piezómetros de respuesta rápida.
- **Correlación con ensayos in situ** (SPT, CPT, velocidad de onda de corte) que
  caracterizan la soltura del depósito.

!!! warning "La saturación es todo"
    Un piezómetro VW o neumático que no está saturado da resultados sin sentido. El
    **procedimiento de saturación** —eliminar el aire del filtro poroso y del tubo de
    conexión— debe hacerse con cuidado en la instalación
    ([Dunnicliff Cap. 9](../dunnicliff/index.md)). Un piezómetro nunca saturado
    adecuadamente es un vacío silencioso en el programa.

## 6.4 Colocación

Los piezómetros se colocan para detectar los modos de falla del
[Capítulo 2](chapter-02-facilities-and-failures.md):

- **Dentro del depósito y la playa** para seguir la superficie freática y las zonas de
  alto $r_u$.
- **En los pies de los terraplenes** (especialmente elevaciones por método aguas
  arriba) para detectar acumulación de presión en el material más débil.
- **En la cimentación** donde hay capas débiles o licuables.
- **Varias profundidades** en un solo barreno (multinivel / MPBX) para perfilar la
  presión de poros con la profundidad.

## 6.5 Lectura e interpretación

Las lecturas se convierten en **carga piezométrica** (elevación equivalente de la
superficie de agua). Interpretaciones clave:

- **Aumento sostenido sin subir la laguna** → posible obstrucción, mayor filtración o
  falla del sensor.
- **Retraso de la presión de poros** respecto al nivel de laguna → indica drenaje y
  permeabilidad.
- **$r_u$ acercándose a los valores usados en diseño** → preocupación de licuefacción.
- **Presión en exceso rápida post-sísmica** → dispara evaluación inmediata.

## 6.6 Fallas comunes

- **Entrada de aire / pérdida de saturación** → lecturas a la deriva o sin respuesta.
- **Cortocircuito del barreno** → lee la zona equivocada.
- **Daño de cable / electrónica** → la falla de instrumento automatizado más común.

## 6.7 Puntos clave

- La presión de poros gobierna las fallas dominantes por licuefacción.
- Siga la relación de presión de poros $r_u$ como indicador de licuefacción.
- Sature adecuadamente cada piezómetro; verifíquelo.
- Coloque los instrumentos en la playa, los pies y la cimentación —donde nacen los modos.
