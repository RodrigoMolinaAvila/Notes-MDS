Random Forest.

Recordemos bagging

- Se generan datasets con metodo de bootstrapping
- Se ajustan los modelos phi (x,d)
Este método es útil cuando los modelos de generadodos por bootstrpping es útil cuando los modelos tienden a estar sobreajustados.

Bagging mejora el error reduciendo la varianza.

Random Forest es una actualización práctica que mejora el bagging.

En el caso de cuando tenemos modelos $$ {\phi} (x, d^{(b)}) $$ la varianza de bagging es rho sigma cuadrado mas 1 menos rho partido b por sigma cuadrado.

donde rho > 0, es la correlacion dos - a - dos

"Se reduce varianza y se induce sesgo"

Random forest intenta reducir la correlación rho en el caso de caso de arboles y entre los arboles.

¿Que cumple arboles que nos interesa en bagging?

Son arboles profundos de modelos que tienden a sobreajustar.

"Para que un modelo no este correlacionado no hay que ocupar las mismas variables"

En random forest será ajustado usando un subconjunto de árboles.

¿Cuantas variables?

Si son muchas podemos incurrir en el riesgo que no encontremos la variable a clasificar

Para regresión: p/3 
Para clasificación: raiz de 3
"esto es para que partan por algo"

Esto es para asegurar que no exista la correlación.

Dentro del algoritmo de RF, la diferencia con bagging es el momento de selección de variables.

"es primordial entender la diferencia entre random forest y bagging"

### Boosting

"Ensambla modelos"
Esto refiere a encontrar modelos con errores, en funcion de reclasificar ese error de forma aislada de la clasificación inicial.

"Consideramos modelos phi "flojos""

Un modelo flojo es cuando gamma > 0 y delta > 0. 

El error será menor a 1/2 - gamma con probabilidad mayor a 1 - delta.

Con esto existe una probabilidad "grande" de que mi modelo sea mejor que el azar.

Paradigma usual:
- 0 < epsilon < 1, delta > 0
- El error sea menor a epsilon
- Con probabilidad 1-delta

***Pac-aprendibilidad debil - pac-aprendibilodad fuerte*** 

Lo que demuestra boosting, es que las dos familias inducidas son iguales, es decir, puede hacer que uno con aprendibilidad debil sea fuerte.

Boosting "convierte" modelos flojos/debiles en modelos fuertes.

¿Cómo se logra esto?

Se ocupan varios modelos debiles, se ajustan, se ponderan y podremos reducir el error en una cantidad arbitraria epsilon.

El algoritmo es AdaBoost.

Boost se refiere a impulsar/potenciar "que agarren vuelo"
 *** Revisar el apunte para considerar los ejemplos y los supuestos presentados para adaboost  pp. 96***

Dentro del boosting se reinterpreta la L(phi_m) a w, es decir, se interpretan los errores de los modelos probados anteriormente como un peso para el nuevo algoritmo.

Explicación algoritmo adaboost:

"partimos con un peso uniforme"
"vamos a meter a la suma los pesos donde se equivocó"
"vamos a minimizar el peso"
"vamos a calcular el error ponderado"
"vamos a utilizar el teorea anterior para obtener al alpha_m"

"entrenamos un modelo nuevo, lo entrenamos, pero lo entrenamos según la fase anterior"

"en este caso se busca el signo como resultado en el caso de clasificación binaria"

Adaboost es para clasificación binaria. (en sklearn)

Considera la noción de residuo, tambien llamado como "cuanto nos equivocamos", "cuanto me sobró/faltó" se encuentra la formula en la pp 98.

Esto se puede interpretar como "el residuo del modelo de m-1"

¿Qué estamos haciendo?

Estamos diciendo que nuestro modelo nuevo, va a justar correctamente cuanto nos hemos equivocado.

"la nocion de boosting, es ajustamos, y luego ajustamos en los errores"

### Gradient boosting

En vez de ocupar como funciónes de perdida como las vistas anteriormente, las utilizaremos como variables.

"se interpreta como una versión funcional"

Lo que hace es agregamiento aditivo por capas, y junto con la ponderación de los errores.

Explicación del algoritmo:

"toma un conjunto de datos"
"ajustamos un primer modelo penca"
"para cada m, vamos a calcular un residuo generalizado, dado por la derivada de nuestra función de perdida en un punto donde vamos a tomar como output en un phi dado x"
"quiero que estos sean mis nuevos pesos (residuos)"
"el gradiente para ese punto esta dado cerca de 0"
"ajustamos un nuevo modelo en los residuos directamente, minimizamos la diferencia,"
"ajustamos los residuos en los gradientes"
"actualizamos los rho"
"actualizamos la función phiM(x)"

¿como se que me fue bien en el proceso de gradientes?
Tiene que ser 0 cuando me fue bien, es decir, que me estoy acercando a un punto critico de mi función.

Que hacemos con árboles?

"boosting no es recomendable en un modelo que ajuste, o que sea fino"

bagging reduce varianza.
boosting corrige el sesgo.

boosting conviene cuando los modelos son de baja varianza y que van a tener un sesgos, pero ese sesgo se va corrigiendo a medida que se suman modelos.

Se utliza en arboles "chicos" o de baja profundidad.

En gradient tree boosting, el ponderador se encuentra en cada hoja del modelo.

XGBoost, es una variante de gradient boosting.


![[./Recording 20240701114927.webm|Recording 20240701114927]]





