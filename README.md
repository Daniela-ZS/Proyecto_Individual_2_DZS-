# Proyecto_Individual_2_DZS-
PIDA

# **Proyecto individual 2: "Mercado Bursátil" (Data Analyst)**

![StreamPLUS]() ![S&P_500]()

## **Por Daniela Zarich Santi**

Como jefa del departamento de Analytics de StreamPLUS y respondiendo a la solicitud del Equipo Directivo de identificar cuál es la mejor opción para ampliar los horizontes de inversión ingresando al Standard & Poor´s 500 (S&P 500), presento el análisis realizado por el departamento que represento.

## Análisis Exploratorio de los datos(EDA)

Si bien el objetivo general de la propuesta es *ampliar los horizontes de inversión y decidir en qué empresa del S&P 500 conviene invertir*, como objetivos específicos (guía), plantemos los siguientes:

* Analizar el histórico financiero de las empresas del sector escogido, a partir del año 2000.
* Analizar la situación actual de las empresas seleccionadas, incluyendo su rendimiento financiero.
* Realizar una comparación entre las empresas seleccionadas, atendiendo los precios de apertura, cierre y cierre ajustado diarios para extraer conclusiones sobre la posición en el mercado financiero.
* Proporcionar recomendaciones sobre en qué empresa invertir, y a qué plazo.

Cabe aclarar que esos objetivos fueron la guía para realizar el análisis en cuestión, pero no fueron respondidos uno a uno.

Una vez comprendida la petición de la empresa y planteados los objetivos, realizamos el EDA correspondiente al análisis en cuestión. 

_____
*Los datos fueron extraídos de Yahoo Finance y Wikipedia. También consultamos otras páginas web como ser Google Finance, S&P 500, entre otras.*

*Los enlaces a continuación:*

* https://finance.yahoo.com/
* https://en.wikipedia.org/wiki/List_of_S%26P_500_companies
* https://www.google.com/finance/?hl=es
* https://www.spglobal.com/spdji/es/indices/equity/sp-500/#overview
_____

Para comenzar, investigamos cuáles son las empresas que forman parte del S&P 500 y en qué sectores se desempeñan, para buscar una categoría acorde a la nuestra (StreamPLUS). Como nosotros nos desempeñamos en el ámbito del streaming, la búsqueda fue orientada por ese lado, sector 'Movies & Entertainment'. Encontramos que hay cinco empresas diferentes en el sector, pero descartamos una, Live, porque está orientada a la ópera y venta de boletos en vivo para espectáculos, por lo que el estudio se realizó sobre las cuatro restantes: Disney, Fox, Netflix y Paramount (los códigos dentro del gigante financiero son DIS, FOX, NFLX y PARA, respectivamente).

![DIS]() ![FOX]() ![NFLX]() ![PARA]()

Luego realizamos reportes de cada una de las empresas mencionadas para extraer conclusiones.

El reporte completo se encuentra en el archivo 'EDA.ipynb'.


## Dashboard

El dashboard que presento es interactivo, realizado en PowerBI, cuenta con ocho pestañas en las cuales se puede observar:

* Evolución de precio de apertura, cierre y cierre ajustado 
* Evolucion de porcentaje de variación de precios apertura/cierre y apertura/cierre ajustado (comparativo)
* Volumen de inversiones
* Volumen de inversiones por empresa (porcentaje)
* Volumen de inversiones por año (porcentaje de cada empresa)
* Valor de las transacciones diarias (comparativo con respecto a precio de cierre y precio de cierre ajustado)
* Valor de las inversiones por año (porcentaje de cada empresa)
* Promedio diario de *volumen* de transacciones y promedio diario de *valor* de tansacciones (por empresa)

En varios tableros se puede filtrar por empresa (DIS, FOX, NFLX, PARA) y por ventana de tiempo, mientras que otros son estáticos, ya que presentan porcentajes anuales y valores promedio diarios,  para cada empresa.

A continuación se presentan ejemplos de la portada y los tableros:

![Portada]()

![Tablero1]()

![Tablero2]()

![Tablero3]()

![Tablero4]()

![Tablero5]()

![Tablero6]()

![Tablero7]()

![Tablero8]()


## KPIs

En el proceso del análisis para encontrar en qué empresa del S&P 500 conviene invertir y ampliar los horizontes de StreamPLUS surgieron varias métricas, como por ejemplo:

