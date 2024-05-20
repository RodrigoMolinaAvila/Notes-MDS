 Sobre tarea 2: Inferencia de parámetros.
Una forma de ajustar mi modelo tiene que tener menos pérdida:

Se usa el Error Cuadrático Medio (ECM):

Lo que queremos para encontrar la mejor recta para ajustar mis datos, es encontrar aquel beta que acorte lo más posible su distancia de la recta.

Luego de su "matrakeo" queda: 
$$\hat{B} = (X^T X)^{-1} X^T Y$$
Propiedades de su estimación.

¿Como se si el estimador es bueno?

Podemos sacar la segunda derivada de esto, para ver si estamos en un mínimo o un máximo.

Segunda derivada por esimación OLS: 
$$2X^T X$$Es un óptimo (mínimo) si es definida positiva
Recordar que estamos en una matríz. Tiene que ser invertible.
Estaremos en un minimo global si esta matriz esta definida positiva.

Sesgadez y varianza del estimador:

Insesgadez: $$\mathbb{E}(\hat{\beta}_{OLS}) = \beta$$Varianza:
La varianza es necesaria en la variable, en la medida que ya tengo todos los patrones, puedo hacer un mejor análisis de datos.

Al analizar por ols, es insesgado si el valor esperado es 0, además si contamos con mucha variabilidadad, la varianza será chica y llegará a la consistencia.

Mientras mejor sean mis datos, mejor será la estimación.

¿Cual es su forma?

Homocedasticidad**

Supuestos OLS:

Supuesto 1: El modelo es lineal y el error es aditivo ¿Que significa? que el modelo es lineal en los parámetros, los betas entran en modelo lineal.
Supuesto 2: Muestra iid, Esperanza = 0 Varianza de (X_ik) es grande entonces la varianza de (beta_ols) es chica.
Supuesto 3: Multicolinealidad: El rango de (X transpuesto X) = K completo, en terminos intuitivos no puedo asumir multicolinealidad, ya que las variables no se explican perfectamente por las otras lineales.

Los supuestos 1 y 3 son esenciales para realizar la estimación

Supuesto 4: No Endogeneidad o Identificación
$$\mathbb{E}(X^T \epsilon) = 0$$
$$\text{Cov}(X, \epsilon) = 0$$
$$\mathbb{E}(\epsilon | X) = 0$$
Cuando hago problemas orientado a identificar, se necesita aseverar: ahi se habla de una causalidad.

No tiene que estar correlacionado con algo que no estamos observando.

"Todo depende de algo"

Cuando me aseguro que no hay endogenidad, implico causalidad.

"Revisar el curso de inferencia causal"

Supuesto 5: Homocedasticidad 
$$\text{Var}(\epsilon) = \sigma^2_{\epsilon} I$$
Teorema de Gauss - Markov: Bajo los supuestos del 1 al 5 OLS es el estimador lineal insesgado de mínima varianza -> Blue/Meli (Mejor estimador lineal insesgado) {Mejor beta_ols}

Si se cumple, no hay mejor modelo de estimador de regresión lineal, es decir que tiene la varianza mas chica posible.

Es muy facil que no se den en la práctica.

![[./Recording 20240425160145.webm|Recording 20240425160145]]


