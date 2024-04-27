Crisp DM: Es una metodología que propone 6 estapas para *asegurar resultados* #drispdm

Considerado en las tesis del magister.

El objetivo es obtener una respuesta a traves de los procesos metodológicos.

Es la mas usada en proyectos exploratorios en Data Science.

Es importante conocer la institución contextualmente es importante para entender de forma mas profunda los datos.

Este metodo es iterativo e incrementual.

- Analizo el problema: 
- Comprendo y preparo
- Modelo y evaluo
- Despliegue

Crisp - ML: Con el desarrollo de la IA existe un nuevo proceso metodológico. #crispml

Cuando no se necesita comprender tanto el problema, es un esquema de analisis enfocado en el proceso de reintentar y rediseñar.

Análisis exploratorio: #análisisexploratorio

- Propósito: Tiene que ir alineado con el objetivo del negocio y del proyecto de data science
- Juicio Experto v/s Estadística: Calcular y comparar la intuición del experto, en función de actualizar o cerciorar la información.
- Toma de decisiones: En funcion de los datos y sus resultados del análisis, modificar o cambiar o datos.

La estadistica sirve para discriminar los datos. #consejos 

No sirven las variables que tienen la variable 0 ?
Es importante apreciar la varianza en las variables.
Cuando la varianza es muy grande pueden haber outliers.

Si hay una diferencia en KS indica que hay una variable relevante que me puede mostrar un fenomeno. Se encuentra en sklearn.

Hay que contrastar las distribuciones de la data.

Para que sirven los test de hipótesis.

### Equidad estadística
 #equidad estadística
Garantiza los resultados del analisis no esten sesgados y que reflejen de manera justa la realidad.
Asegura la no discriminación en datos.

Se basa en la Ley 20609: Buscar en biblioteca del congreso.

¿Cómo discriminamos?

1. A través de una discriminación histórica en los datos.
2. Discriminación por integración de varias fuentes de datos. Incluye el sesgo del inscriptor y creador de la variable.
3. Atributo sensible como proxy. 

Existen formas de identificar estas discriminaciones:

Kamiran et al. (2012) #teoría
Enfoque de Diferencia en proporciones.
¿Por que las premisas no son proporcionales?

Se comprueba la probabilidad de que suceda algo segun los datos.

Cuando hay desproporcion en los datos indica sesgo.

AI Fairness 360: Un toolkit opensource. #toolkit

Entrega herramientas para mitigar sesgos.

Sesgos en los datos y sesgos en los algoritmos.

Hay que tener cuidado con la herramienta luego de mitigar los sesgos.

** No hay certeza de como va a terminar el modelo **

Utilizar la diferencia como ponderación para equilibrar el sesgo.

¿Cuales son los sesgos? #sesgos

Cherry picking: seleccionar lo que me sirve
Data dregreding: testear hasta que lo manipule
Survivorship bias: dataset incompleto
Danger of summary metrics: solo mirar los sumarios
Sampling bias: utilizar una muestra no representativa
Publicación bias

P-Values: #p-values 

P-Hacking: Manipular data o analisis para artificialmente obtener p-valores significativos. Cuando los analisis son escogidos en base a si el p-valor es significativo y no cual es el mejor plan de análisis.

Malos entendidos clásicos de la estadística:

- El p-valor no es el error tipo 1: cuando digo que hay efecto y en la realidad no lo hay.
$$
\text{P-valor} = P(T(x) > t | H_0)
$$
Es la probabilidad de que yo este observando una diferencia bajo una propuesta de hipótesis.
La P-valor no indica la "intensidad" de la significancia

- No podemos quedarnos con los p-values que esten al límite de la significancia, el p-valor no dice nada sobre la magnitud del efecto.
- La hipótesis nula nunca se aprueba, se indica la capacidad o no de rechazar lo que estoy probando.
- No tener significancia estadistica significa la capacidad de no poder descartar una hipótesis, lo que no significa junto con enviar todos los resultados a la basura.

### Family Wise Error Rate
#familywiseerrorrate
Se utiliza para comparar el p valor
$$ 1-(1-{alpha})^{number of tests} $$
### Corrección de Bonferroni
#correcióndebonferroni
Es una forma de aumentar la cota de la distribución de la muestra si es mayor 
$$ alpha/N test $$
Si el p-valor es menor al resultado, podemos aseverar interpretación estadistica.

Recordatorio: #consejos 

Comienzo mi proyecto con mi objetivo en mente.
Hago mi analisis exploratorio.
Hacer test de hipótesis.
![[./Recording 20240409155446.webm|Recording 20240409155446]]
