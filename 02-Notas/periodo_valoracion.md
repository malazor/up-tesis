# Periodo Valoracion

Existen 3 escenarios:
1. Valorar hasta diciembre del 2025. Datos reales hastsa 31 dic 2025. Año 2026 es el primer año del periodo extraordinario. Proyectar 2026 con lo real hasta q3 + lo estimado / proyectado de q4.
2. Valorar hasta q3 2026 utilizando TTM. Datos reales hastsa 31 dic 2025. El año 2026 se completa haciendo un TTM hasta q3 2026.

> **Fecha de valoración y tratamiento de 2026**
>
> La valoración se realiza con fecha de corte al **31 de diciembre de 2025**, último cierre anual del que se dispone de estados financieros auditados. Este es el año base (año 0) del modelo DCF.
>
> Aunque el trabajo se elabora con información posterior, hasta el tercer trimestre de 2026 (Q3 2026), no es posible contar con el año 2026 completo. Por ello, **2026 se proyecta como el primer año del periodo explícito (2026–2030)** y se construye con dos componentes:
>
> - **Componente real:** los resultados efectivamente observados de enero a setiembre de 2026 (Q1–Q3).
> - **Componente estimado:** una proyección propia del cuarto trimestre de 2026 (Q4), basada en los supuestos macroeconómicos y operativos del modelo.
>
> Los flujos de caja proyectados se descuentan a la fecha de valoración (31/12/2025), de modo que el valor resultante corresponde a esa fecha. Dado el propósito académico del trabajo y el momento en que se realiza, incorporar los datos reales disponibles de 2026 hace que la proyección del primer año sea más precisa que una estimación puramente teórica.

### Opción 1: Valoración a Diciembre de 2026 (31 de diciembre de 2026)

Esta opción proyecta el cierre completo del ejercicio 2026 como periodo base ($t_0$) o como primer año completo de proyección.

PROS:

* Ciclo anual completo: Captura el año operativo íntegro, incorporando el impacto decisivo de la campaña navideña y de fin de año.
* Normalización del Balance y Capital de Trabajo: La foto del balance a cierre de diciembre muestra niveles de inventario y cuentas por pagar post-campaña, permitiendo una comparación directa y limpia con los cierres anuales históricos (2024, 2025).
* Simplicidad metodológica en el Flujo de Caja Descontado (DCF): Permite estructurar periodos anuales homogéneos de proyección ($t_1 = 2027, t_2 = 2028, \dots$), evitando fraccionar el primer año en meses parciales para la tasa de descuento (WACC).

CONTRAS:

* Dependencia de proyecciones para el Q4: Exige estimar el desempeño comercial de los dos meses restantes del año en un contexto expuesto a factores de riesgo estacional (como las alertas climáticas de El Niño hacia el verano 2026-2027).
* Fecha base futura respecto a hoy: Valuar al 31/12/2026 implica fijar la fecha de corte dos meses por delante de la fecha actual (31/10/2026), por lo que se requiere descontar nuevamente ese valor si se busca la cifra exacta al día de hoy.

### Opción 2: Valoración a Diciembre de 2025 (31 de diciembre de 2025)

En este escenario se fija el cierre del ejercicio fiscal 2025 como la fecha base o punto de partida ($t_0$) para la proyección de flujos de caja a partir de 2026.

PROS:

* 100% de data auditada y oficial: Se apoya en información financiera completamente verificada por auditores externos (Deloitte / Velásquez, Loli & Asociados) y en la Memoria Anual oficial1. Elimina cualquier incertidumbre sobre la validez de las cifras contables.
* Cierre anual estacionalmente completo: Al abarcar los 12 meses de 2025, incluye el impacto real de las campañas clave como el Día de la Madre, Cyber Wow y la campaña navideña del Q423. Muestra la posición real normalizada de inventarios y capital de trabajo post-fiestas.
* Base de comparación histórica limpia: Permite conectar directamente el año base con las series históricas multianuales (2015–2025)45, facilitando el cálculo de márgenes, tasas de crecimiento (CAGR) y rotaciones operativas sin necesidad de fraccionar periodos.
* Punto de corte con balance desapalancado: El cierre de 2025 marca un hito financiero claro para la empresa, al haber alcanzado una deuda financiera con terceros igual a cero67, lo que simplifica la estructura de capital inicial.

