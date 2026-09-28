<img width="1903" height="917" alt="1" src="https://github.com/user-attachments/assets/711a8e54-27e4-4841-849d-5a3644d4ddd9" />
<img width="1915" height="957" alt="2" src="https://github.com/user-attachments/assets/67ff7546-826a-42e8-bc85-30e24ad37c9f" />
<img width="1920" height="941" alt="3" src="https://github.com/user-attachments/assets/748d44c7-b44d-4c61-b746-40da5de19f39" />
<img width="1920" height="956" alt="4" src="https://github.com/user-attachments/assets/3b92a9f9-e6a4-4321-93d1-0e4d5a9477f1" />

# Python-Analisis_Diego-Ramon
Proyecto para familiarizarse con la limpieza en bases de datos en Python y otros entorno de trabajo similares

# PASOS EJECUTADOS

1. Primero debemos crear un PATH en drive para poder almacenar ahí el dataset y luego poder leerlo con pd.read_csv.
2. Luego realizamos una serie de comandos para comporbar el estado de nuestros datos, por ejemplo, ver el número de columnas que hay, el tipo de dato que contiene cada columna, etc.
3. Convertimos los datos al tipo que corresponden seleccionando las columnas que no coinciden, por ejemplo, convertimos de texto a fecha. Se comprueba que la conversión esté bien realizada.
4. Comprobamos si hay duplicados en nuestro dataset. Por la naturaleza de nuestro dataset (préstamos de una ONG), no debería haber duplicados en ciertas columnas (tales como en el ID del préstamo), por lo que si hubiera alguno se debería eliminar.
5. Comprobamos si hay valores nulos. Por la misma razón que antes, en nuestro dataset hay columnas que no deben tener valores nulos (no tiene sentido prestar 0 unidades monetarias), por lo que debemos eliminarlos en el caso de que hubiera alguno.
6. Realizamos un mapeo de los países y distintas variables categóricas para normalizar sus nombres y que aquellas que puedan llamarse de varias maneras, acaben llamándose de una manera uniforme para facilitar su manipulación.
7. Normalizamos los formatos y tipos numéricos limpiando símbolos (cómo los de los tipo de moneda) y cambiando puntos por comas para la separación e identificación de los millares.
8. Comprobamos ahora los valores atípicos que tenemos en nuestro dataset identificando el primer y el tercer cuartil.
9. Con los valores atípicos definidos, determinamos que solución proponemos para su tratamiento. En nuestro caso, al ser un dataset financiero, no debemos eliminarlos ya que aportan información útil. Creamos un gráfico para que su visualización sea más comprensiva.
10. Creamos columnas nuevas que derivan de otras para que podamos usar información más compartimentada. Por ejemplo, las fechas se dividen por año, mes y día para que la manipulación y su uso más concreto sea prácticamente inmediato. Con las columnas derivadas también es más fácil visualizar porcentajes, ratios y calcular diferencias.
11. Por último codificamos unas variables categóricas para facilitar su recuento y su combinación con otras columnas/variables.
12. Realizamos comprobaciones concretas para determinar que no hay errores en el dataset.
13. Creamos el archivo final y limpio "kiva_loans_clean.csv"
