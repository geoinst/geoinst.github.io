---
lang: es
lang_alt: reference-manuals/practical-rock-engineering/chapter-06-acceptable-design/
---

# Capítulo 6 — ¿Cuándo es Aceptable un Diseño de Ingeniería de Rocas?

## 6.1 La falacia de un único factor de seguridad

En el diseño clásico de acero estructural u hormigón armado, un Factor de Seguridad
($FS$) determinista entre $1,5$ y $2,0$ garantiza la seguridad porque las propiedades
de los materiales se fabrican bajo normas de calidad estrictas con coeficientes de
variación pequeños ($COV < 10\%$).

En ingeniería geotécnica y de rocas, en cambio:
- Las propiedades del macizo rocoso presentan una dispersión espacial enorme ($COV$ de
  la resistencia intacta a menudo $20 - 40\%$; persistencia de juntas y GSI a menudo
  $15 - 35\%$).
- Un talud diseñado con un $FS = 1,3$ determinista calculado con parámetros medios
  puede tener una **Probabilidad de Falla ($P_f$) superior al $20\%$** si la desviación
  estándar de la fricción de juntas o de la presión de poros es alta.
- A la inversa, un talud con $FS = 1,15$ donde la incertidumbre geotécnica es mínima
  puede tener $P_f < 1\%$.

**Un único factor de seguridad determinista carece de sentido si no se especifican la
incertidumbre asociada y las consecuencias de la falla.**

---

## 6.2 Factor de seguridad determinista ($FS$) frente a probabilidad de falla ($P_f$)

```
             RESISTENCIA R (Capacidad)
                 \       /
                  \     /
                   \   /
                    \ /
                     X  <--- ZONA DE SOLAPAMIENTO: Probabilidad de falla Pf
                    / \
                   /   \
                  /     \
                 /       \
             CARGA S (Demanda)
```

1. **Margen de seguridad determinista**:

$$FS = \frac{\text{Capacidad media } \bar{R}}{\text{Demanda media } \bar{S}} = \frac{\sum \text{Fuerzas resistentes}}{\sum \text{Fuerzas motoras}}$$

2. **Índice de confiabilidad ($\beta$)**:
   Suponiendo que la capacidad $R$ y la demanda $S$ son variables normalmente
   distribuidas:

$$\beta = \frac{\bar{R} - \bar{S}}{\sqrt{\sigma_R^2 + \sigma_S^2}}$$

   La probabilidad de falla se relaciona directamente mediante la distribución normal
   acumulada estándar:

$$P_f = \Phi(-\beta)$$

3. **Simulación de Monte Carlo**:
   En lugar de calcular un único $FS$, los parámetros de entrada ($c', \phi',
   \text{GSI}, r_u$) se muestrean de distribuciones de probabilidad estadísticas
   (normal, lognormal, beta) a lo largo de $10.000$ iteraciones:

$$P_f = \frac{\text{Número de iteraciones con } FS < 1,0}{\text{Número total de corridas de Monte Carlo}}$$

---

## 6.3 Criterios de riesgo aceptable por sector

El Dr. Hoek estableció criterios objetivo que equilibran la inversión económica frente
a la consecuencia de la falla:

| Tipo de instalación | Categoría de consecuencia | $FS$ determinista mínimo (estático) | $P_f$ máxima aceptable |
| --- | --- | --- | --- |
| **Bancos temporales de mina a cielo abierto** | Baja (derrame localizado de banco, sin exposición de personal) | $1,1 - 1,2$ | $15\% - 30\%$ |
| **Rampas principales de acarreo / muros altos de mina** | Moderada (interrupción del acarreo, pérdida económica) | $1,3$ | $5\% - 10\%$ |
| **Taludes permanentes de carreteras civiles** | Alta (tráfico público, alteración del comercio) | $1,5$ | $1\%$ |
| **Estribos de presas y cavernas hidroeléctricas** | Extrema (rotura catastrófica de presa o pérdida de vidas) | $1,5 - 2,0$ | $< 0,1\%$ |

---

## 6.4 El papel de los Planes de Respuesta por Umbral de Activación (TARP)

Como la ingeniería de rocas acepta incertidumbre residual, las operaciones deben vincular
el monitoreo en tiempo real con matrices de acción **TARP** explícitas:

- **Nivel 1 (Verde — operación normal)**: velocidad de deformación $< 1,0\text{ mm/día}$;
  presión de poros por debajo de la línea freática de diseño. Continúa la minería o
  tunelización normal.
- **Nivel 2 (Ámbar — aviso / vigilancia reforzada)**: la velocidad sube a
  $2 - 5\text{ mm/día}$ o se detecta tendencia acelerada. Se duplica la frecuencia de
  lectura de sensores; se instalan cable-pernos suplementarios; se inspeccionan grietas
  de tracción.
- **Nivel 3 (Rojo — evacuación inmediata)**: el análisis de velocidad inversa
  ($1/v \to 0$) indica el inicio de falla por fluencia terciaria. Se activan alarmas; se
  retira todo el personal y equipo; se aísla la zona.

---

## 6.5 Terminología canónica

| Español | Inglés | Vietnamita (canónico) | Definición |
| --- | --- | --- | --- |
| Factor de Seguridad (FS) | Factor of Safety (FS) | Hệ số an toàn (FS) | Razón entre el total de fuerzas resistentes y las fuerzas motoras |
| Probabilidad de falla ($P_f$) | Probability of failure ($P_f$) | Xác suất phá hoại ($P_f$) | Probabilidad estadística de que la demanda supere la capacidad |
| Índice de confiabilidad ($\beta$) | Reliability index ($\beta$) | Chỉ số độ tin cậy ($\beta$) | Número de desviaciones estándar que separan el margen medio de la falla |
| Simulación de Monte Carlo | Monte Carlo simulation | Mô phỏng Monte Carlo | Método computacional que evalúa distribuciones probabilísticas |
| Plan de Respuesta por Umbral de Activación (TARP) | Trigger Action Response Plan (TARP) | Kế hoạch ứng phó ngưỡng kích hoạt (TARP) | Matriz documentada que vincula umbrales de sensores con respuestas operativas |
