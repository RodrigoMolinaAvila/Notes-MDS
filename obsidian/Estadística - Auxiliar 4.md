Repaso test de hipótesis: #testdehipótesis 

Trade-off sesgo varianza:

Busca equilibrar la disminución del sesgo y la varianza.

MSE: Propiedad de estimadores #mínimoscuadrados 
$$ MSE = Sesgo^2 + varianza + Error $$

Un modelo predictor se puede interpretar como un estimador.
Random forest se utiliza para casos binarios  **** #randomforest


Test de hipótesis: se define como herramienta de comparación de dos muestras. #testdehipótesis 

$$ H_0 : B_x - B_y = c $$
$$ H_a: \beta_x b_y \neq c $$
$$ b_x - b_y > c $$
$$ b_x - b_y < c $$
La muestra se divide en segmentos: 
- Región de aceptación (aceptance)
- Región de rechazo (regection)

P-values: Si la probabilidad es mejor al nivel de significancia. se rechaza H_0, el valor de significancia se evalua en Z (el mejor o igual depende de la hipótesis planteada) #p-values 
$$ P(Z < E) $$
Intervalos de confianza: Es un mecanismo para rechazar la H_0 Si el intervalo asociado al test no se encuentra el valor objetivo, se rechaza H_0, el valor de significancia se valua fuera de Z.

En python se usa con la implementación del P-Valor

Test de diferencia de medias: #diferenciademedias 
$$ E = \frac{({\hat{X} - \hat{Y}) - (\mu_x - \mu_y)}}{\sqrt{\frac{\sigma^2}{n} + \frac{1}{m}}} $$
Si no conocemos: ver el documento.

Diferencia de proporciones: #diferenciadeproporciones 
$$ E = \frac{({\hat{p}_x - \hat{p}_y) - (p_x - p_y)}}{\sqrt{\hat{p}(1-\hat{p})\left (\frac{1}{m} + \frac{1}{n}\right)}} $$
Simplificado cuando no tenemos Y:
$$ E = \frac{{\hat{p} - p}}{\sqrt{\hat{p}(1-\hat{p})/n}} $$
Para definir valores:
$$ p_x = \frac{x}{n},
p_y = \frac{y}{m},
\hat{p} = \frac{x+y}{n+m}
$$

ANOVA: Compara más de dos medias Yij es la observación de la entidad J en un grupo i, eij es el error aleatorio. #anova
$$ Y_{ij} = \mu + \alpha_i + e_{ij}$$
Mustestra la distinción de nuestras variables definidas en conjuntos, las cuales son diferentes a 0

Prueba Kolmogrov-Smirnov: Indica que la distribuciones son o no distintos. #kolmogrovsmirnov 

Sobre el auxilar 4:

Procedimientos para responder las preguntas: #consejos 

- Identificamos los parametros dados.
- Establecemos las hipótesis (en formula matemática) se define la cola en función si es mayor o menor.
- Establecemos la significancia dada
- Calcular estadístico
- Evaluamos el resultado
- Interpretamos en función del indice entregado con las hipótesis. ojo: responder en función de la pregunta planteada en el problema.

![[./Recording 20240410161606.webm|Recording 20240410161606]]