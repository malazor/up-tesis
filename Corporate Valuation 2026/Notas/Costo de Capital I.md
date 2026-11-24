# Costo de Capital

Es el costo de oportunida del capital.
Es el retorno esperado mas alto de todas las alternativas.

Costo economico vs costo contable
* En Economia. Lo que se deja de ganar.
* En contabilidad. Lo que se paga en una TRX.

Es **costo de capital** el es **costo de oportunidad** del capital.

**Costo de Capital** = **Costo de Opprtunidad** = **Tasa de Descuento**

Un **activo** solo genera **valor** al **accionista** cuando el **rendimiento** de este es **mayor** al **costo de capital**.

## WACC (Weighted Average Cost of Capital)
**Tasa WACC** es el **costo de capital** / **costo de oportunidad** de la firma. Es el rendimiento minimo de la empresa para no ganar ni perder. Es el promedio ponderado de los costos de las fuentes de capital de la empresa (equity y deuda) respecto al enterprise value.

Fórmula del WACC
$$\text{WACC} = \left( \frac{E}{V} \times K_e \right) + \left( \frac{D}{V} \times K_d \times (1 - T) \right)$$
$E$: Valor de mercado del patrimonio (Equity).  
$D$: Valor de mercado de la deuda neta (Debt).  
$$\text{Deuda Neta} = \text{Deuda Financiera Total} - \text{Caja y Equivalentes de Efectivo} - \text{Otros Activos no operativos}$$
$V$: Valor total del capital de la empresa ($E + D$).  
$K_e$: Costo del patrimonio (lo que exigen los accionistas, calculado usualmente con el modelo CAPM).  
$K_d$: Costo de la deuda antes de impuestos (tasa de interés promedio que paga la empresa).  
$T$: Tasa de impuesto corporativo (se multiplica por $(1 - T)$ porque los intereses de la deuda son deducibles de impuestos, generando un escudo fiscal). Se realiza este ajuste para caluclar la deuda que asume la empresa despues de aplicar el escudo fiscal.  

Valor de la empresa = Valor Mercado Equity + Valor Deuda Neta
$$\text{EV} = \text{E} + \text{D}$$

Deuda neta, se le quita el cash porque el cash no genera flujos.

# Modelo CAPM

Mide cual es el rendimiento minimo que cubre el riesgo de incorporar un activo adicional al portafolio diversidifcado. Es decir cuanta rentabilidad minima debo exigir a este nuevo activo en mi portafolio. Dado que añadir esa acción le aporta un riesgo adicional no eliminable a su portafolio, el inversionista exige una recompensa económica.

Como el mercado se considera un portafolio eficiente, dado que no se puide diversificar más.

**Portafolio eficiente:** Es aquel que logra eliminar por completo el riesgo diversificable, manteniendo solamente la exposision al riesgo sistemático que no es mitiga diversificando.

$$K_e = R_f + \beta \times (R_m - R_f)$$

Donde:
* $K_e$: Costo del patrimonio o retorno esperado del activo.    
* $R_f$: Tasa libre de riesgo (Risk-Free Rate). Rendimiento de un instrumento sin riesgo de impago, como los bonos del Tesoro de EE. UU. a 10 años.
* $\beta$ (Beta): Medida de la volatilidad o sensibilidad del activo frente al mercado general. Si $\beta = 1$, se mueve igual que el mercado; si $\beta > 1$, es más volátil y riesgoso.
* $R_m$: Retorno esperado del mercado (por ejemplo, el rendimiento histórico promedio del índice S&P 500).
* $(R_m - R_f)$: Prima de riesgo de mercado (Equity Risk Premium o ERP). Es el rendimiento adicional que exigen los inversionistas por asumir el riesgo de invertir en acciones en lugar de un activo libre de riesgo.

## Estimacion del modelo CAPM

### Tasa Libre de Riesgo
Riesgo es la incertidumbre sobe el rendimiento.
Un **activo libre de riesgo** es aquel que su rendimiento esta garantizado sea cual fuese. El rendimiento realizado es igual al rendimiento esperado. $$\sigma = 0$$  
Debe cumplir las siguientes condiciones:
* No debe tener riesgo de default.
* No debe tener riesgo de reinversión.

Se recomienda utilizar el **T-Bond** dado que es mas liquido y es a largo plazo. Su rendimiento depende de las espectativas nominales de crecimiento de la economía de EEUU a largo plazo.



$$r_f = (1 + \text{Crecimiento esperado del PBI a LP}) (1 + \text{Inlación esperada en LP}) - 1$$

Debe registrarse la tasa libre de riesgo al momento de realizar la valoración. Recoge las espectativas actuales de crecimiento de la economía a largo plazo (LP).

La moneda de la tasa libre de riesgo debe coincidir con la moneda de los flujos de caja.

### La prima de riesgo

* Metodo Implicito. Sacarle la TIR al SP500.


La **prima de riesgo** es la compensación adicional a la **tasa libre de riesgo** que el inversionista obtiene al inverrtir een el portafolio del mercado.
$$\text{Prima de riesgo de mercado} = E[R_\text{mkt}] - rf$$
La prima de riesgo se puede obtener por el metodo implicito e histórico.

