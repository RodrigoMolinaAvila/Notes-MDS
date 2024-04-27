
Aprendizaje de máquinas: #machinelearning 

Repaso inferencia bayesiana: #inferenciabayesiana

Se hace un setup donde:
$$
D = \{(x_i , y_i)\}_{i=1}^{n}
$$
Hay que asumir que D fue generado por:

$$
y_1 = \sum_{j=1}^{n} \theta_j \phi_j(x_1) + e_i
$$
Donde se asume que la distribución es:
$$
e_i \sim N(0, \sigma_e^2) \quad \text{iid}
$$
Podemos observar en theta:
$$
P(\theta | y_1, \ldots, y_n, x_1, \ldots, x_n)
$$
Paréntesis:

$$
\phi_0 = 1
$$
$$
\phi_1 = X
$$
$$
y_1 = \theta_0 + \theta_1^T x + 3
$$
Sin embargo, otra elección de phi permitira en y:
$$
y_1 = \theta_0 + \theta_1 x + \theta_2 x^2 + \theta_3 x^2 + e
$$

Cuando uno ve el modelo importa la expresividad del modelo: lo que importa es si es lineal o no en theta no en X

Modelo de mínimos cuadrados regularizados (MCR)
$$
\Theta = (X^T X + \rho)^{-1} X^T Y
$$
Tenemos que tener en consideración que todos los X pueden tomar el valor phi!

EMV:

$$
\Theta = \arg\max_{\theta} P(\theta | y_1, \ldots, y_n, x_1, \ldots, x_n)
$$
$$
\arg\max_{\theta} \sum \log P(\theta | x_1, y_1)
$$
Si distribuye gaussiano se establece:
$$
\arg\max_{\theta} \sum \log \left( \frac{1}{\sqrt{2\pi\sigma^2}} \exp \left(\frac{-1}{2\pi} e \left(y_1 - \sum \theta_j^T \phi_j(x_1)\right)^2\right) \right)
$$
Para el próximo ejemplo tenemos que asumir en

### Inferencia bayesiana ###

Se establece un metodo para establecer una probabilidad sobre el parametro

A priori no podemos decir nada sobre el parametro antes de ajustarlo

los datos son fijos, nada se puede hacer para alterar los datos

Queremos que el modelo represente espacios de baja y alta probabilidad

Se dice que las funciones hay una region del espacio donde hay una alta probabilidad que este mi función

Para establecer mi funcion la variable aleatoria es theta.

Esto se llama prior, o distribución a priori que se da a traves de una elección del diseñador:
$$
p(\theta | D) = \frac{p(D | \theta) p(\theta)}{p(D)} \propto p(D | \theta) p(\theta)
$$

La constante de normalización es P(D)

$$
P(\theta|D) \propto P(D|\theta) p(\theta)
$$
$$
= \prod p(\theta | y_1, x_1) p(\theta)
$$
$$
= \prod_{i=1}^{n} \frac{1}{\sqrt{2\pi\sigma_e^2}} \exp\left(-\frac{1}{2\sigma_e^2}(y_1 - \sum \theta_j^T \phi_j(x_1))^2\right) p(\theta)
$$

En una gaussiana: 
$$
N(\theta, \mu_0, \sigma_0^2)
$$


