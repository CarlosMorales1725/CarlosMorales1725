Se creo un modelo que sea capaz de identificar si un paciente
tiene cancer o no para lo cual evalue con 4 modelos diferentes
y decidi cual fue el mejor justificando la respuestas en base a las
matrices realizadas en cada modelo

1.-Se realizo un archivo Jupyter Notebook y se trabajo con el 
data wdbc.data para lo cual el primer paso fue importar las librerias 
necesarias para el proyecto 

2- Ejecutamos  el archivo que vamos a analizar y se le agrego los headers 
o cabeceras a sus columnas para una mejor visualización luego de eso en la 
data se cambio en la columna de diagnosis los valores de Maligno y Benigno a 0 y 1,
luego de eso visualizamos la data df para ver si tenemos valores flotantes y convertirlos
a enteros para lo cual utilzamos astype que es el método para convertir un objeto a un tipo 
especificado, luego de eso quitamos la columna Id para nuestro analisis dividimos nuestra data 
en tres grupos diferentes en mean,se,worst , se realizo una data con 5 columnas para hacer las graficas 
la primera grafica lo utilzamos para ver la columna de diagnosis con sus valores teniendo como 
resultados mayores de cancer de tipo benigno y maligno mas bajo como indica la primera grafica
se hizo 2 graficas en las cuales me muestra datos de columnas de la data con la columna diagnosis 
comparando en dos colores en cual hay mas malignos y benigos otra grafico que ingresamos fue el de 
pairplot de serborn mostrando las interacciones de cada columna mostrandose de color azul como 
benigmo y de color naranja maligno siedo en la mayoria de columnas el tipo de cancer benigno- Luego 
utilizamos una grafica para mostrar la correlación de los datos.

MODELO 1 

Construiremos un modelo a partir de el conjunto de datos del conjunto de datos entrenados para 
lo cual utizamos accuracy para representar el porcentaje total de los valores correctamente clasificados
sacando un valor de 0.92 luego de eso se realizo la matriz de confusión de l primer modelo 
en el cual tiene falsos negativos de 7 y falsos positivos de 6 siendo un buen modelo para poder identificar si 
un paciente tiene o no cancer 

MODELO 2

Se creo un modelo con un arbol de decisión DecisionTreeClassifier para visualizar la columna de 
diagnosis igual utilizamos un accuracy para representar el porcentaje total de los valores correctamente
clasificados sacando un valor de 0.37 y con una matriz de confusión teniendo un falso negativo de 0 
y un falso positivo de 108 siendo este un mal modelo.

MODELO 3

Se creo un metodo de Random Forest para la regresion y clasificación teniendo el modelo mas
preciso por que accuracy se acerca mas al 1 (100%) 

MODELO 4 
Se utilizo el metodo de KNeighborsClassifier para predecir y clasificar los datos del modelo 
teniendo un accuracy de 94 

Como conclusión general creo que etercel modelo y el primero podrian ser los mejores para 
poder identificar si un paciente tiene o no cancer.


