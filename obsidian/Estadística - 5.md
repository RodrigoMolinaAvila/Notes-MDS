Se realiza una presentación en menti.

Se realiza un resumen de la primera parte del curso: Estadística tradicional

De acuerdo las propiedades de los estimadores y sus variables aleatorias, estos tienen proíedades.

Desde la inferencia estadistica, esta se enfoca en la predicción y la identificación. En ciencia de datos se interesa en la predicción.

Depende el modelo se decide el enfoque.

Test de hipótesis:

Equidad estadística. Tiene fundamentos desde la estadística clásica {Fairenes in AI|ML}

Expone sobre equidad estadística: 

Test mann withney - U test. Prueba no paramétrica.

Kruskall wallis H test: parametrico para pruebas no normales.

"La probabilidad de que no existe una diferencia es muy baja"

Como recomendación, es parte del analisis exploratorio realizar los análisis estadisticos y aplicar estimadores convenientes.

AI FAIRNESS 360: tiene herramientas para proteger grupos privilegiados, en funcion de aplicar la ley correctamente (ley de las variables).

En el analsis estamos al borde de lo político, diferenciar entre la opinión técnica y la opinión política. Como consecuencia las personas empiezan a sesgar.

Modelos OLS: 

¿Como identificamos si un modelo propuesto es bueno?

Es un modelo que tiene un error bajo, el modelo es bueno cuando se equivoca poco.

Métricas: precision, accuracy, recall.

¿Que miden?

Falso positivo, falso negativo, etc.

Se comienza con funciones de pérdida: ¿Que signfica?

Una función de perdida, intuitivamente determina el costo de estimar uno de los argumentos mediante el otro.

Definición matemática:

Sea, tetha eciste en omega y a existe en omega un estimador, entonces el costo de estimar theta medianta a esta dado por la funcion de costo definida mediante:
$$
L(\omega \times \omega) \rightarrow \mathbb{R}
$$

$$
(\theta \times a) \rightarrow L(\theta \cdot a)
$$

Como ejemplo existe el error cuadrático:

Es el modelo que miniminiza los errores:
$$
L_2 (\theta, a) = ||\theta - a||^2
$$ Queremos aquel modelo lineal que minimice el error

Minimos cuadrados ordinarios: OLS

$$
\hat{\beta} = (X^T X)^{-1} X^T y
$$

X transpuesto X tiene que ser invertible.

Por el determinante, y cuando las columnas son linealmente.

Lo cual es algo que no siempre se puede dar.

Si hay una dependencia lineal no es invertible.


![[Recording 20240423160022.webm|Recording 20240423160022.webm]]
