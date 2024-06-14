LDA es un proceso de dirichlet.

Prior propio: es mas facil tener una formula cerrada para la posteriori. 

Conjugado, la posterior distribuye igual que el prior.

A traves de la posterior marginal puedo detectar el parámetro de interés.

Intercambiabilidad: es un criterio deseable, es lo que se hablaba de que se acerca  a iid, pero no es iid.

LDA: Latent dirichlet allocation.

Cadenas de Markov: Proceso estocástico que describe una serie de posibles eventos donde la probabilidad de cada evento solo depende del evento anterior. Condicionado en el presente, el futuro y el pasado son independientes. La idea de las cadenas de markov es demostrar que la distribución del prior proviene desde la posterior.
$$
P(X_{n+1} = j | X_1 = i_1, X_2 = i_2, ..., X_n = i_n) = P(X_{n+1} = j | X_n = i_n)
$$

Existe una propiedad deseable en las cadenas de markov que es el estado estacionario.

Se puede entender como distribución estacionaria.
Con esta distribución se garantiza que se esta consiguiendo información de distribución de la posterior.

Algoritmo Metrópolis:

1- Tomamos theta_0 tal que p(theta_0|y) > 0 para partir p_0 (theta)
2- T=1,2,3...
a. Tomamos theta^* de una distribucion de salto (o "proposal") J(theta^*|theta^t-1)

b. calculamos r = p(theta^*|y) partido por p(theta^t-1|y)
c. defino: thetha^t ={tetha^* con probabilidad min (r,1)| theta^t-1} (esto es un ratio de aceptación o rechazo)

Se samplea desde la likelihood.

El estado de estacionario es optimo cuando sea inreducible.

Observación: para que esto realmente se pueda hacer (metropolis) J tiene que ser simétrica: es decir, P(j(theta_a|theta_b)) = p(j(theta_b|theta_a))

Hasting dice que J puede ser no simétrica.

Gibbs sampling:

El algoritmo de Gibbs Sampling se puede resumir en los siguientes pasos:

1. Inicializar los valores de las variables en el vector de estado $\mathbf{x} = (x_1, x_2, ..., x_n)$.

2. Para cada iteración $t$ hacer:
   - Para cada dimensión $i$ en $\{1, ..., n\}$ hacer:
     - Muestrear $x_i^{(t)}$ de la distribución condicional $P(x_i | \mathbf{x}_{-i}^{(t-1)})$, donde $\mathbf{x}_{-i}^{(t-1)}$ denota el vector de estado en la iteración $t-1$ excluyendo la $i$-ésima dimensión.

Este algoritmo genera una secuencia de muestras que convergen a la distribución conjunta de interés.

Periodo de calentamiento: primeras 100 muestras que no considero para generar la posterior. Esto es para la calibración del modelo.

Para observar el buen ajuste, los histogramas generados por el muestreo de datos tiene que parecerse al dato dado por la posterior. Es decir, tiene que parecerse a los datos originales.

ver: Gellman pt2. Para ver formas de evaluar.


![[./Recording 20240611155752.webm|Recording 20240611155752]]




