
Para cluster de k medias, buscar el menor SSE.

Cluster jerárquico
Cluster aglomerativo - distancia entre 2 clusteres
DBSCAN: Es comparable, evalua la densidad. Une por regiones contiguas.
- En dbscan se consideran los core, border y noise.
- Hay que asignar eps y minpts.

"Si hay muchas dimensiones, hay que aplicar PCA"

Como se calibra?

Método de la rodilla.
Analisis K-dist. Se define un K. (indica el vecino más cercano)

El salto indica el determinante para utilizar el valor de EPS.

Otras tecnicas:

Mapas autoorganizados
Fuzzy C.means
Mezcla de gaussianas y algoritmo EM.

Validación de clusteres:
"Se pueden validar en el mismo márco"
"Pensar en que representa el cluster"
"Determinar la tendencia de agrupamiento"
"Encontrar la cantidad óptima de k"
"Compara"

Para categórico aplicar ONEHOT***
Es sensible a las variables escala.

Métricas de validez: "Menor SSE: distancia cuadrática"
- No supervisada: si no tengo labels
- Supervisada: si tengo labels
- Relativo: mezcla entre ambas.

Para SSE: se espera un "menor valor"

Medidas de cohesión: Se calcula con SSE.
Medidas de separación: "Separación de clusters" "Métrica para el clustering total"

"Minimizar la cohesion y maximizar la separación"

"La suma entre la cohesión y la separación es una constante"

"Coeficiente de silhoette": entrega el balance entre separación y cohesión

Distancias:

Euclidiana: r=2
Manhattan: r=1
Similitud coseno: ???

Coeficiente de silhoette: "Medida interna"
Penaliza los puntos lejanos a su centroide
Penaliza puntos cercanos al cluster de al lado
"Se evalua entre 1 y -1": Mientras más cerca al 1, mejor.
"El coeficiente promedio, permite encontrar el K optimo"

Sihoette vs Codo. "Tiene la capacidad dual"

"No son claros para DBScan"

Matríz de proximidad:
"saquen una muestra por cada cluster"

"La distancia es lo contrario de la similutud" se puede aplicar razonamiento matemático

Permite observar la correlación entre las distancias y las pertenencias al cluster.

Correlacion utilizando k medias:
"Si el clustering es bueno el puntaje es alto" y visceversa.

"Queremos evaluar si nuestros clusters son reales o son efectos del azar"

Determinar numero óptimo de clusteres:

En el codo, el punto donde logre una diferencia en su expresión "es decir, cuando se ve plano, o muestra un punto de inflexión"

Medidas Supervisadas:

Busca correspondencia entre las etiquetas y las clases.

Por que??: Entregan información sobre los atributos de las clases. Ayuda para validar la técnica de clasificación. Etiquetación automática

Pureza y entropía: son terminos antónimos

Pureza: para la clase que tiene mayor probabilidad.

Evaluación de la significancia:
"Poder cuantificar la incertidumbre"
"Se simula con aleatoriedad"
Se realliza a traves de un histograma con muestras aleatorias de datasets compatibles:

"Traten de poner un nombre a lo que represente a ese cluster"

Conclusiones:
- Se puede utilizar como una técnica exploratoria.
- Entrega una visión, una estructura.
- Se evalua y valida a través de métricas internas y externas.



![[./Recording 20240517132422.webm|Recording 20240517132422]]





















