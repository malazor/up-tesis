# Supuestos de valorización – Saga Falabella S.A.

> **Fuente:** `Supuestos_Falabella_v3_1.xlsx` (hoja `Sheet1`, rango B3:E23, título en A1: *"Supuestos SAGA Falabella"*).
> Este documento resume y referencia las variables, supuestos y fundamentos del Excel, organizados en sus dos bloques: **Generales** (filas 4–18) y **Macroeconómicos** (filas 19–23).

---

## 1. Supuestos generales

### 1.1 Alcance y horizonte

#### 1.1.1 Fecha de Valoración:
**Fecha:** 31/12/2025.  
**Detalle:**   
Fecha de valoración y tratamiento de 2026

La valoración se realiza con fecha de corte al 31 de diciembre de 2025, último cierre anual del que se dispone de estados financieros auditados. Este es el año base (año 0) del modelo DCF.   
Aunque el trabajo se elabora con información posterior, hasta el tercer trimestre de 2026 (Q3 2026), no es posible contar con el año 2026 completo. Por ello, 2026 se proyecta como el primer año del periodo explícito (2026–2030) y se construye con dos componentes:
* Componente real: los resultados efectivamente observados de enero a setiembre de 2026 (Q1–Q3).
* Componente estimado: una proyección propia del cuarto trimestre de 2026 (Q4), basada en los supuestos macroeconómicos y operativos del modelo.   

Los flujos de caja proyectados se descuentan a la fecha de valoración (31/12/2025), de modo que el valor resultante corresponde a esa fecha. Dado el propósito académico del trabajo y el momento en que se realiza, incorporar los datos reales disponibles de 2026 hace que la proyección del primer año sea más precisa que una estimación puramente teórica.

---
| Variable | Supuesto | Fundamento |
|---|---|---|
| **Fecha de valorización** (C4) | 31/12/2025 | Cierre del ejercicio fiscal más reciente con estados financieros auditados y publicados por Saga Falabella ante la SMV al iniciar el trabajo. |
| **Moneda de valorización** (C5) | Sol | Moneda funcional de la empresa y con la que reporta sus estados financieros. |
| **Objeto de la valorización** (C6) | Saga Falabella S.A. Individual | Se excluye el valor patrimonial de empresas relacionadas (Banco Falabella Perú S.A., falabella.com S.A.C.); se tratan como variables estratégicas y operativas, no como activos a valorar. |
| **Horizonte de proyección** (C7) | 5 años (2026–2030) | Año base (año 0) = 31/12/2025. Cinco años se consideran suficientes para capturar la fase de mayor dinamismo antes de que el sector converja a tasas estacionarias. |
| **Año inicio de perpetuidad** (C8) | 2031 | Punto de entrada al "estado estacionario": el crecimiento converge al PBI potencial de 3.3 % (BCRP). Se asume completado el ciclo estratégico regional de metas de sostenibilidad al 2030, con eficiencias operativas maduras (energía, residuos) y Capex de mantenimiento estabilizado. |

### 1.2 Operación y financiamiento

| Variable | Supuesto | Fundamento |
|---|---|---|
| **Demanda** (C9) | Depende del consumo privado, el PBI y la capacidad adquisitiva. | (1) Correlación directa entre los ingresos de 2025 y el consumo privado, que creció 3.6 %. (2) Mayor liquidez de la población (empleo, baja inflación). (3) Acceso al crédito de consumo: según el BCRP, el crédito de consumo real vuelve a tasas positivas, con crecimiento proyectado de 9.0 % en 2026; la tarjeta CMR de Banco Falabella financia gran parte de las transacciones, lo que eleva ticket promedio y frecuencia. |
| **CAPEX** (C10) | Inversiones en repotenciar la línea de negocio E-Commerce. | Las memorias muestran inversión reciente en infraestructura logística (eficiencia de despacho), pero no en la plataforma e-commerce ni en marketing. falabella.com es operada por falabella.com S.A.C. (entidad relacionada), por lo que Saga no capitaliza software ni servidores; el acceso a esa tecnología se proyecta como **OPEX variable** ligado a ventas digitales. El modelo debe reflejar un **CAPEX de mantenimiento y modernización de la red física y logística** (recojo en tienda y última milla). |
| **DEUDA** (C11) | La empresa cumplirá sus obligaciones con empresas relacionadas. | Financiamiento de relacionadas con vencimiento hasta 2029, a una tasa implícita de "entre 7 y 75 %" (tal como figura en el Excel; ver *Observaciones*). Se proyecta estabilidad en las tasas y se asume que se prioriza la deuda con relacionadas sobre la de terceros. |
| **Dividendos** (C17) | De acuerdo al FCF. | La alta distribución de 2024 (S/ 245 MM) y 2025 (S/ 235 MM) fue posible por la solidez financiera y la baja deuda con terceros. La política del modelo debe ser consistente con la caja disponible tras el CAPEX de mantenimiento y los pagos de deuda con relacionadas. |

