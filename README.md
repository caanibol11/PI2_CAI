![](https://github.com/caanibol11/PI2_CAI/blob/main/graficas/gr5.jpg?raw=true)

# PROYECTO ANALISIS DE DATOS
![](https://github.com/caanibol11/PI2_CAI/blob/main/graficas/gr6.jpg?raw=true)

**INTRODUCCION **

El Observatorio de Movilidad y Seguridad Vial (OMSV),  de la Ciudad Autónoma de Buenos Aires tiene identificado que entre los años 2018 y 2022 se registraron 19630 muertes en siniestros viales o también se puede decir que 11 personas por día fueron declaradas como víctimas fatales por accidente de tránsito.
Por lo tanto se requiere identificar información e indicadores  que permita la toma de decisiones, lograr la prevención, el aumento de la seguridad vial y disminución de siniestros viales con víctimas fatales en la Ciudad.


**ETL EXTRACCION, TRANSFORMACION Y CARGA **

Inicialmente se importan las librerias de Pandas, NumPy para trabajar dataframes los archivos originales de HECHOS y VICTIMAS. Posteriormente se realiza limpieza de datos, identificando registros nulos, duplicados y faltantes. De acuerdo a la distribución de datos en columnas se determina eliminar algunos nulos y algunas columnas que no son necesarias para el archivo final.
Se logra un archivo unificado de los dos archivos originales Hechos y Victimas con el cual se empieza la etapa de EDA.

**EDA ANALISIS EXPLORATORIO DE DATOS **

Una vez trabajado el proceso de ETL donde se logró un archivo mejorado en sus datos, se procede a analizar estos datos usando diferentes herramientas de visualización como MATPLOTLIB y SEABORN. 
Este análisis permite determinar la mejor manera de manipular la fuente de datos para obtener respuestas a los problemas planteados, como descubir patrones, detectar anomalías o poner a prueba una hipótesis. 
Con lo anterior se logra una mejor comprensión de las variables del dataset y la relación entres esas variables. 
Con este análisis se podría garantizar que los resultados proporcionados sean válidos a los obsjetivos del negocio deseado.

Para iniciar se usan primero las siguientes variables categóricas y se genera gráficos de barras y se observa su comportamiento:

variables = ['ROL', 'SEXO', 'TIPO CALLE', 'LUGAR', 'ACUSADO', 'COMUNA', 'VICTIMA']

![](https://github.com/caanibol11/PI2_CAI/blob/main/graficas/gr1.jpg?raw=true)
Grafica del Rol: en esta gráfica se observa que en la mayoría de siniestros viales, el rol de CONDUCTOR (+300) supera a los demás. Es seguido por PEATON (+250), Pasajero acompañante (+80) y de último lugar esta el ciclista  (+30). Con lo anterior se puede inferir que se debe enfocar todos los esfuerzos de educación vial al conductor del vehículo (auto o moto) ya que pueden ser varios los motivos del accidente, como, distracción, alta velocidad, perdida de control, no uso del cinturon de sguridad. en segundo lugar esta el peaton, donde aplica tambien 
incrementar la educacion vial a peatones y no incrementar la confianza en las calles.


![](https://github.com/caanibol11/PI2_CAI/blob/main/graficas/gr2.jpg?raw=true)
Gráfica por victima: se observa en la gráfica que el mayor número de victimas por accidentes se da en MOTO, con aprox 290 victimas, seguido de PEATON   con 260 aprox, y luego por Auto con aprox 90  casos. Esto quiere decir que la myoría de las victimas van conduciendo motos cuando ocurre el accidente vial. la campaña se debe enfocar en los conductores de motos, quienes deben revisar la velocidad con que viajan en las calles y avenidas, asi como el estado mecanico de la moto y los documentos en regla. Luego, tambien se debe enfatizar en las victimas por peatón, donde deben existir adecuada señalización y espacio para estos actores viales, como andenes, puentes, semaforos, cebras, parques, espacios sociales, zonas verdes, etc.

**DASHBOARD - POWER BI **



![](https://github.com/caanibol11/PI2_CAI/blob/main/graficas/gr3.jpg?raw=true)

Para presentar los resultados del análisis del EDA, se usó la herramienta POWER BI, donde se elaboró un dashboard con tres presentaciones relacionando las gráficas y medidas correspondientes al análisis de tiempo, datos personales como sexo, edad, y por último se discrimina por el lugar del siniestro vial.

![](https://github.com/caanibol11/PI2_CAI/blob/main/graficas/gr4.jpg?raw=true)

Adicional en este proyecto se estableció tres KPIs :
- Reducir en un 10% la tasa de homicidios en siniestros viales de los últimos seis meses, en CABA, en comparación con la tasa de homicidios en siniestros viales del semestre anterior.

- Reducir en un 7% la cantidad de accidentes mortales de motociclistas en el último año, en CABA, respecto al año anterior.

- Reducir en un 5 % la cantidad de accidentes mortales en la AVENIDA en el último año respecto al año anterior.


**CONCLUSIONES **

- De acuerdo a los resultados de las diferentes gráficas se puede concluir que la mayor parte de casos de siniestros viales ocurren con la conducción de MOTOS en una calle tipo Avenida, donde existen intersecciones y cruces entre calles y además es de doble sentido vial, por lo cual incrementa el riesgo de accidente. 
- Con base en lo anterior se recomienda implementar estrategias de socialización y concientización entre las personas entre edades de 20 a 40 años que son los principales actores de siniestros viales entre los años 2016 a 2021.
- En este periodo, se observa una reducción de los siniestros viales fatales, por lo cual hay una mejoría en las campañas de prevención viales, sin embargo, parte de estos resultados se deben  al fenómeno de la pandemia del año 2020 donde muchas peronas no salían de su casa.
- Se observa que la mayoría víctimas fatales son los hombres, superando a las mujeres en más de un 30%. Con lo anterior se confirma que los hombres son los que coducen en su mayoría  el vehículo accidentado. la campaña de prevnción de accidentes debe ir enfocado a los hombres conductores y verificar que su licencia de tránsito este conforme a la ley, ajustado la exigencia en su expedición.
- De las 15 comunas, la que tiene más cantidad de accidentes viales es la comuna 1, seguido por la comuna 4 y 9. La comuna que menos accidentes tienen son las comunas 5, 6 y 2.
- Tambien se debe enfatizar en las victimas por peatón, donde deben existir adecuada señalización y espacio para estos actores viales, como andenes, puentes, semaforos, cebras, parques, espacios sociales, zonas verdes, etc.