CONTRAS:

* Desfase temporal ("Lag" de 10 meses): Al estar situados a 31 de octubre de 2026, tomar como corte diciembre de 2025 implica ignorar 10 meses de desempeño operativo ejecutado del presente año, proyectando como "futuro" un periodo que en la práctica ya transcurrió.
* No captura los eventos ejecutados en 2026: Desaprovecha la información real acumulada a los primeros tres trimestres de 2026 (efecto de las elecciones presidenciales, variaciones en la inflación y alertas climáticas del ENFEN respecto a El Niño Costero)89.
* Requiere ajuste de valor presente a hoy: El valor intrínseco resultante correspondería a finales de 2025, por lo que requeriría ser capitalizado a la tasa WACC por los 10 meses transcurridos para reflejar la cifra equivalente a la fecha actual.

### Resumen Comparativo de los 3 Escenarios

| Criterio                    | **1\. Diciembre 2025**                                  | **2\. Q3 2026 (Septiembre)**                          |
| --------------------------- | ------------------------------------------------------- | ----------------------------------------------------- |
| **Naturaleza de los datos** | 100% Auditados (Memoria 2025)[1]                      | Intermedios reales (no auditados)                     |
| **Estacionalidad**          | Completa (cierre anual)[2]                            | Incompleta (falta Q4 navideño)                        |
| **Oportunidad / Frescura**  | Desfasada (hace 10 meses)                               | Muy cercana (hace 1 mes)                              |
| **Uso idóneo**              | Trabajos académicos o valoraciones históricas rigurosas | Decisiones de transacción inmediatas (con ajuste LTM) |

### Sugerencia IA
Para una tesis académica, la opción más sólida y defendible ante un jurado es fijar Diciembre de 2025 como el año base ($t_0$), combinándolo con un enfoque híbrido de calibración con la data de 2026.

¿Por qué Diciembre de 2025 es la mejor opción para la tesis?

**Rigor y auditabilidad de datos (**$t_0$ oficial): Los jurados de tesis priorizan que los estados financieros del año base sean completos, oficiales y auditados (Memoria Anual 2025 / Deloitte). Usar datos intermedios del Q3 como año base genera observaciones metodológicas porque son estados no auditados y carecen de notas explicativas detalladas.

Ventaja metodológica única (Calibración de $t_1$**):** Al estar en octubre de 2026, tienes una ventaja que fortalece la sustentación: usas 2025 como $t_0$, pero fundamentas la proyección de 2026 ($t_1$) utilizando los 9 meses de desempeño real reportados a la SMV al Q3 2026. Esto reduce la incertidumbre del primer año proyectado a solo estimar el Q4 restante.

Ciclo anual estacionalmente completo: El sector retail depende drásticamente de la campaña navideña del Q4. Fijar el año base a diciembre garantiza que las cifras de ventas, márgenes, inventarios y capital de trabajo estén completamente normalizadas, algo que un corte al Q3 deja distorsionado.

Simplicidad en el modelo DCF: Evita complicaciones metodológicas con la tasa WACC (como fraccionar tasas para periodos de 9 meses) y permite estructurar periodos anuales limpios de proyección (2026–2030 o 2026–2031).

Cómo estructurarlo en el capítulo metodológico de tu tesis

Para dejar el modelo impecable ante las observaciones de los revisores, puedes redactar el supuesto base de la siguiente manera:

"Se establece como año base de la valoración el 31 de diciembre de 2025 ($t_0$), utilizando los estados financieros consolidados auditados de la compañía. Para el periodo de proyección (2026–2030), el primer ejercicio ($t_1 = 2026$) se modela calibrando la información financiera real reportada a la SMV al tercer trimestre de 2026 (Q3) y estimando el cierre de la campaña del cuarto trimestre."