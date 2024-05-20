¿Hay herramientas de machine learning insesgadas y consistentes?

R: "depende de la forma es la propiedad", la mayoría están sesgados.

Se realizó un menti:

Test de hipótesis.

Estos son los procesos de descripción de los datos, en los analisis exploratorios.

Estudiamos variables aleatorias:

Esta herramienta nos ayuda a entender que si uno se para a entender los segmentos desde ciertas variables aleatorias.

Permite acotar la probabildad de que un X sea (resultado)

"Que tan probable es que X suceda si Y"

Siempre hay que establecer un alpha: esta fija umbrales

Procedimientos:

Se plantea un problema
	¿Cómo me puedo asegurar si mi muestra es comparable, si son iguales? 
	R: No se puede, se deja al azar.
	Tener en consideración que hay factores que no podremos captar
	Se plantea una hipótesis:
		En primer lugar una hipótesis nula (H0) estas se plantean como si no existiera el efecto
		Junto con una hipótesis alternativa
	
Se selecciona un N:
	Consideración muestra: Que sea una muestra representativa
Se realizan grupos
Se realiza una experimentación
	
Se registra las observaciones (estableciendo métricas cuando sea necesario)
Se rechaza o no la hipótesis nula

### P - Valor ###

La probabilidad de que bajo H0 los datos muestren una diferencia = > a lo que observo

Lo que se busca es valor de p valor sea bajo.

Las corrientes que usan el p valor son la de Fisher y la de Pearson y Newman.

Si el p valor es grande, no hay efecto.

Cuando los valores son pequeños se utiliza la significancia estadística.

Es un instrumento de  "sorpresa"

Es muy importante este valor, corresponde a un estándar dentro de la investigación.


### Significancia estadística ###

Acota el P Valor.


El alpha valido dentro de la significancia son:
	0,1
	0,05
	0,01
	0,001

¿Qué testea?

Que tan real es el efecto.

"cae en la cola el grupo que se busca en cada grupo"

Que tan probable es que este sucediendo X o Y en una distribución de probabilidades < 0,05

Que hizo Pearson y Newman:
	La probabilidad en la que me este equivocando es chica.
	Para hacer un test de hipotesis se plantea la hipt, y entrega un p valor con una confianza.

Decir que tiene significancia estadística es parte de argumentar sobre que el suceso si tiene relación con lo propuesto en las hipótesis.

### Errores más comunes en los instrumentos ###

Error tipo 1: Falso positivo
Error tipo 2: Falso negativo, digo que hay efecto cuando no lo hay

Al no rechazar la hipótesis nula no acepta la alternativa.
En ningún caso se acepta la hipótesis alternativa.
Las hipótesis se rechazan, no se aceptan.

Malinterpretar el "no se rechaza", se interpreta como un "no soy capaz de observar"

La magnitud del p valor cuando sea pequeña no indica más valor en la apreciación de la significancia.


### Test de hipótesis ###

	1. Se establece una hipótesis nula y alternativa
	2. Se fija un alpha para compara el p valor y ver significancia estadística
	3. Estadístico para realizar el test de hipótesis (instrumento aleatorio que caracterice la muestra en función de su distribución)
	4. Definir supuestos o hipótesis "mantenidas" al realizar un test de hipótesis (¿altera la varianza?)
	5. Como distribuye el estadistico bajo la hipótesis nula 

No puedo testear que algo si existe, solo puedo tratar la probabilidad de observar lo que observamos dado lo que existe.

¿Qué sucede si las variables son complicadas?

"hay cosas incalculables si nos ponemos muy creativos"

Se analizan las métricas, hay que buscar el estadístico completo que responda la hipótesis (varianzas, medias)


"behacking: forzar la data para que llegue al p-valor objetivo"


![[./Recording 20240403155800.webm|Recording 20240403155800]]



#estadística #p-values #inferenciaestadística #testdehipótesis #consejos #classrecording









> [!failure]- Failure 
>   InsufficientQuotaError: 429 You exceeded your current quota, please check your   plan and billing details. For more information on this error, read the docs:   https://platform.openai.com/docs/guides/error-codes/api-errors.
>   
>   - plugin:obsidian-textgenerator-plugin:10968 Object.defaultFailedAttemptHandle    r [as onFailedAttempt]
>     plugin:obsidian-textgenerator-plugin:10968:21
>   
>   - plugin:obsidian-textgenerator-plugin:5098 RetryOperation.eval [as _fn]
>     plugin:obsidian-textgenerator-plugin:5098:29
>   
>  
