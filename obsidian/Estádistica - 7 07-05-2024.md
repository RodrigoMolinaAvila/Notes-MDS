Comentes sobre la tarea.

1) la varianza no tiene relación en el sesgo
2) Es mejor es insesgado con varianza pequeña.
4) Podía tener relación la varianza
5) el p valor no dice nada sobre el efecto, es normal tener un p valor chico en una muestra grande. basar toda una política pública en el p valor. Comentar desde la estadística. Las opiniones no ameritan puntaje, se tiene que argumentar desde la estadística. Leer con más detalle. 
6) Se puede resolver en muchos test en grupos distintos.
7) El intervalo se acota, y cuando aumento el nivel de significancia el intervalo crece.
8) Cuando se tiene una muestra chica, se puede determinar normalidad facilmente, ojo con las muestras, cuando es muestra chica los test pueden dar cualquier cosa.
9) Es asintitoticamente insesgado
10) Sobre la moneda es solo operación de estadística
11) Si el ks score es alto las distribuciones son distintas. se responde en función en los turnos de mejor productividad, en funcion de homogeneizar criterios. Indicar que bajo el contexto si hay diferencias. La correlación sea 0 no significa que sean independientes. Sugerir indagar más con otras variables.

Materia:

Tarea 2 es de estimación paramétrica.

El modelo presenta parámetros que se buscan explicar el fenómeno.

Primero: modelos lineales
Segundo: OLS

Sus supuestos:
- Linealidad
- Muestra iid
- Multicolinealidad
- Endogeneidad
- Homocedasticidad

El curso es inferencia causal, electivo MDS.

Estos supuestos permiten utilizar el teorema de Gauss-Markov: Cuando se cumplen los supuestos P_ols es BLUE/MELI: el mejor estimador lineal insesgado.

R cuadrado: cuanta varianza explica la muestra dentro de los parámetros. Explica la variabilidad.

Formas de estimar: Métodos de los momentos.

Recordad: una distribución de probabilidad puede ser descrito por sus momentos.

Los momentos se definen así:
$$\mu_k = \mathbb{E}(X^k)$$
Recordad que la varianza tiene relación con la media.

Ejemplo 1: X distribuye Poisson (Lambda)

$$P(X=x) = \frac{\lambda^x e^{-\lambda}}{x!}$$

El lambda del metodo de los momentos es el promedio.

Es criterio de la poisson es que la esperanza de x y lambda de x es igual al promedio.

Hay que asumir que X distribuye poisson

El promedio ajusta a X.

Otro ejemplo:

Se estiman los momentos, y se pueden relacionar a los parametros que necesito de la distribución, es decir, que en el momento 2:

Momento 1: Centralidad
$$\mu_1 = \frac{1}{N} \sum_{i=1}^{N} X_i^1 = \hat{X} = \hat{\mu}$$

Momento 2: Dispersión$$\mu_2 = \frac{1}{N} \sum_{i=1}^{N} X_i^2 = \sigma^2 + \hat{X}^2$$ $$\hat{\sigma}^2 = \frac{1}{N} \sum_{i=1}^{N} (X_i - \hat{X})^2$$
Método de máxima verosimilitud:

Definición: Sea X=(X_1,X_2, ...., X_n) variables aleatorias con densidad conjunta F(X|theta) con parametros que viven en este espacio paramétricos, la funcion de MVS se define como:

La funcion en conjunta describre Y.

En la práctica se sabe que existe un parámetro normal.

Esta funcion muestra que se puede hacer con theta.

En el mundo ideal, tengo las x y conozco a la perfección theta.

Busca econtrar aquel theta que maximiza la ocurrencia de las X que estamos observando.

Y se maximiza, para maximizar la ocurrencia de X.

Esta función es abstracta. No necesita criterios previos.

Observaciones:

Max Likelihood :
- es una función de tetha, o para theta. X es fijo.
- No es una PDF, no está normalizada, esto quiere decir que puedo ajustar la muestra, es decir una normal, una poisson, etc. porque base a eso defino la F
- Es necesario conocer o asumir una distribución. Si o si hay que decir como distribuye.
- Trabajaremos con variables iid. por que? porque permite realizar pituatorias

Log verosimilutud: Es más facil de computar. al trabajar con variables iid, se tranforma en la sumatoria de log(f(x_1|theta))

Para minimizar, es como la menos log verosimilitud.

Para poission se estima el parámetro lambda

La pitatoria se transforma en la sumatoria en logaritmo.

El logaritmo de la exponencial se anula.

La sumatoria al resolverse pasa por N

Al trabajar la expresión, se hace mas facil derivar.

Las tecnicas tienen pro y contras, se llegan a resultados iguales o similares con los ejercicios.


![[./Recording 20240507160227.webm|Recording 20240507160227]]












Para llegar al estimador de mínimos cuadrados ordinarios se necesita
