# “Pronóstico del Acumulado Mensual de Pólizas de Automóviles en Panamá, para enero de 2024”

Estimar la cantidad de pólizas de automóviles en Panamá es crucial para el sector asegurador, ya que permite a las aseguradoras planificar la gestión de riesgos, establecer precios adecuados y garantizar la solvencia financiera. A medida que crece la cantidad de vehículos en territorio nacional, estas estimaciones ayudan a anticipar la demanda, adaptar productos y cumplir con regulaciones. Además, es esencial para el desarrollo de políticas públicas en seguridad vial y seguros obligatorios. Una proyección precisa fortalece la estabilidad del mercado y asegura una protección efectiva tanto para los conductores como para la industria aseguradora.

Bajo este contexto, hemos recabado información, obtenida de la web de la Superintendencia de Seguros y Reaseguros de Panamá, sobre el acumulado mensual de pólizas de automóviles desde enero de 2021 hasta diciembre de 2023, con la intención de estimar el acumulado del periodo de enero de 2024.

Para el desarrollo de este proyecto, a continuación, vamos a hacer uso de algunos de los modelos vistos en clases, como: Regresión Lineal, Promedios Móviles, Suavización Exponencial y Modelo de Holt y un último modelo investigado, ARIMA (3,1,3).

# Sobre las Pólizas de Automóviles en Panamá

El acumulado mensual de pólizas de automóviles en Panamá entre 2021 y 2023 proporciona información valiosa sobre el comportamiento del mercado asegurador en el país. Este periodo ha sido clave para entender las dinámicas de crecimiento del sector, influenciadas por factores como el aumento de la cantidad vehicular y cambios en la economía. 


