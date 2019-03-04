<h1>Clusters: algoritmo k-means</h1>

JUPYTER-NOTEBOOK: https://github.com/robagliom/clusters_k-means/blob/master/k-means.ipynb

K-means es un método de agrupamiento, que tiene como objetivo la partición de un conjunto de n observaciones en k grupos, en 
el que cada observación pertenece al grupo cuyo valor medio es más cercano.

Dado un conjunto de n observaciones (x1, x2, …, xn), donde cada observación es un vector real de d dimensiones, k-means construye una partición de las observaciones en k conjuntos (k ≤ n) a fin de minimizar la suma de los cuadrados dentro de cada grupo: 
S = {S1, S2, …, Sk}.

Pasos del algoritmo:
* Paso 1:
        Seleccionamos al azar k centros de agrupamientos (centroides). Tomamos como centroides c1, c2, .., ck; podemos decir
        que C = c1, c2, .., ck es el conjunto de todos los centroides.
* Paso 2:
        Asignamos cada valor de entrada al centroide más cercano. Este se hace calculando la distancia euclidiana entre el punto y
        cada centroide.
* Paso 3:
        Encontramos el nuevo centroide tomando el promedio de todos los puntos asignados a ese grupo.
* Paso 4:
        Repetimos los pasos 2 y 3 hasta que ninguna de las asinaciones de cluster cambie.
        
Elegir el valor de k:
Con frecuencia, conocemos el valor de K. En ese caso, usamos el valor de K. De lo contrario, usamos el Método Elbow.
Ejecutamos el algoritmo para diferentes valores de K (por ejemplo, K = 10 a 1) y trazamos los valores de K contra SSE (suma de errores cuadrados). Y seleccione el valor de K para el punto de codo.
