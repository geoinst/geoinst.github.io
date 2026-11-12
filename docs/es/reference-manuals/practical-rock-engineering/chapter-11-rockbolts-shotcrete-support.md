---
lang: es
lang_alt: reference-manuals/practical-rock-engineering/chapter-11-rockbolts-shotcrete-support/
---

# Capítulo 11 — Pernos de Roca, Cable-Pernos y Sistemas de Soporte con Shotcrete

## 11.1 Mecanismos fundamentales del soporte

Los sistemas de soporte del terreno estabilizan las excavaciones mediante tres
mecanismos mecánicos distintos:

1. **Suspensión**: suspender bloques de roca de peso propio o capas estratificadas
   sueltas a través de luces inestables, anclándolos a estratos rocosos competentes
   suprayacentes.
2. **Formación de viga (aprisionamiento de laminaciones)**: empernar estratos delgados
   de techo sedimentario crea una viga estructural compuesta. Los esfuerzos normales de
   apriete generan fricción de corte entre estratos, suprimiendo el deslizamiento y
   reduciendo la deflexión del techo en un factor de $n^2$ (donde $n$ es el número de
   laminaciones empernadas).
3. **Arco de roca reforzado (trabazón y confinamiento)**: en roca bloqueada o muy
   fracturada, el empernado en retícula con shotcrete superficial aplica un esfuerzo de
   confinamiento radial ($\sigma_3 > 0$). Esto moviliza la envolvente de resistencia de
   Hoek-Brown y transforma la roca fracturada en un anillo de compresión
   autoportante.

---

## 11.2 Clasificación y selección de pernos de roca

```
A. CASQUILLO DE EXPANSIÓN       B. BARRA DE RESINA TOTALMENTE    C. PERNO DE FRICCIÓN
   MECÁNICA                       INYECTADA                        (SPLIT SET)
   [Ancla]=======[Placa]          [====Resina====][Placa]          [===Tubo expandido===][Placa]
   Anclaje puntual; fluencia      Totalmente acoplado; rígido      Friccional; cedencia dinámica
```

| Tipo de perno | Mecanismo de anclaje | Característica carga–deformación | Aplicación principal |
| --- | --- | --- | --- |
| **Casquillo de expansión mecánico** | Anclaje puntual acuñado en la roca por un casquillo dentado | Respuesta elástica inicial rígida; susceptible de aflojamiento por vibración de voladura | Soporte temporal de minería en roca dura y competente |
| **Barra corrugada con resina totalmente inyectada** | Adherencia continua a lo largo de barra de acero corrugada mediante cartuchos de resina de poliéster | Alta rigidez ($> 100\text{ kN/mm}$); curado rápido ($30\text{ s}$); excelente protección anticorrosiva | Túneles civiles y galerías permanentes de minería subterránea |
| **Estabilizador de fricción (Split Set)** | Tubo de acero ranurado en C hincado en un taladro de menor diámetro ($38\text{ mm}$ en taladro de $35\text{ mm}$) | Cedencia friccional a lo largo de la longitud ($10 - 15\text{ kN/m}$ de empotramiento); gran capacidad de desplazamiento | Tajeos de minería de gran deformación; fijación temporal de hastiales |
| **Tubo inflable (Swellex)** | Tubo de acero plegado expandido hidráulicamente con agua a alta presión ($30\text{ MPa}$) | Trabazón mecánico inmediato en toda la columna; alta capacidad ($100 - 200\text{ kN}$) con ductilidad moderada | Instalación rápida en tunelización; macizos rocosos con agua |
| **Perno de roca cedente (D-Bolt, Garford)** | Barra lisa con cuñas de anclaje diseñadas o puntos engrosados | Se deforma hasta $150 - 200\text{ mm}$ bajo carga alta constante ($180 - 220\text{ kN}$) | Terrenos propensos a estallido de roca y de aprisionamiento severo |

---

## 11.3 Shotcrete reforzado con fibra de acero (SFRS)

El shotcrete (hormigón proyectado) actúa como una piel estructural flexible y de acción
rápida.

### Ventajas del shotcrete reforzado con fibra de acero:
1. **Elimina el peligro de la malla metálica**: proyectar las fibras directamente evita
   la instalación manual, lenta y peligrosa, de malla electrosoldada contra frentes de
   roca sin soportar.
2. **Tenacidad post-fisuración**: mientras el shotcrete sin reforzar falla frágilmente en
   cuanto se fisura, las fibras de acero dúctiles ($30 - 50\text{ kg/m}^3$ de mezcla)
   puentean las bocas de las fisuras, aportando capacidad sustancial de absorción de
   energía (clases de absorción del sistema $Q$: $500\text{ J}, 700\text{ J}, 1000\text{ J}$).
3. **Ganancia de resistencia temprana**: los aditivos acelerantes alcanzan resistencias
   a compresión de $1\text{ MPa}$ en 1 hora y $10\text{ MPa}$ en 24 horas, proporcionando
   soporte inmediato tras frentes de perforación y voladura o de TBM en avance.

---

## 11.4 Interacción del soporte y compatibilidad del sistema

El modo de falla más común de los sistemas de soporte es la **incompatibilidad de
deformaciones**:

- Combinar un soporte rígido y frágil (shotcrete grueso sin reforzar) con un perno de
  roca flexible (Split Set) hace que el shotcrete se fisure y desconche con $2\text{ mm}$
  de deformación, mucho antes de que los pernos movilicen su capacidad a tracción.
- **La regla de oro del diseño de soporte**: los componentes del soporte (piel
  superficial, tendón, anclaje) deben poseer capacidades de desplazamiento
  concordantes y deformarse armónicamente bajo la dilatación prevista del macizo
  rocoso.

---

## 11.5 Terminología canónica

| Español | Inglés | Vietnamita (canónico) | Definición |
| --- | --- | --- | --- |
| Barra de resina | Resin rebar | Neo thanh thép dính kết bằng vữa nhựa | Perno de acero corrugado adherido con cartuchos de resina de poliéster |
| Estabilizador de fricción / Split Set | Friction stabilizer / Split Set | Neo ma sát dạng ống xẻ rãnh | Tubo ranurado hincado en taladro de menor diámetro que desarrolla resistencia friccional |
| Shotcrete reforzado con fibra de acero (SFRS) | Steel fiber reinforced shotcrete (SFRS) | Bê tông phun gia cường sợi thép (SFRS) | Hormigón proyectado con fibras de acero con extremos ganchudos para tenacidad post-fisuración |
| Capacidad de absorción de energía | Energy absorption capacity | Khả năng hấp thu năng lượng dẻo | Tenacidad del shotcrete reforzado medida por la energía absorbida bajo deflexión |
| Incompatibilidad de deformaciones | Strain incompatibility | Không tương thích về mặt biến dạng | Desajuste de capacidad de deformación que provoca falla prematura de componentes rígidos |
