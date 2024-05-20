Test de hipótesis conjuntas: #testdehipótesisconjuntas
Se plantean de la siguiente forma:
$$ H_0 = \beta_1 = 0 \land \beta_2 + \beta_3 = 1  $$

Rechazar la hipótesis nula en estos casos significa rechazar una de las hipótesis nulas planteadas.

Cuando se usa?
Cuando tengo muchos subgrupos para testear al mismo tiempo.

Que gráficos se utilizan para observar los valores? 
Los gráficos de boxplots y violinplots.

Boxplots: #boxplots
Se utilizan para describir las frecuencias de la muestra de varios grupos. Se aprecia como se distribuye una variable en sus diferentes categorías.

Entrega un "ancho" de sus estadísticos descriptivos.

Hay que ver cual es la categoría que distribuye de forma distinta para encontrar el parámetro que pudiese alterar el test de hipótesis.

Anova: Analysis of Variance #anova 

Analiza la varianza de los intra-grupos dentro de los inter-grupos.
Test de hipótesis conjunta para distintos grupos.

Se hace el experimento en:
$$ I = Grupos $$
y $$J = Observaciones $$
Entonces: $$ Y_(ij) : medición de la persona (j) en el grupo (i) $$
Donde: $$Y_{ij} = \mu + \alpha_i + e_{ij}$$
Mu = media poblacional natural
Alpha_i = efecto por ser del grupo i
E_ij = Error aleatorio "no observable"

E_ij : iid
E(E_ij) = 0
Var (Eij) = Sigma cuadrado_e
... incompleto.

Entonces la hipótesis se redacta:
$$H_0: \sum \alpha_i = 0$$
El analisis de varianza se trata de:
$$\hat{Y}_{..} = \frac{1}{I} \cdot \frac{1}{J} \cdot \sum_{i=1}^{I} \sum_{j=1}^{J} Y_{ij}$$
Existen dos tipos de dispersión:
$$\sum_{i} \sum_{j} (Y_{ij} - \hat{Y}_{i.})^2 + \sum_{i} \sum_{j} (\hat{Y}_{j.} - \hat{Y}_{..})^2$$

Dispersión intra-grupos: (SSW) #dispersionintra-grupos$$\sum_{i} \sum_{j} (Y_{ij} - \hat{Y}_{i.})^2 $$ Dispersión inter-grupos: (SSB) #dispersióninter-grupos$$ \sum_{i} \sum_{j} (\hat{Y}_{j.} - \hat{Y}_{..})^2$$
Procedimientos del estadístico:
- Estimar SSW
- Estimar SSB
- Testeo la diferencia entre ellos

Entonces:
1) $$ S_p^2 = \frac{SSW}{I(J-1)} \sim \chi^2_{i}(J-1) $$
2) 
$$ \frac{SSB}{i-1} \sim \chi^2_{i-1}, \text{ solo si } \alpha_i = 0 $$
3) $$ F_{(i-1), i(j-1)} $$
Entonces para el ANOVA: $$ Y_{ijk} = \mu + \alpha_i + \beta_j + f_{ij} + e_{ijk} $$
¿Que se concluye al rechazar ANOVA de una vía?

Que al menos una de las medias es distinta a otras significativamente.

ANOVA de dos vías: #anova2vías

Cuando se interpreta los gráficos hay que ver el paralelismo de la distribución de las medias.

Existe un paradigma diferencial entre la interpretación estadistica vs la interpretación de ciencia de datos
![[./Recording 20240411155517.webm|Recording 20240411155517]]