![image](https://github.com/user-attachments/assets/c1d723e6-f509-4907-aac7-542c242a6126)

![image](https://github.com/user-attachments/assets/2eeec77d-1696-4a9c-a8d3-075a3243af06)

# 1. Modelo de Regresión Lineal Simple

![image](https://github.com/user-attachments/assets/6a376b37-d51f-481c-8611-6bf9939a05fb)

![image](https://github.com/user-attachments/assets/0c8ae0f6-a3d0-4e0a-89f7-cab190280079)

## Resultados

•	El pronóstico obtenido con la regresión lineal fue de 89186 pólizas para el periodo de enero de 2024.
•	Presenta un r2 muy débil, de 0.12, lo que indica que la variabilidad del acumulado de pólizas mensuales solo está explicada un 12% por la variabilidad o paso del tiempo (meses) y el otro 88% por la variación de otras variables.
•	Presenta un MAD de 6746
•	Presenta un MAPE de 8.0586
•	Presenta un MSE de 68411253
•	Presenta una señal de rastreo inferior de -3.12 y una señal de rastreo superior de 3.51, lo que indica que está dentro de los rangos, es decir, sin demasiado sesgo.


# 2. Modelo de Regresión polinomial de 3er grado

![image](https://github.com/user-attachments/assets/eb04bc66-f945-4f4f-a037-9033e7136a2b)

![image](https://github.com/user-attachments/assets/9db6b182-d04e-4515-87d5-fe8fd43a9fff)

## Resultados

•	El pronóstico obtenido con la regresión polinómica de 3er grado fue de 93399 pólizas para el periodo de enero de 2024.
•	Presenta un r2 muy débil, de 0.15, lo que indica que la variabilidad del acumulado de pólizas mensuales solo está explicada un 15% por la variabilidad o paso del tiempo (meses) y el otro 85% por la variación de otras variables.
•	Presenta un MAD de 6704
•	Presenta un MAPE de 8.0312
•	Presenta un MSE de 66551668
•	Presenta una señal de rastreo inferior de -3.00 y una señal de rastreo superior de 3.92, lo que indica que está dentro de los rangos, es decir, sin demasiado sesgo.


# 3. Modelo de Promedios Móviles

![image](https://github.com/user-attachments/assets/67a67f2d-0f7a-4702-ab57-6f7449f6a570)

![image](https://github.com/user-attachments/assets/42565eb1-2eda-4f1a-aef4-68f74a5dd12c)

## Resultados

•	El pronóstico obtenido con el modelo de promedios móviles fue de 91422 pólizas para el periodo de enero de 2024.
•	Presenta un MAD de 8337
•	Presenta un MAPE de 9.7997
•	Presenta un MSE de 95913247
•	Presenta una señal de rastreo inferior de -5.18 y una señal de rastreo superior de 1.73 lo que indica que está dentro de los rangos, es decir, sin demasiado sesgo.

# 4. Modelo de Suavizamiento Exponencial

![image](https://github.com/user-attachments/assets/02079f5b-fd6e-4075-89cc-85d78c9bddb1)

![image](https://github.com/user-attachments/assets/3deb91c8-2362-405e-b249-e5cc1b77f7b9)

## Resultados

•	El pronóstico obtenido con el modelo de suavizamiento exponencial fue de 85150 pólizas para el periodo de enero de 2024, con un Alpha de 0.057.
•	Presenta un MAD de 7269
•	Presenta un MAPE de 8.6261
•	Presenta un MSE de 80331254
•	Presenta una señal de rastreo inferior de -3.93 y una señal de rastreo superior de 6.24 lo que indica que está dentro de los rangos inferiores y solo un poco por encima de los superiores, es decir, sin demasiado sesgo.


# 5. 	Modelo de Holt

![image](https://github.com/user-attachments/assets/9a01efdb-0f24-47dd-84bc-4b19e8bf9c78)

![image](https://github.com/user-attachments/assets/a1cc011c-b4a4-4eb9-8af2-9466970f5688)

## Resultados
•	El pronóstico obtenido con el modelo de Holt fue de 89186 pólizas para el periodo de enero de 2024, con un Alpha de 0.05 y una beta de 0.354
•	Presenta un MAD de 7,156
•	Presenta un MAPE de 8.5655
•	Presenta un MSE de 77,622,853
•	Presenta una señal de rastreo inferior de -3.92 y una señal de rastreo superior de 3.20 lo que indica que está dentro de los rangos inferiores y superiores.


# 6. Modelo ARIMA (3,1,3)

![image](https://github.com/user-attachments/assets/ed54febe-3097-44e4-aa1e-c259a33dcdd8)

![image](https://github.com/user-attachments/assets/e6c76b0c-9ffe-489e-a441-47fb6ec2d518)

## Resultados
•	El pronóstico obtenido con el modelo de ARIMA 3,1,3 fue de 100,003 pólizas para el periodo de enero de 2024, con 𝜙1 de 0.10, 𝜙2 de 0.13, 𝜙3 de 0.37 y 𝜃1 de 0.10, 𝜃2 de 0.24, 𝜃3 de 0.14.
•	Presenta un MAD de 8,428
•	Presenta un MAPE de 9.6499
•	Presenta un MSE de 142,046,487
•	Presenta una señal de rastreo inferior de -1.97 y una señal de rastreo superior de 7.00 lo que indica que está dentro de los rangos inferiores y una unidad por encima de los superiores, es decir, con muy poco sesgo. 


# Resultados Generales

![image](https://github.com/user-attachments/assets/5c3336b4-ca86-4579-8e5c-396b1a63de3d)

•	En base a las medidas de error obtenidas y desviación estándar, se podría intuir que la opción del mejor modelo sería la de regresión polinomial de 3er grado, sin embargo, este modelo a su vez presentó un r2 de 0.15, recordando que hay que tener presente distintos indicadores para seleccionar un modelo que mejor estime el acumulado de pólizas y no solo los errores, nos indica que un 85% no está explicado bajo este modelo, hacen falta más variables. 

•	Por este mismo camino, el modelo de regresión lineal simple mostró un r2 de 0.12, inclusive más bajo que el anterior mencionado, y así sucedió con los otros modelos de regresión, el r2 estuvo alrededor del 0.12 y 0.15. Con los datos acumulados por año se nota un incremento considerable del coeficiente de correlación, sin embargo, este análisis se descartó debido a los datos atípicos que se mostraron en 2020 y los pocos registros a los que se tenía acceso (2017-2023), solo 7 años, 7 registros.

•	El modelo de promedios móviles mostró resultados muy parecidos, a destacar la desviación estándar un poco alta.

•	El modelo de suavización exponencial también presentó resultados similares, sin embargo, fue uno de los dos cuya señal de rastreo superior, está fuera del rango aceptado, por muy poco.

•	El modelo de Holt, también conocido como doble suavizamiento exponencial, obtuvo mejores resultados que el de suavizamiento exponencial, así lo reflejan sus medidas de error, rangos Ts y desviación estándar.

•	El modelo de ARIMA (3,1,3) mostró resultados muy cercanos a los otros 5 modelos, sin embargo, un poco altas; hay que resaltar que, para este modelo, bajo la metodología Box-Jenkins se recomiendan 50 registros (mínimos), actualmente tenemos 36 (3 años), por lo mencionado del 2020, no optamos por usar esos datos. Lo que podemos apreciar, es que, al comparar las dos gráficas, entre los datos reales y los estimados, el comportamiento es muy similar, debido a que no se trata de una regresión o una suavización de datos y contamos con más parámetros de estimación (7).

•	Por otra parte, contamos con los datos reales de enero de 2024 (brindados por la SSRP), en donde el acumulado de pólizas de automóviles es de 98365, siendo los más cercanos, la estimación por regresión polinomial de 3er grado con 93399 y la estimación del modelo ARIMA con 100003. Lo anterior indica, que el modelo polinomial presentó una diferencia de 4966 pólizas y el modelo ARIMA sobrepasó por 1168 pólizas, siendo estos los dos modelos que mejor estimaron los datos reales.

•	Por lo anterior descrito, recomendamos el modelo de regresión polinomial de 3er grado y el modelo ARIMA (3,1,3), el primero por todos los resultados obtenidos respectos sus medidas de error y haciendo la salvedad que y el segundo por ser el que mostró el comportamiento más parecido de los datos en el tiempo, sin contar que, al compararlo con el dato real del 2024, es el mejor estimador para este. En este caso, para ARIMA, podemos recomendar que se utilicen los 50 datos que exige la metodología Box-Jenkins y así ver si las medidas de error mejoran y sustentan el comportamiento similar al graficar los datos.





















