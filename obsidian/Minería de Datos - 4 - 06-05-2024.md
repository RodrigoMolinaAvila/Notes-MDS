Clustering: Encontrar grupos de ejemplos en datos sin recurrir a etiquetas previas.

Los clusteres dependen de sus atributos como datos agrupados.

Es mas "cualitativo"

Lo que se busca minimizar la varianza intercluster, y maximizar la varianza intracluster.

Desde la parte exploratoria nos entrega información acerca de sus atributos.

K-Means:

El algoritmo busca "la asignación de cluster" y "re-calcular centroides"

k = cantidad de clases que se busca encontrar.

centroide: promedio a nivel vectorial.

La asignación de K de forma aleatoria inicial no es "tan bueno"

Es muy improbable encontrar un cluster "optimo" cuando las k que se buscan son altas (en el ejemplo expone k = 10)

Cualquier truco de eliminar outliers "ayuda"

Cluster jerarquico aglomerativo:

Analiza el posicionamiento de los clusteres

Es una tecnica antigua.

Se trata de calcular la matriz de distancia entre clusteres.

Se trata de unir clusteres para conseguir otro.

El problema es la distancia euclidiana.

Cuando se realiza un dendograma, cuando se itera se juntan los que tienen un "menor" valor entre los puntos de clusteres.

Puede ser en orden de procedimiento, iniciar con cluster de k medias y luego proceder al jerarquico.

DBSCAN:

Algoritmo de cluster basado en densidad

Se trata de interpretar las posiciones de los clusteres dentro del plano. Establece un analisis a traves de los parámetros "EPS" y "MinPts"

Estos puntos pueden resultar en: "core", "border", "noise" (su interpretación es intuitiva)

Permite identificar mas precisamente los "ruidos", aislandolos o descartandolos.

Sobre Hito 2:

En funcion de las preguntas describir el metodo que se utilizará para responderla. Es algo parecido a las preguntas directices pero con métodos.

Solo ejecutar 1.
![[./Recording 20240506131413.webm|Recording 20240506131413]]


















