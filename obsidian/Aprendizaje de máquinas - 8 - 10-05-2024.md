En la resolucipon del problema phi puede ser cualquier cosa, estamos hablando dentro del contexto lagraniano, en la separación por SVM.

Cauqluer k que sea menos que 0. 

Por que? "Es por punto vector"

Los K que sirven son los K que tienen forma de producto punto.

Cuales son?

Se necesita un teorema:

Si tenemos uq eecontrar un objeto pero noq uiero diseñarlo con el producto punto.

"me gustaría que phi tenga dimensión infinita".

Las dimensiones se pueden interpretar como atributos.

Las variables pueden tener distintos componentes: (signifca su forma en la cuales como se grafican), tambien pueden llamarse como features.

"Queremos encontrar un phi que no esta en R^d, sino que en R infinito"

Recuerda: el phi son atributos.

Cuando esta en infinito es una función.

Un buen phi puede ser

Al estar en inifito el valor de R toma un valor en R.

Cada punto va asociado a una función entera.

Una funcion de dos variables se grafica en un plano.

Cuando x 1 y x 2 dentro de la función son 0 significa que son máximos.

El phi siempre lo usaremos en producto punto.

cuando phi es constante, k tiene que ser positivo.

Cuando los phi son iguales, k tiene que ser positivo.

Cuando k es escalar, tiene que ser un k escalar postivo.

La bidiagonal son los X mas cercanos a la diagonal.

Dentro de la matriz la diagonale tiene los valores mayores.

Phi no depende de X.

Propiedad de Kernell (K): que garantiza que tiene producto punto.

K es una función definida positiva:

Tiene que ser simétrica, porque phi conmuta.

Si K es definido positivo phi tiene un simétrico.

Todos los mercer kernell existen un phi para k

Teorema de mercer dice:

Si k es un mercer kernell

Para hacer un SVM se necesita calcular el producto punto.

Uno tiene la expresividad en el espacio finito con conmutatividad en el espacio infinito.

Como esta definida en dos dimensiones, K tiene que ser definida positiva. (en el caso infinito en el espacio de los datos)

En el caso finito, K es una matriz.

K es elproducto punto entre x_1 y x_2

el phi arregla el producto punto, es decir, que hace que tenga sentido el producto punto.

Phi corresponde al espacio latente

K corresponde al espacio real.

En un espacio K finito, equivale a phi transpuesto phi.

buscar en wikipedia "positive define matrix"

"buscar algo relacionado como 20 statements son equivalentes"

Hay que asegurarse que cumpla su definición.

La integral rescata solo los valores que pasan por sobre 0.

Uno no construye el K, sinó que existe una biblioteca de K.

Kernel polinomial: En este se puede encontrar el phi. Todos los puntos tienen que ser calculados por K_pol (x,y) = (c+xtranspuesto y)^d

Funcion de base radial: gausiana, kernell gaussiano, igualmente es definida positiva.

Kernell periódico: muestra caracteristicas periodicas.

Que pasa ahora con los SVM???

Esta tecnica es no paramétrica. En ningun momento se entrega la solución. Se hace el calculo abstracto para conseguir las predicciónes.

La función de costo depende de finitos datos.


![[./Recording 20240510114726.webm|Recording 20240510114726]]