* Porcentaje de variación de cierre ('% var cierre') y de cierre ajustado ('% var ajustado'). Indican cuánto ha variado el precio de apertura y de cierre/cierre ajustado, diariamente, en porcentaje.
* Valor de las transacciones, teniendo en cuenta el precio diario de cierre y de cierre ajustado. Este valor indica el flujo económico de la empresa. Estas métricas fueron calculadas diariamente. 
* Resumen anual del valor de las inversiones, en el que se puede observar que hay una variación mínima entre el valor considerando el precio de cierre y el valor considerando el precio de cierre ajustado, ya que se realiza el promedio anual del mismo.

Atendiendo a esas métricas calculadas podemos plantear KPIs acordes a los objetivos planteados con anterioridad:

* Sostener el promedio de variación de cierre ajustado con valores positivos durante el próximo trimestre.
* Aumentar el valor de las inversiones un ...% el próximo semestre.
* Alcanzar un promedio de inversiones de ... el próximo año.

Estos KPIs medirán si la inversión fue positiva o no, en el plazo máximo de un año.


## Análisis

Como conclusiones del análisis podemos obtener:

### Disney
* Presenta una oscilación en los precios de apertura, cierre y cierre ajustado, pero la tendencia está creciendo.
* Considerando porcentaje de variación entre cierre y cierre ajustado, no hay variación entre los mismos.
* El porcentaje de volumen de inversiones por año muestra que, si bien aumentó en los últimos años tiende a estabilizarse.
* El porcentaje de valor de inversiones ocupa el segundo lugar, prácticamente estable en el tiempo.

### Fox
* Ocurre un escenario similar al de Disney, mostrando también tendencia a aumentar en el tiempo.
* Los porcentajes de variación entre los precios de cierre y cierre ajustado variarion en el tiempo, pero la tendencia es a equipararse en los últimos días.
* El porcentaje de volumen de transacciones por año es equivalente en el transcurso del tiempo.
* El porcentaje de valor de inversiones de Fox es casi imperceptible comparado con las otras empresas.

### Netflix
* Considerando los precios de apertura, cierre y cierre ajustado, en general la tendecia va en suba, con un pico en noviembre de 2021. Hubo una baja hasta mayo de 2022, pero la tendecia sigue siendo positiva.
* No hay variación entre variación de precios de cierre y cierre ajustado.
* Si bien el porcentaje de volumen de transacciones por año fue liderado por esta empresa, actualmente es equitativo con otras.
* El porcentaje de valor de inversiones lidera la lista, como en los últomos 10 años.

### Paramount
* Si bien los precios de apertura, cierre y cierre ajustado variaron notablemente en el período de tiempo analizado, en las cuatro empresas se presenta un comportamiento similar: en marzo de 2020 comenzó una suba que tuvo un pico en marzo 2021 y luego bajó abruptamente durante un mes, para luego tener variaciones mínimas. Eso se debe claramente a la irrupción de la pandemia, el aumento de suscripciones fue porque las personas debieron quedarse en sus hogares por el aislamiento, el marzo de 2021 se "normalizó" la situación y por eso el decaimiento mencionado. 
* Considerando los últimos días, la tendencia muestra un aumento en el valor de los precios de apertura, cierre y cierre ajustado, en las cuatro compañías.
* El porcentaje de volumen de transacciones por año ha aumentado en los últimos años.
* El porcentaje de valor de inversiones de esta empresa es muy bajo comparada con las otras.

______
*Por lo que no es posible determinar una única empresa para inveritir, sino que deberían reevaluarse los objetivos y, teniendo en cuenta los ítems mencionados en el párrafo anterior, seleccionar cuál es la mejor opción.*
_______

## Repositorio de GitHub

El repositorio de GitHub que contiene el análisis completo es:

https://github.com/Daniela-ZS/Proyecto_Individual_2_DZS-.git 

Contiene:

* README ---> este archivo que estás leyendo
* SyP500_ZS.ipynb ---> notebook con el trabajo sobre S&P 500
* Trab_pataformas_ZS.ipynb ---> notebook con el trabajo sobre las plataformas
* EDA_ZS.ipynb ---> notebook con el EDA y los reportes de cada empresa
* PIDA_ZarichSanti.pbix ---> archivo PowerBI con las visualizaciones
* Imágenes ---> Carpeta con imágenes incluidas en el Readme
