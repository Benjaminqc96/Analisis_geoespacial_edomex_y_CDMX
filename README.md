# Análisis geoespacial del comercio de abarrotes en México

El comercio de abarrotes al por menor es una actividad económica importante, ya que de acuerdo al INEGI, representa el 12.8% del total de ingresos de comercio al por menor. De ese 12.8% de ingresos, el 82.3% se realizaron de manera física en un establecimiento.

El presenter análisis pretende explicar la dinámica del comercio al por menor comparando las tiendas de abarrotes y las tiendas de conveniencia, poniendo como principal motivo las desventajas competitivas que tienen las tiendas de abarrotes contra las cadenas de conveniencia, tales como los diversos métodos de pago alternos al efectivo (vales de despensa, tarjeta de crédito, tarjeta de débito), el pago de servicios, los horarios extendidos entre otros.

Los datos empleados provienen de dos fuentes, la fuente para las tiendas de abarrotes es el Directorio de Unidades Económicas del INEGI (DENUE), mientras que para las tiendas de conveniencia es la base de tiendas OXXO autorizadas para realizar pagos para la banca Afirme, disponible en la siguiente liga: https://www.afirme.com/dam/jcr:28a5a601-e270-487b-bc04-7e8fbc0feff5/SUCURSALES%20OXXO%202022.pdf.
Para el caso del DENUE contiene la latitud, longitud, dirección, número de empleados, cógigo postal, nombre del establecimiento entre otros, por otra parte la base de datos de Afirme contiene latitud, longitud, código postal, dirección y variables internas de la cadena. La base del DENUE está actualizada al año 2021 y la base que comparte banca Afirme al mes de abril de 2023.

Inicialmente se hace un conteo por AGEE para así gráficar por entidad la cantidad de tiendas de abarrotes y de OXXO's que se ubican en cada estado de la república, teniendo como resultado los siguietes gráficos:


