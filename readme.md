# Análisis S&P500

En el archivo "SP500_analisis.ipynb" se presenta un análisis del indice en el periodo 2000-2021 donde se pretende dar respuesta a las siguientes preguntas:

### Cual fue el mejor día para invertir teniendo en cuenta el retorno de los movimiento gap?

![gaps](https://github.com/facundoallia/analisisSP500/raw/main/asset/days.png)



Según el analisis realizado, si bien las diferencias no son significativas, el mejor día para invertir solo teniendo en cuenta los rendimientos gap es el martes, con un retorno promedio en el periodo bajo estudio de 0.06%. Por otro lado, el peor dia para realizar esta estrategia es el viernes, con un retorno promedio en el periodo bajo estudio de un -0.01%.

Si bien la estrategia "buy the close, sell the open" parece funcionar en la teoría, se deben tener en cuenta varios factores que merman drasticamente sus resultados:

![strategy](https://github.com/facundoallia/analisisSP500/raw/main/asset/strategy.png)

+ Deslizamiento o Slippage: Hace referencia a la diferencia entre el precio al que se ordena una operación y el precio al que se ejecuta finalmente. Es poco probable operar al mejor precio en la apertura, principalmente cuando se producen eventos de volatilidad o se operan activos poco liquidos.

+ Costo operativo: La estrategia sobreopera llevando a incurrir en costos operativos elevados. Si se tiene en consideración una comisión de 0.01% la estrategia deja de ser rentable, por lo que se recomendaría un contratar un servicio con esquema de comisiones flat fee en caso de implementarla.

+ Por ultimo la estrategia no tiene en cuenta métricas de exposición al riesgo: Operar acciones individuales mediante esta estrategia podría exponernos a un riesgo muy elevado, principalmente en las ruedas previas a la presentación de resultados o eventos significativos para la empresa en cuestión. Aplicar la estrategia en índices o carteras bien diversificadas (con correlación baja entre sus activos) reduciria notablemente la exposición al riesgo no sistemático.

### Cual fue el mejor día para invertir teniendo en cuenta el retorno de los movimientos intradiarios?

![intra](https://github.com/facundoallia/analisisSP500/raw/main/asset/days_intra.jpg)



Las mismas consideraciones que fueron presentadas para la estrategia "buy the close, sell the open" deben ser tenidas en cuenta para la segunda estrategia

### Cuales fueron las 9 mejores empresas para invertir?

Obtenemos así las 9 mejores empresas para haber invertido en el periodo bajo estudio. Si hubieramos invertido en Monster al inicio del periodo hubieramos multiplicado nuestra inversión por mas de 1000

![top](https://github.com/facundoallia/analisisSP500/raw/main/asset/top_stocks.png)


### Cuales fueron las mejores industrias que pertenecen al SP500 en las cuales se puede invertir?

Para responder esta pregunta agruparemos las acciones del S&P500 en los 11 sectores en los que se divide y compararemos sus retornos acumulados en el período analizado:

![sectors](https://github.com/facundoallia/analisisSP500/raw/main/asset/sectors.png)

El sector que presento mejores resultados en el período analizado es "Consumer Staples" seguido por "Consumer Discretionary" y "Communication Services". Por otro lado los sectores que menos rentabilidad ofrecieron fueron "Financials", "Utilities" y "Energy"

### Cuales fueron los momentos de alta volatilidad que afectaron al SP500?

Para determinar los momentode de alta volatilidad que afectaron al S&P500 podemos utilizar el índice VIX. El índice de volatilidad VIX es un indicador que muestra la volatilidad esperada a corto plazo en los mercados financieros de Estados Unidos. Se construye con una cartera ponderada de opciones call y opciones put sobre el índice americano S&P 500 (SPX).

![vix](https://github.com/facundoallia/analisisSP500/raw/main/asset/vix.png)

Podemos deducir los cambios de régimen de volatilidad estableciendo como valor significativo de 40 puntos. El valor que toma el VIX es la volatilidad que esperan experimentar los inversores para el índice SPX en un período de 30 días. Por lo tanto, cuando el VIX toma valores superiores a 40 puntos, el mercado espera que el índice S&P500 tenga una volatilidad de al menos 40% en los proximos 30 dias. Esta situación se da en 7 momentos en el período analizado:

 + Septiembre 2001: Atentado 9/11 

 + Julio 2002: Piso de la caída de la crisis punto com
 
 + 2008-2009: Gran crisis de deuda subprime

 + Mayo 2010: Resago de la crisis subprime

 + Agosto 2011: Crisis eurozona

 + Agosto 2015: Suba de tipos de interes
 
 + Febrero 2020: Crisis Covid-19