#### Método Implícito
Es un enfoque prospectivo del rendimiento adicional que exigen los inversionistas a partir de los precios actuales del mercado.

* Igualación al precio actual: Se toma la cotización de mercado actual del índice S&P 500 como el valor presente del portafolio.
* Proyección de flujos de efectivo: Se estiman los retornos en efectivo esperados (Cash returns) para los inversionistas, calculados como la suma de los págos de dividendos y recompras de acciones de todas las empresas del índice durante el periodo explícito de proyección (habitualmente 5 años) más un valor terminal con una tasa de crecimiento de largo plazo.
* Despeje de la tasa del mercado: Se resuelve la ecuación de valor presente para despejar la tasa de retorno esperada del mercado, $E(r_{S\&P500})$, la cual iguala el valor presente de los flujos futuros con el nivel del índice.
* Cálculo de la prima implícita: A ese rendimiento esperado del mercado se le resta la tasa libre de riesgo ($R_f$) del T-Bond a 10 años23: 

$$\text{Nivel Actual del S\&P 500} = \sum_{t=1}^{n} \frac{E(\text{Cash Return}_t)}{(1 + E(r_{\text{S\&P500}}))^t} + \frac{E(\text{Cash Return}_{n+1})}{\left(E(r_{\text{S\&P500}}) - g_{LP}\right) \cdot (1 + E(r_{\text{S\&P500}}))^n}$$

**Donde:**
* **$\text{Nivel Actual del S\&P 500}$**: Cotización observada del índice en la fecha de corte.
* **$E(\text{Cash Return}_t)$**: Flujos de efectivo esperados para los accionistas del índice, calculados como la suma de **dividendos esperados + recompras de acciones (*buybacks*)**.
* **$g_{LP}$**: Tasa de crecimiento esperada de los flujos de caja en el largo plazo.
* **$E(r_{\text{S\&P500}})$**: Rendimiento esperado del mercado (variable a despejar).

**Cálculo de la Prima por Riesgo Implícita**
Una vez hallada la tasa interna de retorno del mercado $E(r_{\text{S\&P500}})$, se le resta la tasa libre de riesgo ($R_f$) correspondiente al T-Bond a 10 años:

$$
\text{Prima implícita por riesgo} = E(r_\text{S\$P500}) - R_f
$$

#### Método Histórico
Se calcula como la **diferencia** entre el **rendimiento histórico** de un **índice de mercado** y el rendimiento del **bono del gobierno**.

La prima historica depende de los siguiente factores:
* Variable que representa el mercado S&P 500. El S&P 500 se toma como referencia dado que es un portafolio ponderado de las **500 acciones más grandes de EEUU**. Asimismo representa mas de 70% del mercado de valores de EEUU.
* Variable que representa la tasa libre de riesgo T-Bond o T-Bill.
* Periodo de tiempo a incluir. Los periodos cortos tienen un **error estándar** mas alto que los periodos largos. Los periodos cortos estan sesgados por ciclos economicos.
* Tipo promedio aritmetico o geométrico. Es mejor utilizar el promedio geométrico dado el **efecto de capitalizacion**, reflega mejor el **crecimiento anual (CAGR)** y tienen **menor error estandar**.

**¿Cuál es mejor?**
Ninguna es mejor que la otra, solo depende del **supuesto de la valoración**.
* Implítica, que la valoración debe ser neutral al mercado.
* Histórica, que revertirá el promediod e largo plazo.


## Beta $(\beta)$
Es la sensibilidad del rendimiento de un activo respecto al rendimiento del mercado. Es decir, cuánto **cambia** el **rendimiento de la empresa** respecto al **rendimiento del mercado**.  
* Si $\beta$, es < que 1 entonces la empresa tiene menos riesgo sistemático respecto al mercado.
* Si $\beta$, es > que 1 entonces la empresa tiene más riesgo sistemático respecto al mercado.
* Si $\beta$, es = que 1 entonces la empresa tiene el mismo riesgo sistemático del mercado.

Mide 2 tipos de **riesgos**. Riesgo de **negocio** y **apalancamiento**.

### Betas regresión.
Para estimarla se estiman la realcion entre los rendimientos en exceso de la **accion** y el **mercado**. El resultado depende de la elección del índice que representa el mercado ($S\&P500$), periodo y frecuencia de los datos.

Los betas de regresión presentan **problems** dado que el **error estandar** es sustancial, representan el negocio y apalancamiento promedio del pasado, puede que estos hayan cambiado.

Es recomendable utilizar betas de regresión cuando la empresa esta **listada** y cuenta con **datos historicos**, el negocio y el apalancamiento haya sido **constante** y se proyecte no cambie drásticamnte en el futuro, el **error estandar** de la regresión sea **bajo** o aceptable y **falta de muestras comparables** ue impidan hacer un bottom up.

### Betas Bottom up.





Empresas pequeñas o jovenes, empresas ciclicas tienen mas riesgo.

Volatilidad del activo respecto a la volatilidad del mercado.

Betas mas alto para empresas mas apalancamiento.

se estiman en base a regresion y bottom up.

Escudo Fiscal y tasa participacion de los trabajadores. Diapositiva 92y 93.

Unlevered beta corrected for cash
El cash de la empresa no tine risgo. 94.


## Costo de Capital de la Deuda



