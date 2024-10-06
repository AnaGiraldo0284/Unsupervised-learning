## Informe sobre algoritmo K-Means - Parcial.

### Ana Sofía Giraldo Franco
### Mariana Franco Ramírez 
### Nicolás Lemus Mora

Hemos realizado un total de 5 versiones usando el algoritmo K-means, la implementación de este algoritmo fue totalmente manual, con el objetivo de entender su funcionamiento para su uso práctico a futuro. A continuación, veremos un poco más de detalles al respecto:  

La base de datos que fueron utilizados para la realización del algoritmo fue *EA sports FC 25*, pero con todos los jugadores (cantidad de datos: 17737).  

-	Se realizó un análisis exploratorio de los datos (EDA) para el entendimiento correcto de los datos para mejorar sus estadísticas y comprender sus características.  

-	Encontramos los datos faltantes y los imputamos para manejar los valores nulos, en cuanto al pie preferido de los jugadores, lo convertimos en una variable binaria de igual forma, usando 0 y 1.  

-	Por otro lado, para la implementación del algoritmo k-meas, usamos librerías como numpy, pandas, matplotlib.pyplot, seaborn, skalearn y mlp.toolkits.mplot3d la cual es un módulo de matplotlib.  

-	Se implementó el algoritmo K-means de manera manual, usando la librería sklearn, también, usando la librería sklearn con el algoritmo K-means++ y finalmente, el algoritmo K-means con tres diferentes distancias (Euclidiana, de Mahalanobis y Manhattan).  

-	El algoritmo K.means consiste en formar grupos de alta similitud la cual está determinada por la distancia que existe entre los datos. Su funcionamiento consiste en cinco pasos: En el primer paso se escoge el número de clústers (K) de manera óptima, esto por medio del método del codo. En el segundo paso se seleccionan de manera aleatoria los centroides que son los puntos que establecen los centros de cada clúster y con estos se pueden calcular las distancias a los demás datos, de esta manera se inicializa los clústers escogiendo aleatoriamente cada punto dentro de los datos a analizar. El tercer paso consiste en asignar los clústers, para esto, se recorren los datos y se calcula la distancia de cada punto a cada centroide para asignarlos a los clústers más cercanos, además dependiendo de que tan buenos sean los grupos, se realizan más iteraciones o el algoritmo se finaliza. En el cuarto paso se recalculan los centroides en caso de no haber terminado con el algoritmo. Finalmente, en el quinto paso, tras recalcular y hallar los nuevos centroides, se repiten los pasos 3 y 4 con el objetivo de ajustar cada vez más los clústers, si se ha indicado una cantidad máxima de iteraciones, esto se hace hasta conseguir la calidad deseada o hasta que se le haya indicado al algoritmo.   

-	Se usa PCA (Principal Component Analysis o Análisis de componentes principales) como técnica de reducción de dimensionalidad, esto con el fin de tener mayor rendimiento en el algoritmo, pues el PCA permite toma un conjunto de variables correlacionadas y las convierte en variables nueva e independientes la cuales se denominan “Componentes principales”. Reduciendo las dimensiones a 2D y 3d para su visualización gráfica. 

### Conclusiones generales:  

En conclusión, el algoritmo K-Means es un método de agrupación que se fundamenta en la asignación iterativa de los centroides más próximos, actualizándolos hasta alcanzar la convergencia, es decir, hasta que los datos no sufran una alteración significativa. La forma en que medimos las distancias entre puntos en un conjunto de datos específico afecta la forma en que esos puntos se agrupan en grupos. La distancia Euclidiana puede generar agrupaciones compactas pero pueden ser influenciadas por variables atípicas, la distancia Manhattan podría generar agrupaciones más dispersas pero menos impactadas por valores atípicos, mientras que la distancia Mahalanobis, al incluir la información de covarianza, puede generar agrupaciones que representen de manera más efectiva la estructura subyacente de los datos, esta nos presento diferentes inconvenientes a la hora de su ejecución, por lo tanto, lo hicimos de dos maneras diferentes. Es fundamental visualizar los resultados en un espacio en 2D para determinar la calidad de los clusters. Además, una representación en 3D.
