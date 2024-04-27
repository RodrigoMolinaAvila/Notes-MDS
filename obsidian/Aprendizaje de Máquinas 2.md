#regresiónlineal #machinelearning
Machine learning, se discute sobre la tarea 2, la tiene que tiene que confirmar el profesor para su resolución.

Llegué tarde.

Sobre auxiliar 3.

Ejercicio 1

Hay que asumir que theta es conocido, y que conocemos la varianza.

el truquito es:

El y es la variable aleatoria junto la gausiana.

En cada punto que me paro tengo que considerar la densidad dada por la formula

$$
p(y|\theta ,x) = \frac{1}{\sqrt{2\pi\sigma^2}} e^{-\frac{1}{2\sigma^2} (\theta^T x + \theta_0 - y)^2}
$$

2. #regularizaciónl1

Regularización L1 = LASSO, lo que haces es imponer un prior

Estoy regularizando, pero ¿Qué realizo?, conociendo las probabilidades.

Escribir el estimador de LASSO haciendo maximo a posteriori

Estimador LASSO:
$$
\Theta_{\text{lasso}} = \arg\min_{\theta} \left( \sum_{i=1}^{n} || y - (\theta^T x + \theta_0) ||_2^2 + \rho ||\theta||_1 \right)
$$
Si queremos encontrar el theta MAP (máximo a posteriori) #maximoaposteriori
$$
\theta = \arg\max_{\theta} \left( p(\theta|\{X_{1},...,X_{n}\}) \right)
$$
$$
\theta = \arg\max_{\theta} \left( P(D|\theta)\pi(\theta) \right)
$$
$$
\Theta_{\text{map}} = \arg\max_{\theta} \left( \prod_{i=1}^{n} \frac{1}{\sqrt{2\pi\sigma^2}} e^{-\frac{1}{2\sigma^2} (\theta^T x + \theta_0 - y)^2} \right)
$$
Aplicamos logaritmo: (se usa por monótona creciente) **el logaritmo de dos cosas es la suma de dos cosas)
$$
\log() = \arg\max_{\theta} \left( \sum_{i=1}^{n} \left( \log\left(\frac{1}{\sqrt{2\pi\sigma^2}}\right) - \frac{1}{2\sigma^2} (\theta^T x + \theta_0 - y_i)^2 \right) + \log\left(\prod \theta\right) \right)
$$
Se simplifica:

$$
\log() = \arg\max_{\theta} \left( \sum_{i=1}^{n} \left( -\frac{1}{2\sigma^2} ||\theta^T x + \theta_0 - y||_2^2 \right) + \log\left(\prod \theta\right) \right)
$$
Recuerda la distribución exponencial:
$$
p(x) = \lambda e^{-\lambda x}
$$
Hay que declarar que Rho > 0

Como ejercicio, argumentar probablisticamente que esta sucediento con el theta.
Sabemos que estamos regularizando

¿que sucede si aumento rho?

estamos castigando el tamaño de los parametros, en el estimador de lazo que es una seleccion de variables autimaticas.

El sentido probabilistico cuando tenemos un prior gausiano, la regularización que tenemos es ridge la regulación es gausiana es (0,1) cuando utilizamos r2 utiliza distribución exponencial.

Cuando aumenta lamda el gráfico se comprime y va cayendo más rápido.

### P2 Regresión no lineal ###

Se encontraba en la tarea 1, donde teniamos que utilizar medidas polinomiales

Proviende del paquete sklearn PolynomialFeatures.

Hasta que punto podemos aplicar caracteristicas polinómicas

Simule = tirar variables aleatorias
![[./Recording 20240405114555.webm|Recording 20240405114555]]
#regresiónnolineal