### 1.3 Costo de capital (CAPM) (Excel: C12:C15 combinadas)

| Componente | Valor / fundamento |
|---|---|
| **Tasa libre de riesgo** (D12) | T-Bond a 10 años: **4.38 %** a febrero 2026. |
| **Prima por riesgo de mercado** (D13) | **4.18 %** – Damodaran ERP, enero 2026. |
| **Riesgo país** (D14) | **2.07 %** – Damodaran CRP, enero 2026. |
| **Beta reapalancado** (D15) | Beta apalancada a la estructura de endeudamiento mantenida (el Excel menciona "Engie"; ver *Observaciones*). Beta desapalancada: **1.14**, corregida por caja, de Damodaran ("Beta, Unlevered beta and other risk measures"). |

### 1.4 Impuestos y valor terminal

| Variable | Supuesto | Fundamento |
|---|---|---|
| **Tasa de IR** (C16) | 29.5 % | Aplicada a todo el horizonte 2026–2030 y al valor terminal, según el régimen tributario peruano vigente. Se calcula sobre la utilidad operativa neta tras deducir el 8 % de participación de los trabajadores, consistente con la estructura histórica de costos. |
| **Crecimiento en perpetuidad** (C18) | Convergencia al PBI potencial; **g = 3.3 %** | Sustentado en la proyección de PBI potencial del BCRP (Reporte de Inflación de junio 2026). Desde 2031 se asume estado estacionario, con inflación estabilizada en 2.0 % y brecha del producto cerrada. |

---

## 2. Supuestos macroeconómicos (Excel: B19:E23)

| Variable | Supuesto | Fundamento |
|---|---|---|
| **PBI** (C19) | 3.4 % en 2026; 3.2 % en 2027 | Proyección del BCRP, alineada con la brecha del producto y las estimaciones de PBI potencial. |
| **Consumo privado** (C20) | 3.3 % anual 2026–2029 | Variable crítica para proyectar demanda y ventas; sustento: Marco Macroeconómico Multianual 2026–2029 (MEF). |
| **Inflación** (C21) | 3.8 % en 2026; 2.0 % en 2027 | Alineada con el Reporte de Inflación del BCRP; años siguientes dentro del rango meta 2 % ± 1 %. |
| **Tasa de interés de referencia** (C22) | 4.25 % | El Directorio del BCRP la mantiene desde septiembre de 2025; no se suponen cambios salvo indicios claros de recalentamiento o enfriamiento. |
| **Tipo de cambio** (C23) | S/ 3.40 por USD | Promedio proyectado en el Marco Macroeconómico Multianual 2026–2029 (MEF). |

---

## 3. Fuentes citadas en el Excel

- Estados financieros auditados de Saga Falabella S.A. (SMV) y memorias de la empresa.
- BCRP: Reporte de Inflación, tasa de referencia, PBI potencial, crédito de consumo.
- MEF: Marco Macroeconómico Multianual 2026–2029.
- Damodaran: ERP y CRP (enero 2026); *Beta, Unlevered beta and other risk measures*.
- T-Bond a 10 años (febrero 2026).

## 4. Observaciones sobre el Excel (a revisar)

Detectadas al transcribir; no se modificaron en este documento:

1. **Beta reapalancado (D15):** el texto menciona la estructura de endeudamiento de **Engie**, no de Saga Falabella; probablemente es un resto de otra plantilla.
2. **Tasa de la deuda con relacionadas (E11):** dice "entre 7 y 75 %"; el valor de 75 % parece un error de digitación (¿7 %–7.5 %?).
3. **Ortografía:** "Diviendos" (C17), "proveninte" (E11) y "platfora" (E10).
4. **Inflación de largo plazo:** E18 asume 2.0 % en la perpetuidad, mientras g = 3.3 % se apoya en el PBI potencial (¿real o nominal?). Conviene aclarar la base para que sea coherente con el flujo en soles nominales.
5. **Fecha de fuente:** E18 cita el Reporte de Inflación de junio 2026, posterior a la fecha de valorización (31/12/2025); es válido como información de mercado, pero conviene dejarlo explícito.