Hoy - Estadística: Test de hipótesis paramétricos. #estadística 

Actividad práctica:

Datos: personas que atienden en el call center:

Table:        N     X  DE    Failure     Vacation Week

Francisca  1320  3,54min  0,53  7,05%  26

Tomas  1320  4,56min  1,82 7,88%  29


| Nombre    | N    | $$ X $$  | DE   | Failure | Vacation Week |
| --------- | ---- | -------- | ---- | ------- | ------------- |
| Francisca | 1320 | 3,54 min | 0,53 | 7,05%   | 26            |
| Tomás     | 1320 | 4,56 min | 1,82 | 7,88%   | 29            |
"No nos importa quien sea mayor o menor, estamos estableciendo la diferencia"
Primero que todo planteamos la hipotesis nula

H0 = Xf = Xt

### Test de diferencia de medias T-Test###

#diferenciademedias
Hipótesis: 

$$T = X_1 - X_2 - 0/fra$$

Supuestos:

Las varianzas son iguales V21 = V22
X distribuye normal
Si sigma es conocido, distribuye normal:
Si sigma cuadrado no es conocido lo que tengo que realizar:

### T - Student ###

#t-student

T = X1 - X2 / Raiz de S cuadrado
 Tener en consideración que todo se determina con la muestra.

Tres formas para analizar la distribución:

	1. Si T(alpha) < T : Se rechaza H0
	2. P valor < alpha  P (X) > T(alpha)|H_0 = Se rechaza H0
	3. Intervalos de confianza (IC): Si el intervalo de confianza pasa por el 0 no puedo rechazar la hipótesis nula

 El T se compara con el numero objetivo en función de rechazar o no la hipótesis.
 Y puedo decretar una diferencia estadística significativa

Hay que comparar el valor de la normal con la tabla T, si el resultado de la t es mayor que...

Intervalos de confianza:
$$
IC = \frac{\hat{X}_1 - \hat{X}_2}{\sqrt{S^2 \left(\frac{1}{N} + \frac{1}{M}\right)}} \pm t_{\alpha} \cdot SE(\hat{X}_1 - \hat{X}_2)
$$
Hay que tener ojo con la conclusión, no solo se rechaza la nula, si no que hay un comportamiento resultado además de la interpretación estadística.

### Test de diferencia en proporciones ###

#diferenciadeproporciones

Es pensado en distribuciones binomiales.
Las muestras vienen de las mismas poblaciones

Es lo mismo de diferencia de medias pero con valores binomiales

¿Como distribuye? No se sabe cuando es para muestras pequeñas, cuando hay mucha muestra utiliza las propiedades de teoria asintotica distribuyendo (0,1)

N= es la sumatoria de ambas muestras

Se testea:
$$
X_1 = \frac{N}{\text{Total de casos}}
$$

$$ H_0 : P_1 = P_2 \longleftrightarrow p_1 - p_2 = 0 $$

Entonces

$$
\text{Var} = \frac{p(1-p)}{N}
$$

### Test de diferencia en varianzas o Test de fisher ###

#testdefisher
La hipótesis nula \( H_0 \) se expresa como:
$$
H_0: \sigma^2_{X1} = \sigma^2_{X2} \longleftrightarrow \frac{\sigma^2_{X1}}{\sigma^2_{X2}} = 1
$$
El estadístico \( T \) se calcula como:
$$
T = \frac{S^2_{X1}}{S^2_{X2}} = \frac{\frac{(n-1) s^2_{X1}}{\sigma^2_{X1}}}{\frac{(m-1) s^2_{X2}}{\sigma^2_{X2}}}
$$
La razón de dos variables chi cuadrado distribuye una distribución F de la siguiente manera:
$$
\frac{\chi^2_{n-1}/(n-1)}{\chi^2_{m-1}/(m-1)} \sim F_{n-1, m-1}
$$

Averiguar sobre los test de normalidad

### Test de Kolmogrov - Smirnov (Conocido como KS) ###

#kolmogrovsmirnov

Es un test no paramétrico, no testea un parametro, testea una distribución
Esta hecho para comparar si dos distribuciones empiricas son iguales

Lo que me interesa es la curva, la distribución completa

Es util para analizar por categorías de formas descriptivas

**En sciklearn es kscore**

Si el ks score es muy alto 

¿Como se hace?

Estadístico:
$$
D_{n,m} = \sup_x |F_{1,n}(x) - F_{2,m}(x)|
$$


Esto analiza las diferencias dentro de la distribución.

Rechazo H0 Si :
$$
D_{n,m} > c_{\alpha} \cdot \sqrt{\frac{n+m}{nm}}
$$

 C(alpha) =
$$
C(\alpha) = \sqrt{-\ln\left(\frac{\alpha}{2}\right)} \cdot \frac{1}{2}
$$

#pruebasparamétricas
#pruebasnoparamétricas
