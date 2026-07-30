# Cuánto cuesta una semana de atraso — marco para cuantificar el dolor de obra

> Marco de referencia para **estimar el costo económico de una semana de atraso** en un proyecto residencial, con evidencia de la literatura. Sustenta la afirmación de la propuesta de Field: *"si Field evita un atraso en los doce meses, se pagó solo."*
>
> **Regla de oro (rigor intelectual):** hay evidencia sólida para dar **rangos y órdenes de magnitud**, pero **no** para afirmar cifras exactas y universales. Un rango defendible con supuestos explícitos es más creíble —y más difícil de refutar— que un número preciso inventado. Ver §5 "Qué NO afirmar".

Proyecto de referencia: **Macarena** — contrato llave en mano **$8.000M COP** (≈ **USD 2M** a ~$4.000/USD), **12 meses**. Ver también: `reporte-constructoras-colombia.md`.

---

## 1. Qué dice la evidencia (lo defendible)

**Los atrasos y sobrecostos son la norma, no la excepción**, y en Latinoamérica el problema es más agudo por debilidades de planeación y ejecución. El BID señala que la eficiencia de entrega de infraestructura en la región tiene espacio relevante de mejora, con el mayor peso en la fase de *delivery* (ejecución).[^bid][^cost-overrun-review]

**Rework (retrabajo) — la evidencia más sólida:**
- CII (359 proyectos, citado por ASCE): costos **directos** de rework ≈ **5%** del costo total de construcción.[^cii]
- Love & Edwards (Australia): rework **6.4% directo + 5.9% indirecto** del valor del contrato.[^love]
- Get It Right Initiative: rangos reportados de **3% a 15%** del valor del contrato.[^giri]
- → Para un residencial de USD 2M, un envelope de contingencia por rework **3%–7% (centro 5%)** es defendible si no hay mejor dato del contratista. **No** todo es atribuible a atraso, pero sí hay base empírica de que el rework consume varios puntos del presupuesto.

**Costos indirectos y "delay damages":** para cuantificar una semana de atraso lo clave no es el costo directo extra, sino el **costo de mantener el proyecto abierto** una semana más: administración de obra, supervisión, instalaciones temporales, seguros, vigilancia, equipos en sitio, overhead de campo y —según contrato— parte del overhead de oficina.[^love][^giri]

**Overhead de oficina (fórmula Eichleay):** mecanismo jurisprudencial (EE.UU.) para calcular overhead de oficina *no absorbido* durante demoras. Útil como **techo conceptual**, no como regla automática: la crítica es que supone una relación mecánica entre facturación y overhead y exige probar *standby* y demora compensable.[^capital][^eichleay] → Para un boutique en Colombia, mejor **costo real de prolongación** y usar Eichleay solo como referencia superior.

**Causa raíz por mala información:** hay respaldo a que la **información incompleta/faltante** y la comunicación pobre entre diseño, contratista y suministro alimentan errores y rework.[^giri] Esto es exactamente lo que Field ataca (centralizar y verificar lo que ya circula en la obra).

**Latencia "ocurre → se detecta":** la evidencia publicada es **más débil** de lo que se asume. Los sistemas tradicionales son reactivos (reportes periódicos, comunicación fragmentada) y falta detección temprana, pero **no hay un benchmark universal de "X días de latencia".** → cualquier cifra puntual de latencia es **supuesto de proyecto**, no constante empírica.[^radman]

**Tecnología de monitoreo (dron/BIM/visión por computador):** la evidencia favorece que **detectan desvíos antes y con menos fricción** y mejoran coordinación, pero la mayoría son pilotos/revisiones, no pruebas causales a gran escala. El estudio en Chile (UAV + fotogrametría + BIM 4D en un residencial de concreto) confirma efectividad para monitorear avance físico y comunicar a stakeholders. **No** existe un "reduce el atraso en Z%" generalizable.[^uav][^cv1][^cv2]

---

## 2. Modelo defendible de 3 capas (para presentar a un CFO)

### Capa 1 — Costo base de prolongación semanal
Costo incremental de tener la obra **abierta una semana más** (no el burn de producción, sino los indirectos de sostenimiento):

