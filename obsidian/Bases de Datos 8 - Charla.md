Datalized:

Uso de SQL en analítica.

Analitics engineer.

Datalized: Solucionan problemas de negocios a traves de herramientas de bussiness inteligence y machine learning.

Es una empresa que es parte de un monton de empresas conocidas y grandes.

Ciclos de vida de data science:

Recoleccion: data engineer, ml engineer
Limpieza: data analyst
Analisis expxloratorio: data analyst, data engineer
Construcción modelo: data scientist
Implementación modelo: data scientist, ml engineers

ml engineer, ve el rol del analisis completo del modelo propuesto.

La realidad chilena son entre "data engineer" y "data analyst"

Ejemplos práctocos sql:

Data sur: es la base de datos que contiene las exportaciones.

Se utilizó para informes comerciales e identificar factores que afectan la compra / reglas de negocio.

Es importante la depuración de los datos, si entra basura de base de datos, es posible que salga basura de la base de datos.

Es importante almacenar las actualizaciones para conocer históricamente los valores que se encuentran dentro del procesamiento realizado.

json se utiliza en postgres.

Es imporante utilizar trigger y funciones:
Reutilizacion de codigos.
Modularidad y mantenibilidad
Depuración y pruebas.
Documentacion y legibilidad
Limitaciones y lenguaje triggers

se utiliza el lenguaje plpgsql en este caso para las funciones mixtas.

Ejemplo blue express:

Las historias de los pedidos (datos) van en constante reprocesamiento.

Es una buena práctica utilizar un truncate en vez de cargar toda la data una y otra vez como sucedio en blue express

los triggers se actualizan de forma automática.

Procedimiento de almacenado 
- Comparar ambas tablas
- Update de la validez
- Insert de nuevos registros.

Para la consultoria es lo principal es la confiabilidad del dato.

Las logicas involucradas dentro de la ciencia de datos es lo primordial en vez de la herramienta.

Es importante avanzar a traves de procesos, es decir, lo más basico, y más adelante explorar la herramienta que se solicita que es más innovadora. Primero el problema / despues la herramienta.


![[./Recording 20240627171152.webm|Recording 20240627171152]]

Sobre redis:

- Leer los datos
- Formatear
- Escribirlos en redis.

sobre la 2.

- ids personas con notas > o igual 
- match de id -> nombres
- guardar nombres

cuando piden hacer raw queries es como redactarla en maria db


![[./Recording 20240627174050.webm|Recording 20240627174050]]

