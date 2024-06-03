Backpropagation

Modelo regresión neuronal.

H hace producto punto

Las neuronas aprenden y adquieren propiedades de las capas aprendidas en los procesos anteriores.

Tengo que saber que es W:

Derivada: tasa de cambio.

Esto corresponde la pendiente o el arco tangente del angulo.

Se puede calcular la recta tangente.

Es la tasa de cambio, cuando es muy abrupta es cuando la derivada tiende al infinito.

Existe la derivada de la composición.

Los g indican la distribución:

Composición de funciones, se trata de utilizar el primer termino y elevarlo por el segundo termino componiendo funciones.

La red neuronal corresponde a una composición, por eso es importante las derivadas.

La salida de la red es una composición de funciones que derivan de equis.

Gradiente estocástico = regla de la cadena en derivadas.

Batches: es un conjunto de N muestras.

Se tiene que calcular la derivada, y se tiene que calcular cada una derivada por muestras, y se dividen por el total.

En backpropagation, se deriva en función a la dirección correcta.

U= activación, el resultado de la operación lineal

F =  Salida de las neuronas

J= capa k-ésima (donde se hace la activación, el peso, los calculos)

H= es un vector

H_k = es total de todos los resultados.

U^k_dj=

Pivote = punto intermedio, se selecciona justo el después del J. en este caso U

Dw_ij = Como depende de una neurona los pesos para activarla

No todas las capas tienen las mismas neuronas, es por eso que no estan definidas.

La suma ocurre en la capa anterior, es decir que es la sumatoria desde la k-1 a a=1

F(x) = x = 1

W solo afecta a W

Se encuentra una "recursión" para delta.

La recursión no es relacionada desde la k.esima

La recursión se encuentra en el error.

"Se entiende como la derivada de la capa k hasta el final"

Proxima clase, tipos de redes:
![[./Recording 20240603114837.webm|Recording 20240603114837]]