```
C_semana_base = (C_campo_fijo_diario + C_oficina_asignable_diario + C_sitio_y_equipos_temporales_diario) × 7
```
Incluye: nómina fija de obra y administración · vigilancia, cerramiento, bodegaje · servicios provisionales · arriendo/depreciación de equipos y andamios · seguros/primas extendidas · overhead de oficina imputable (si el contrato lo permite).

### Capa 2 — Factor de riesgo por atraso
Ajuste por **productividad perdida, reprogramación y fricción de coordinación**, expresado como **% del costo semanal base** (no como número arbitrario). Rango prudente ilustrativo: **+15% a +40%**.

### Capa 3 — Ajuste por rework y claims
Separado de la mera prolongación (no son lo mismo). Modelable como **% del contrato** (3%–7%, centro 5%) o por partidas sensibles a cambios/errores; imputar solo la fracción razonablemente atribuible a detección tardía.[^cii][^love][^giri]

> Además de estas 3 capas (lente **operativo/contratista**), para un **desarrollador** existe un cuarto lente, normalmente el mayor: el **costo financiero / TIR** (§4, Lente B).

---

## 3. Variables a pedirle al cliente (inputs del modelo)

- Cronograma base con **ruta crítica y holguras**.
- **Costo directo mensual** de obra y **burn rate** mensual.
- **Nómina fija** de obra y administración.
- Costos (diarios/mensuales) de **vigilancia, cerramiento, bodegaje, servicios provisionales**.
- **Arriendo/depreciación** de equipos y andamios.
- **Overhead de oficina** imputable al proyecto.
- Historial de **cambios, RFIs, NCRs, submittals y retrabajos**.
- **Curva S** plan vs. real y **productividad real** por frente.
- Términos contractuales sobre **compensable delay**, extensión de plazo y costos indirectos.

---

## 4. Aplicación a Macarena — nota ejecutiva (ilustrativa)

> ⚠️ **Cifras ilustrativas** con heurísticas de la literatura, a validar con los inputs de §3. Sirven para dimensionar el orden de magnitud, no como cotización.

Base: contrato directo **$8.000M COP / 12 meses** → burn directo promedio ≈ **$667M/mes**.

### Lente A — Costo de prolongación (operativo)
Los **indirectos de obra** (site overhead) típicamente corren **8%–15%** del costo directo.
- Indirectos totales estimados: 8.000M × (8%–15%) ≈ **$640M–$1.200M** en 12 meses → **$53M–$100M/mes**.
- **Costo de prolongación por semana** (÷ 4.33) ≈ **$12M–$23M COP/semana** (≈ **USD 3.000–5.750**).
- Con Capa 2 (+15%–40% por productividad/coordinación): **~$14M–$32M COP/semana**.

### Lente B — Costo financiero / TIR (para el inversionista)
Es el que más pesa en un desarrollador. Cada mes de atraso empuja los flujos y suma *carry* financiero sobre el capital empleado.
- Ilustrativo: capital empleado ~$4.000M–$6.000M a un costo de capital ~18%–24%/año → *carry* ≈ **$60M–$120M/mes** ≈ **$14M–$28M COP/semana**, **antes** del efecto sobre la TIR.
- La caída **27% → 18%** ya materializó el impacto: cada mes adicional erosiona más puntos de TIR, cuyo valor en NPV suele **superar** el costo de prolongación operativo.

### Punchline para el CFO
| | Por semana (ilustrativo) |
|---|---|
| Prolongación operativa (Lente A) | **$12M–$32M COP** |
| Carry financiero (Lente B) | **$14M–$28M COP** + erosión de TIR |
| **Tarifa Field** | **$4.9M COP/mes** ($59M / 12) |

→ Por **cualquiera** de los dos lentes, **una sola semana** de atraso evitada supera con holgura **el costo mensual** de Field. Field = **0.7%** del costo directo. **Esto es lo que respalda "se pagó solo".**

