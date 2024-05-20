Enfoque regenerativo de la regresión logística - de eso se va a tratar la tarea. #enfoqueregenerativo

Al decidir el modelo primero hay que ajustar una línea.

El overfitting depende de los grados del polinomio de la prueba. #overfitting

Existen dos fuentes de incertidumbre

Incertidumbre epistemológica: incertidumbre inherente al set de datos.

La información correspondiente al entrenamiento y el test tienen que estar mezclado.

¿Cuál podría ser una técnica que podría servir en todos los casos?

Entrenar el modelo varias veces, es decir entrenar el modelo en diferentes P.

¿Cómo se llama eso?

Validación cruzada, es el "sello de garantía" para demostrar que el modelo "mejor". Esto significa hacerse cargo de cierta aleatoriedad de los datos. #crossvalidation

Hiperparámetro: los hiperparámetros se deciden a mano a través de una métrica. #hiperparámetro

Al asumir la distribución de los datos es uniforme, tengo que seleccionar puntos del dataset.
Otra forma, es asumir la gaussiana, con los datos se ajusta la media y la desviación estándar.
También puede ser un chi cuadrado.

Existen modelos no paramétricos. Estos modelos pensaría que no tiene tienen parámetros pero si lo tiene. #modelosnoparamétricos

Por ejemplo en un histograma es un modelo no paramétrico, ya que tiene información contenida en cada bin a diferencia de las distribuciones (n, gaus, x2)

Validación cruzada exhaustiva: Es un tipo de VC exhaustiva. Donde se prueban todas las particiones #validacióncruzadaexhaustiva

Leave p out:
Leave one out:

Es una buena métrica dejar 50% entrenamiento, 25% para validación y 25% para test.

Esto tiene para mitigar desventajas:

A través del criterio de información Akaike (AIC) #akaike

En caso es un mal modelo:

Cuando hay pocos datos, es decir que si la realización de datos es buena, mi estimador será "bueno".

Tenemos que definir la esperanza de la verosimilitud, también conocido como riesgo: #esperanzadelaverosimilitud #riesgo
$$
\mathbb{E}(L) = \int L(\theta|x) P_\theta (x) dx
$$

Aproximación de Laplace (?)

La gausiana es el taylor de orden 2 de las distribuciones.

*** señala que a través de maxima verosimilitud no siempre se utiliza el modelo real, se elige bajo supuestos ***
Formula de red neuronal de una capa: #redneuronal $$
y(x) = \sum_{i=1}^{k} \theta_1 f_1 (x)
$$

Vectores de soporte vectorial: #vectoresdesoportevectorial
Restricción:

Los puntos mas cercanos al vector en C_1 y C_2 se pueden definir como los soportes vectoriales. Lo que hace es definir el punto intermedio del margen. Estos fijan la pendiente.

Hay que considerar que con 2 puntos no se puede definir el margen.

El margen es: 

**los escalar se pueden transponer**


![[Recording 20240419114757.webm|Recording 20240419114757.webm]]


