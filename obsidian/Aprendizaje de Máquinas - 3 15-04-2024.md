Entender las medidas de clasificación
- CLF Lineal
- Perceptrón
- Regresión Logística

 
Descenso de gradiente estocástico: (SGD) #descensodegradienteestocástico
Función de costo:

Sea X una variable aleatoria que existe en $R^m$ y $(T_t)_t$ existe en N
Cuando es una variable aleatoria hay que escribir una esperanza, que se expresa:

$E (J(theta,x))$

La consecuencia es que j termine siendo igualmente una variable aleatoria.

X distribuye en una variable desconocida (mu)

¿por que tengo que optimizar mi esperanza?

El descenso de gradientes

En el gradiente estocastico vamos punto por punto.

SGD toma una sucecion iid de la variable aleatoria: {X_t}_ten

Se busca identificar la densidad del dataset.

Lo vamos a tomar como una secuencia de punto aleatorios en X.

SGD va a actualizar una predicción de theta:

En escencia esto es descenso de gradientes.
$$
\theta^{\tau + 1} = \theta^{\tau} - n_t \cdot d_{\theta} \, j(\theta^{\tau}, x_{\tau+1})
$$
$$
D_{\theta} (\theta^{\tau}, x_{\tau+1}) = D_{\theta} \, \mathbb{E}\{J(\theta^{\tau}, x)\} + \Delta_{\tau}
$$
$$
\Delta_{\tau} = \hat{V}_{\theta} J (\Theta^{\tau}, x_{\tau+1}) - \hat{V}_{\theta} \mathbb{E}\{J(\theta^{\tau}, x)\}
$$

En estocastica es punto por punto, donde puede pasar cualquier cosa por donde tomamos las sucesiones.

Delta= grandiente estocastica
 
El algoritmo ayuda de salir de espacios donde puede ser considerado un minimo en la muestra. Entonces la sucesion (t rara averiguar) que decresca lo suficientemente lento.

El teorema que lo justifica: Sigmund y Robbins (1951)

Le pedimos a la funcion J que cumpla ciertas hipotesis de relatividad.
Tiene que ser integrable respecto a theta.
Tiene que ser de decrecimiento lento, una sucesion lenta hacia el 0.

SGD es escencial en redes neuronales.

Ahora lo aplicaremos en el caso particular del perceptrón:

¿Que hace?

Es un algoritmo de clasificación lineal.

Tenemos un conjunto de datos donde sus agrupaciones se ven dispersas dentro del plano, lo que busca es separar entre una clase y otra.

Es una alternativa al clasificador MSE.

Tenemos que utilizar otro tipo de features.
Consideremos:

y = { c1 si tetha transpuesto x + theta_0 igual o mayor a 0 c2 si tetha transpuesto x + thetha_0 < c}

donde:
 y(x)= f t(theta transpuesto phi (x))

La distancia del hiperplano determina la confianza
Cuando tengo mis datos bien clasificados en el caso ideal se cumple una condicion específica:
"para todo n=1 ... N ( {X_n, t_n}^n_n=1)"
Determinamos una función de costo J utilizando el criterio del perceptrón:

Lo que se busca con el resultado es estar lejos del punto crítico: 0

La idea es que esté mas alejado del punto critico en funcion del hiperplano separado.

Vamos a decir que nuestra funcion de costo:

J(tetha, x) = -theta transpuesto (xi)t_i 1_theta tranpuesto p (x1) t_i menor o igual a 0

Si queremos aplicar SGD a J:

D_theta J (theta_i , x_i) = - phi (xi) t_i
1 theta transpuesto phi (xi) t_1 menor o igual a 0

Entonces en cada paso actualizamos theta segun:

Theta transpuesto +1 = theta transpuesto - n_t delta_theta J (theta, x_t) = theta transpuesto + phi (xi) t_i ; 1 theta tranpuesto phi (xi) T_t+1 menor o igual a 0

Con descenso de gradientes encontraremos el punto más cercano a 0.

Regresión logística:

La regresión logistica segun el auxiliar: por que pensamos la funcion logistica?

como pensar el problema en probabilidades, determinar una nocion probabilistica del modelo,

hay que encontrar un hiperplano mu = thetha tranpuesto x + theta_0 que separe los datos.

Si es igual a 0 no tengo certidumbre de la clasificación.

Mientras el mu sea más positivo, más seguridad tenemos de que sea una clase (en este caso C_1)

Cuando se refiere a mas positivo es que si está mas cercano al 1.

No se usa para enfrentar un problema de regresión, solo para problemas de clasificación.

sigma R flecha a derecha (0,1)
R flecha sigma(r) = 1 partido por 1 + e elevado a -r

propiedad:

d partido por d_r por sigma(r) = sigma (r) (1-sigma(r))

La idea de la regresion es unir el hiperplano con la clasificación.

P(c_1|x) = sigma (tetha transpuesto x + theta_0) = 1 partido por 1+ e elevado a +theta transpuesto x - theta_0

Opciones del auxilar:

1) Optimizar "altiro"
2) deducir theta y theta_0
En la opción 2: cuando asumimos 
p(x|c_1) ~ N (mu_1, sumatoria)
p(x|c_2) ~ N (mu_2, sumatoria)

donde 

p (x) ~ alpha(mu_1, sumatoria) + (1-alpha) N (mu_2, sumatoria)

(mu_1, mu_2, sum, alpha)_ map = argmax theta sombrero pituatoria n 1=i p (x_i, c_1 | theta sombrero) elevado a t p(x_i, c_2 | theta) elevado a 1-t

= argmax theta sombrero sumatoria de n a i=1 t_i log (alpha) + (1-t_i) log (1-alpha) + t_i 1/2 {log (1 partido por 2ph elevado a n/2 |sumatoria| elevado a 1/2)} - (x-mu_1) sumatoria elevado a -1 (x - mu_1)^t

mu1  = medida empirica de la clase 1

Si modelamos con nuestra hipotesis gausiana podemos llegar a deducir la recta que modelaba, que mientras mas lejos estuviera, mejor estaria la clasificacion.

Approach discriminativo:

Lo unico que me interesa es modelar el p(c_1|x)

tetha_ map = argmax pituatoria n i01 sigma^t_i (1- sigma_i)^1-t
donde sigma_i = sigma (theta transpuesto x_i)
d/d tetha log sigma = (t, sigma_i) x_i

tiene una nocion de residuo "que tanto me equivoqué en el modelo"

Modelar como un modelo "generativo"
![[./Recording 20240415115020.webm|Recording 20240415115020]]





