### Plantilla en blanco (para llenar con el cliente)
```
Costo directo mensual ....................... $________
Indirectos de obra (% del directo) .......... ____%  → $________/mes
Nómina fija + administración ................ $________/mes
Vigilancia + cerramiento + servicios ........ $________/mes
Equipos/andamios (arriendo o deprec.) ....... $________/mes
Overhead oficina imputable .................. $________/mes
--------------------------------------------------------
(A) Prolongación semanal base = suma/4.33 ... $________/sem
(B) Factor de riesgo (+15–40%) .............. $________/sem
(C) Carry financiero semanal ................ $________/sem
(D) Rework atribuible (envelope 3–7%) ....... $________ (contingencia)
========================================================
Costo defendible de 1 semana de atraso ≈ (A×B)+(C)  $________/sem
Comparar contra tarifa Field: $4.9M/mes
```

---

## 5. Qué NO afirmar (para no perder credibilidad)
No está bien respaldado empíricamente decir, para un residencial boutique en Colombia:
- ❌ "Una semana de atraso cuesta **exactamente X%** del contrato."
- ❌ "El tiempo promedio de detección de desvíos es **Y días** (estándar regional)."
- ❌ "BIM 4D / dron reduce el atraso en **Z%**" de forma generalizable.

Sí es defendible: los atrasos/sobrecostos son sistemáticos; el rework consume varios puntos del contrato; y el monitoreo **reduce la probabilidad de detección tardía y mejora la coordinación** —aunque la magnitud exacta depende del caso y no está estandarizada.[^uav][^cv1][^cv2]

---

## Fuentes principales
[^bid]: BID — *Increasing the Efficiency of Public Infrastructure Delivery* (LAC). https://publications.iadb.org/publications/english/document/Increasing_the_Efficiency_of_Public_Infrastructure_Delivery_Evidence-based_Potential_Efficiency_Gains_in_Public_Infrastructure_Spending_in_Latin_America_and_the_Caribbean.pdf
[^cii]: CII / ASCE — *Measuring the Impact of Rework on Construction Cost Performance* (359 proyectos, ~5% directo). https://ascelibrary.org/doi/10.1061/(ASCE)0733-9364(2009)135:3(187)
[^love]: Love & Edwards — *Calculating total rework costs in Australian construction* (6.4% directo + 5.9% indirecto). https://ro.ecu.edu.au/ecuworks/2401/
[^giri]: Get It Right Initiative — *Literature Review* (rango 3–15%; causas por mala información). https://getitright.uk.com/live/files/reports/4-giri-literature-review-revision-3-599.pdf
[^capital]: *Capital Electric Co. v. United States* — lógica de la fórmula Eichleay. https://law.justia.com/cases/federal/appellate-courts/F2/729/743/313383/
[^eichleay]: *The Eichleay Trilemma* — U. Chicago Business Law Review. https://businesslawreview.uchicago.edu/online-archive/eichleay-trilemma
[^radman]: Radman — *Delay management with real-time data* (sistemas reactivos; sin benchmark universal de latencia). https://mro.massey.ac.nz/server/api/core/bitstreams/ef9f091c-6d48-4da6-b6d7-63c6e6750741/content
[^uav]: *UAVs for Physical Progress Monitoring of Construction* (Chile, residencial, BIM 4D). https://pubmed.ncbi.nlm.nih.gov/34203045/
[^cv1]: *A Review of Computer Vision-Based Techniques for Construction Progress Monitoring* (ISARC 2023). https://www.iaarc.org/publications/2023_proceedings_of_the_40th_isarc_chennai_india/a_review_of_computer_vision_based_techniques_for_construction_progress_monitoring.html
[^cv2]: *Automated Computer Vision-Based Construction Progress Monitoring* (Heriot-Watt). https://researchportal.hw.ac.uk/en/publications/automated-computer-vision-based-construction-progress-monitoring-/
[^cost-overrun-review]: *Systematic Review of Cost Overrun Research (developed & developing)*. https://publisher.uthm.edu.my/ojs/index.php/IJSCET/article/download/7456/4247

> Nota: las cifras en COP/USD de §4 son **ilustrativas** (heurísticas de literatura + tasa ~$4.000/USD) y deben recalcularse con los inputs reales de §3 antes de mostrarlas al cliente.
