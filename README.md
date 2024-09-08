# Conclusiones 

# ANALISIS UNIVARIADO 

Se utilizó un dataset de un banco portugués con 45,211 registros y 17 columnas, enfocado en la efectividad de campañas de marketing para nuevos créditos. La columna objetivo, "poutcome", indica si una campaña fue efectiva o fallida. Se encontraron 36,959 valores nulos en esta columna, que fueron eliminados, reduciendo el dataset a 6,412 registros. Además, se eliminaron registros etiquetados como "otros" para mayor claridad. La columna objetivo se transformó en variables numéricas, codificando campañas fallidas como 0 y exitosas como 1. El análisis reveló 1,488 campañas exitosas y 4,850 fallidas. Los gráficos mostraron que el 76.5% de las campañas fueron fallidas y el 23.5% efectivas, proporcionando información valiosa sobre la efectividad de las campañas y posibles áreas de mejora en marketing.


# ANALISIS BIVARIADO

Aunque no se encontraron correlaciones significativas entre las variables del dataset que permitieran predecir si una campaña de marketing es efectiva o no, se lograron establecer varias conclusiones valiosas. En particular, se determinó que los retirados, desempleados y estudiantes tienen una proporción similar de campañas fallidas y efectivas.

Adicionalmente, se observó que los trabajadores en el sector blue-collar y los de management fueron quienes recibieron el mayor número de intentos de comunicación, y también presentaron la mayor cantidad de campañas fallidas. Estos fueron seguidos por los trabajadores en las categorías de admin y technician.


# PREPARACION DE LOS DATOS 
En la preparación de los datos, primero se realizaron las siguientes transformaciones:

Dumificación: Se crearon variables dummy para aquellas variables categóricas con solo dos respuestas posibles:

poutcome (éxito o fracaso),
contact (celular o teléfono),
housing (propietario de vivienda o no),
loan (con o sin préstamo).
Normalización: Las columnas numéricas balance, pdays, age, day, duration y previous se normalizaron dividiendo cada valor por el máximo de su respectiva columna.

Codificación ordinal (cart codes): Las variables categóricas con más de dos niveles, como job, education, marital y month, se codificaron de manera adecuada para ser incluidas en el análisis.

Con las variables correctamente dumificadas, normalizadas y codificadas, el dataset está listo para analizar correlaciones y probar diferentes modelos de machine learning.