<div align="center">
Distribución por estado de la cadena comercial OXXO  
</div>


  
![](https://github.com/Benjaminqc96/Analisis-geoespacial-del-comercio-de-abarrotes-en-M-xico/blob/main/cont_oxxo_tot.png)



<div align="center">
Distribución por estado de las tiendas de abarrotes
</div>

![](https://github.com/Benjaminqc96/Analisis-geoespacial-del-comercio-de-abarrotes-en-M-xico/blob/main/cont_aba_tot.png)



De los gráficos anteriores contrastan los estados de Nuevo León, Estado de México, Ciudad de México y Oaxaca. Nuevo León es el estado donde más registros hay de tiendas OXXO, con 1,816 sucursales y 15,910 tiendas de abarrotes; el Estado y la Ciudad de México resaltan porque contienen una alta densidad de tiendas de conveniencia y de abarrotes, en la Ciudad de México hay 11389 sucursales de OXXO y 38,001 tiendas de abarrotes, mientras que el Estado de Mèxico hay 1,582 sucursales de OXXO y 88,615 tiendas de abarrotes; el estado de Oaxaca hay 206 sucursales de OXXO y 31,333 tiendas de abarrotes.

De los tres casos expuestos con anterioridad resalta el del Estado y la Ciudad de México, son las entidades con mayor número de habitantes, con 16.9 y 9.2 millones de habitantes respectivamente, por lo que el enfoque será para estas dos entidades.

<div align="center">
Distribución de tiendas OXXO en la Ciudad y el Estado de México
</div>

![](https://github.com/Benjaminqc96/Analisis-geoespacial-del-comercio-de-abarrotes-en-M-xico/blob/main/cont_oxxo.png)




<div align="center">
Distribución de tiendas de abarrotes en la Ciudad y el Estado de México
</div>

![](https://github.com/Benjaminqc96/Analisis-geoespacial-del-comercio-de-abarrotes-en-M-xico/blob/main/cont_aba.png)


Ya con los conteos por AGEM, se procede a hacer un análisis puntual de aquellas en las que se encuentra la mayor concentración de tiendas OXXO, así como las que contienen mayor concentración de tiendas de abarrotes. Empleando la distancia de Haversine se estima la cantidad de tiendas de abarrotes que hay en un radio de 350 metros alrededor y asì estimar una densidad promedio


El primer caso es el de la delegación Cuauhtémoc en la Ciudad de México, en la cuál hay 244 sucursales de tiendas OXXO y 1,825 tiendas de abarrotes. Con la metodología y los parámetros expuestos la densidad estimada es de 18.2 tiendas por cada OXXO 

<div align="center">
Gráfico de dispersión de la alcaldía Cuauhtémoc 
</div>


![](https://github.com/Benjaminqc96/Analisis-geoespacial-del-comercio-de-abarrotes-en-M-xico/blob/main/9.15.png)


Con la metodología ya aplicada se puede apreciar que hay partes donde la densidad de los OXXO's es menor, de las cuales destacan las colonias Tlatelolco, Tepito y Peralvillo, mientras que donde se observa mayor densidad se encuentran colonias como la Condesa, Roma e Hipódromo.


<div align="center">
Gráfico de dispersión restringido de la alcaldía Cuauhtémoc 
</div>

![](https://github.com/Benjaminqc96/Analisis-geoespacial-del-comercio-de-abarrotes-en-M-xico/blob/main/9.15.r.png)


Con la restricción del radio de 350 metros alrededor de la tiendas OXXO algunos puntos se excluyen del gŕafico.


El segundo caso que se expone es el del municipio de Toluca, en el cual se encuentran 180 sucursales de OXXO, y 5,508 tiendas de abarrotes. La densidad estimada es de 14.6 tiendas de abarrotes por cada OXXO.

<div align="center">
Gráfico de dispersión restringido del municipio de Toluca
</div>

![](https://github.com/Benjaminqc96/Analisis-geoespacial-del-comercio-de-abarrotes-en-M-xico/blob/main/15.106.r.png)


Únicamente se muestra el gráfico restringido con fines de visualización, ya que de lo contrario no es posible apreciar debido a la aglomeración de puntos en el mapa.

El tercer caso es el de la alcaldía Benito Juárez en la Ciudad de México, en la cuál se encuentran 168 sucursales de OXXO y 680 tiendas de abarrotes, con una densidad estimada de 10.3 tiendas de abarrotes por cada OXXO.


<div align="center">
Gráfico de dispersión restringido de la alcaldía Benito Juárez
</div>

![](https://github.com/Benjaminqc96/Analisis-geoespacial-del-comercio-de-abarrotes-en-M-xico/blob/main/9.14.png)


Un par de casos que resaltan bastante es el de los municipios de Ecatepec y Nezahualcoyotl, los cuales se encuentran en la zona conurbada de la ciudad de México. Para el caso de Ecatepec, se encuentran 92 OXXO's y 9,616 tiendas de abarrotes, con una densidad estimada de 22.8 tiendas de abarrotes por cada OXXO.


<div align="center">
Gráfico de dispersión del municipio de Ecatepec
</div>

![](https://github.com/Benjaminqc96/Analisis-geoespacial-del-comercio-de-abarrotes-en-M-xico/blob/main/15.33.png)


las partes despobladas del municipio corresponden al parque ecológico Ehecatl, ubicado al poniente y a la ciénega de de san Juan, ubicada al oriente   

Para el caso de Nezahualcoyotl. en él se encuentran 54 OXXO's y 5628 tiendas de abarrotes, con una densidad estimada de 37.1 tiendas de abarrotes por cada OXXO.

<div align="center">
Gráfico de dispersión del municipio de Nezahualcoyotl
</div>

![](https://github.com/Benjaminqc96/Analisis-geoespacial-del-comercio-de-abarrotes-en-M-xico/blob/main/15.58.png)

La parte deshabitada corresponde a una parte del parque ecológico del lago de Texcoco y al tramo carretero del anillo periférico.


