#mineríadedatos 
Algoritmos de clasificación: Árboles, KNN, Naive Bayes.

Existen dos algoritmos de predicción que entregan dos caminos para llegar al función F (a) = y

#árboldedecisión
Árbol de decisión:

¿Qué hace?

Elige atributos y hace distintas ramas que puede tomar el atributo, lo busca reductivamente buscando un valor a predecir.

El árbol elige atributos y corta el data set.

El corte en el árbol se traduce: pregunto por el atributo a1 y pregunta la probabilidad de una opción u otra.

La idea de árbol es que encuentre atributo que sean buenos ejemplificando particiones distintas.

Se denomina dentro del arbol de decisiones un "arco entrante" y un "arco saliente"

El arbol fragmenta el dataset.

Hay mas de un arbol apropiado para cada dataset.

Tambien se puede utilizar en datos no etiquetados.

El modelo predice solo una clase.

¿cómo lo entreno?

- a través de estrategia, "top - down"
Eligo atributo, y creo rama para cada valor posible
Divide las intancias.

Si tengo un criterio, se aplica el mismo criterio recursivamente hasta que se logre la clasificación

Tiene que ser un criterio computable.

Ejemplo de clase: dataset Weather.

Primero: defino un criterio de atributo de partición
Se establece un criterio binario para cada atributo dentro de los valores dentro de la categoría para buscar una región pura, es decir, esten muy concentrados en yes o no.

Segundo: que atributo elijo?
se tiene que tener en consideración la entropía para elegir cada región, se promedia esa entropía y ver cual es el atributo que me da menos entropía. 
La entropía da la formula de criterio para elegir los atributos.

El resultado de la entropía se traduce en **Bits**.

El dataset se particiona en función de los valores que tiene la variable.

El resultados termina cuando ya los resultados no pueden seguir particionandose.

Ojo con los atributos de muchas categorías, son beneficiados por su capacidad de fragmentar el dataset.
Uno de los beneficios son la interpretabilidad del método.

Evolución del analisis de los arboles
### Random Forest ###

Combinación de arboles de decisiones

### Gradient Boosting ###

Arbol que aprende de los errores

## Clasificador KNN  (Key nearest neighbors)

Es la noción de distancia.

Se calcula la noción de distancia de sus vecinos más cercanos.

Es un metódo que requiere alto valor de procesamiento.

"Si me parezco a algo, debo ser eso"

Como se hace?
A través de raiz euclideana
A traves de la distancia Minkovski

Para escalar distnancias a traves de la normalizacion distancia 0 y varianza unitaria
Tambien una normalizacion a rango 0 y 1

Esto se hace solo en los datos de TRAIN.

La metodología de pre-procesamiento y normalización tiene que ir en training y testing.

ojo con el oversampling cuando hay pocos valores predecibles.
el oversampling esta en las filas, no en las columnas.

¿Tiene sentido hacer oversampling en mi data set?
Es una pregunta que hay que realizar antes de aplicar este metodo.

k = hiperparametro.

Cuando hay un K.

La validación es una subpartición entre el train y el test

La validación es un punto para evaluar hiperparametros antes de realizar el testing.

*** Grid Search ***

## Naive Bayes

Es un clasificador desde el punto probabilistico
*** es el mas facil que hay ***

ofrece miradas distintas.

¿cual es la idea?

dado un set de entrenamiento, construir un estimador de probabilidad.
 *** algoritmos distributivos y algoritmos generativos ***

estimar las probabilidades a traves del teorema bayesiano

se necesita crear un supuesto que entregue posibilidad.

¿que hago?

asumir independencia en los valores.
una vez que se el valor de x|y dado que se la clase, esto se llama interdependencia condicional

Se calcula la probabilidad de todas las variables con el y dado.

Se utiliza Laplace Smoothing

Que sucede con atributos numéricos??  ver slide


![[./Recording 20240408131531.webm|Recording 20240408131531]]








