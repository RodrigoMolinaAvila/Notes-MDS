En esta clase responderemos las preguntas

- Es Theta_mle insesgado?
- Es inconsistente?
- Es eficiente

Se realiza a traves del hesiano: que es una "segunda derivada"

Es una condicion de seugndo orden para verificar si estamos en un maximo local.

Nos da la informacion de la curvatura que tiene la verosimilitud en nuestro punto máximo.

Nos dice como se comporta la curvatura, si es pronunciada o no.

Cuando la curvatura es más pronunciada la varianza/disperción es menor y viceversa

Analizar el hessiano nos permite conocer la curvatura.

Hessiano responde como se comporta la varianza del theta_mle

La funcion de verosimilud puede ser "lo que nosotros queramos"

Se espera en el hessiano sea definido negativo.

La matriz de información de fisher, "smoothness" de f:

La condición de segundo orden esta ordenada en el hessiano.

Dependiendo de las caracteristicas van a aparecer

Las formulas van apareciendo cuando se dan las caracteristicas de la muestra.

La matriz de información se utiliza cuando n tiende infinito (asintótico)

Condiciones de regularización:

- Las primeras tres derivadas de la función ln f(x|theta) con respecto a theta son continuas y finitas y para casi todo X_i y para todo theta. Esta condición asegura la existencia de ciertas expanciones de Taylor y que la varianza sea finita. Cuando tenga esta condicion puedo demostrar consistencia. theta_mle es asintóticamente insesgado, con esto podemos podemos conseguir la consistencia del estimador.

Hay un estimador es consistente es cuando la varianza se da a 0.

- si se tienen las condiciones necesarias para obtener la esperanza de la primera y segunda derivada de ln f (x|theta). Esto se utiliza para verificar que el maximo verosimil es asintóticamente normal.

En el greene esta la demostración de todas las formulas.

La idea es conseguir la intuicion de como conseguir la estimación.

- Si tengo todos los otros criterios, es posible encontrar la efenciencia del estimador, es decir que theta_mle es de mínima varianza.

Se necesita demostrar que existen estas condiciones, que se realiza a traves de la demostración matemática.

Cuando se cumplen estos 3 criterios se demuestra que theta_mle es BUE (Best unbiased estimator)

Esto se da en lo asintótico.

En un mundo no asintótico theta_mle es sesgado, es decir que la var(theta_mle) es "dudosa".

*Cuando se trabaja más con los  datos es más perceptible los sesgos*

Test de ratios de verosimilitud: test de hipótesis: como mejora mi modelo en medida que agrego más varianza.

H0: 
![[./Recording 20240509154753.webm|Recording 20240509154753]]





