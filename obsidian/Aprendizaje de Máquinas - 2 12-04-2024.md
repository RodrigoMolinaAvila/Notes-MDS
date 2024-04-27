Ver slide 7.

Hoy vamos a ver los problemas de clasificación. #clasificación

Problema de clasificación y nociones de problemas de clasificación.

En un espacio de datos (ambient space)

Tenemos espacios representados en diferentes clases (X|C)

C = Clase

El problema surge cuando aparece un nuevo elemento, si resolví el problema, tengo que determinar cual es la clase de ese nuevo elemento.

En esta clase resolveremos cual es el problema lineal
El parametro es: $$ a^tx+b $$ Que tenga un transpuesto significa que "Existe en R"

La linea vectorial se define: Es posible denominarla como frontera de decisión $$ y(x) = a^tx+b = 0 $$ Para definir una clasificación se considera$$ y(x) = a^tx+b < 0 $$ $$ y(x) = a^tx+b > 0 $$ 
Antes de definir a y b:

Consideremos 1. $$ X1, X2 \in \text{frontera} $$
2. $$ \exists X \text{ tal que } a^T x + b = 0 $$
3. $$ 0 = y(x1) - y(x2) $$$$ 0 = a^T x1 + b - a^T x2 - b $$$$ 0 = a^T (x1 - x2) $$Entonces la proyección de A se encuentra en:
   
Para cualquier X existente en los reales.
$$ \text{proy}_a(x) = \frac{a}{||a||} \cdot ||x|| \cdot \cos(\theta) $$
 $$ \cos(\theta) = \text{ángulo}(x,a) $$ $$ ||\text{proy}_a(x)|| = ||x1|| \cdot \frac{a^T x}{||a||} $$ $$ ||x1|| = \frac{b}{||a||} $$

 
** A controla el ángulo de la recta y el b controla el sentido **

3) "y es una distancia con sigma a la frontera"

X_f = es la proyección de X en la frontera.
Lambda a union = es el vector de la frontera.
1. $$ y(x) = a^T (x_r + r a_{\text{unión}}) + b $$ $$ y(x) = a^T r \hat{q} = a^T \left(\frac{a}{||a||}\right) r = ||a|| r $$ $$ a_{\text{union}} = \frac{a}{||a||} $$ Ahora como extendemos esto a multiclase.

K - Clase r  #k-clase
1) One v/s all: no es consistente
2) One v/s one: tampoco es consistente
3) Multiclases: Si tengo k clases, utilizo k clasificadores
En este caso se testea las clases buscando el minimo, esto corresponde una probabilidad no normalizada
$$ J = argmax y_j (x) $$
¿Cómo ajustamos y encontramos a y b?

Hint: recordar que es un problema de regresión donde:
El problema lineal no abarca todos los conjuntos de datos:

Utilizar minimos cuadrados cuando las clases son similares (tienen la misma cantidad de elementos, por simentría)

Pero cuando no son similares no se utiliza mínimos cuadrados.

Perceptrón: uno de los primeros modelos de A.I. (es una motivación para gradientes estocásticos)

Modelo perceptron = #perceptrón

1. $$ y(x) = f(a^T x + b) $$
$$ f(u) = 
\begin{cases} 
1 & \text{si } u > 0 \\
-1 & \text{si } u < 0 
\end{cases}
$$ Recuerda:$$ \theta^T \hat{x} = a^T x + b = u $$ ¿Cómo asignar el fn de coste?
$$ J(\theta, \text{datos}) = \sum_{i} J(\theta, x_i, c_i) $$

Se clasifica entre los valores que tienen el punto, se dividen por el valor que entregan, si son positivos están bien clasificados y los que tienen puntaje negativo están mal clasificados.

Los puntos mal clasificados:
$$ - \sum_{i} c_i \cdot \theta^T \hat{x} $$
Modelo discriminativo: Tengo un x y necesito saber la clase #modelodiscriminativo

Modelo generativo: construyo modelo para generación de datos, voy a determinar como los datos se generan, tanto su x como su etiqueta. #modelogenerativo
$$ p(c,x) = p(c|x) \cdot p(c) $$
$$ p(c_1|x) = \frac{p(x|c_1) p(c_1)}{p(x)} $$

$$ = \frac{p(x|c1) p(c1)}{p(x|c1) p(c1) + p(x|c2) p(c2)} $$

$$ = \frac{1}{1 + \frac{p(x|c2) p(c2)}{p(x|c1) p(c1)}} $$

$$ p(c1|x) = \frac{1}{1 + e^{-a}} $$

Donde: 

$$ a = - \log \left( \frac{p(x|c2) p(c2)}{p(x|c1) p(c1)} \right) $$

*** Regresión logística: *** #regresiónlogística
-1 en un vector
1/2 en la recta
1 en otro vector
$$ p(c1|x) = \frac{1}{1 + e^{-\theta^T x}} $$



![[./Recording 20240412115142.webm|Recording 20240412115142]]







 