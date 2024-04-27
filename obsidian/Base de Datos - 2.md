
Sobre el control 1:

Existe un párrafo relacionado con contexto dentro del enunciado.

Como consejo: 
- Leer el parrafo completo
- Identificar las tablas y sus contenidos
- Identificar las caracteristicas
- Vincular con llaves foreaneas la relación con otra tabla
- Agregar detalles adicionales necesarios para identificar
- Cerciorar con el enunciado completo y verificar las tablas y sus relaciones

Cuando hay que hacer muchos joins, hay que iniciar con la tabla que tiene más tablas foraneas.

Las consultas tienen esstructuras similares generalmente.

Parte por la condición, y luego identifica la estructura.

Charla:

Sobre base de datos:

Rodrigo Pizarro 
Lead Machine Learning Engineer. - Rappi
Trabaja en el sistema de recomendaciones de Rappi

Ojo con los ascensos, hay que negociar los trabajos para lograr ascensos, a traves del cambio de trabajo u contraofertas.


- Se establecen objetivos principales
- Dentro del análisis de machine learning se puede utilizar en bases de datos en tiempo real, geolocalizando la información.
- Ojo con las interpretaciones y la evaluaciones del usuario final
- Problema de cold start: entregar las recomendaciones en base a la data para buscar las sugerencias

Dentro del MLops
- Design
	- Entender y responder las necesidades o problemas del negocio
	- Tenemos lo que necesitamos?
		- Data QA
		- Infra
- Model Develpment
	- Preparación de la data 
	- Desarrollo de los modelos
- Ops
	- Como lo podemos en producción, asegurando que la data esté buena, no estamos usando una data equivocada, no estamos haciendo predicciones incorrectas, tenemos las variables suficientes, darnos cuenta en el momento del error ** ** **
	- CI/CD/CT
	- Tipo de predicción
		- Batch: calcular las predicciones para cierto tipo de usuarios predeterminadas. x tiene predicciones, las sube, las carga
		- Tiempo Real: Search, a traves de la recepción de la query del usuario, entregar la sugerencia
		- Contextual (Session based), basado en la travesía del uso, se hace la recomendación 

Sobre la base de datos:
SQL: Bare minimum de la industria
- Snowflake (SQL)
- Amazon S3
	- Data que no carga en el tiempo
	- CSV para front end - backend
	- Resultados de Modelos
- REDIS
	- Feature Store
	- Data en memoria acceso ultra rápido


Airflow: Orquestador de datos ¿Qué es?, que correr, cuando correr, y que hacer 

- Definición de DAGs: Son flujos que no tienen ciclos y que son dirigidos, se puede programar
- Programación: se programa en intervalos o momentos específicos

Para que sirve?

Automatizar trabajos programáticamente dividiéndolo en subtareas
permite su planificación y monitorización desde una herramienta
Orquestar datos, mantenimiento previo, y tareas de administración.
Es relevante además, ya que las organizaciones importantes utilizan los orquestadores

Base de datos: SQL Best practices

No es solamente que la query corra, sino que corra bien y que sea fácil de mantener.
Trabajar contigo mismo, y mantener buenas practicas por eso es necesario tener un framework para trabajar

habla contigo mismo a traves de los comentarios
Primero: Entender que cuando se actualiza data y escribiendo data nueva, cada query, cada select que hagas tiene el costo (monetario)

No se hace un select con asterisco

Siempre hay que filtrar

Hay que tener muy claro que data usar, utilizar asterisco no es correcto.

***** Aplicar where and group by before join and union *****

Si tienes que hacer grandes procesamientos de datos: dividelos!

Procesar el datos en múltiples procesos.

Es recomendables utilizar templates para estructuras de querys.

Jinja: herramienta para utilizar estructuras de querys

Bases de datos: be mindful

Es necesario usar todas las columnas?
Necesitamos tantos años de data

Mala practica: update con nueva data en toda la data general

Buena practica: comenta todo tu codigo, elegir correctamente el nombre de las variables

Una variable que entregue detalles en su escritura puede ayudar a recordar de lo que se trabajo durante el futuro.

Learn to code: programacion orientada a objetos, code with classes, aprender a abstraer el codigo, "Clean Code" by robert c martin, no tener miedo a leer codigo.

Learn SQL: minimo

Expandir el toolbox: Aprende hacer reques a api
Aprende a usar orquestador like airflow
Aprender algun servicio cloud
Aprender herramientas python


Estadisticas básicas:

A/B testing
Significancia estadística
Regresiones, minimo conocimiento

Busca incomodidad!

Si no aprendo en tu trabajo, buscar donde aprender, buscar otro trabajo

Tener un buen jefe, aprende de el, motivacion

Problemas de machine learning en la vida real.

Desafios de ingenieria:

Mantenerse actualizado en la industria

XTboost
Regresiones logisticas
Arquitectura de deep learning basados en transformers.

![[./Recording 20240411175257.webm|Recording 20240411175257]]













