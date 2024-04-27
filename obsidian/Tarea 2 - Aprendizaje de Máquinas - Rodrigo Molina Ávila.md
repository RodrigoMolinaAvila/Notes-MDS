P1 - Bayes
Objetivo del problema:
Estimar el número de personas que NO tienen la enfermedad a pesar de haber sido diagnosticadas como positivas, es decir, calcular $$P(EN|TP)$$Definiciones:
- **EN (Enfermedad Negativa):** La persona no tiene la enfermedad.
- **EP (Enfermedad Positiva):** La persona tiene la enfermedad.
- **TN (Test Negativo):** El resultado del test es negativo.
- **TP (Test Positivo):** El resultado del test es positivo.

 Datos Conocidos:
- **Sensibilidad P(TP|EP):** Tasa de verdaderos positivos, igual a la especificidad dado el supuesto de simetría del test.
- **Especificidad \P(TN|EN)\:** Tasa de verdaderos negativos.
- **Prevalencia P(EP):** Probabilidad de tener la enfermedad. Conocida, 
- **Número de resultados positivos P(TP):** Se han registrado 10,000 resultados positivos.

A) Utilizamos el teorema de Bayes para calcular la probabilidad condicional de no tener la enfermedad dado un resultado de test positivo: $$
P(EN|TP) = \frac{P(TP|EN) \times P(EN)}{P(TP)}
$$Consideramos que la tasa de falsos positivos es el complemento de la especificidad:
$$
P(TP|EN) = 1 - P(TN|EN) = 1 - P(TP|EP)
$$
El modelo bayesiano queda:$$ P(EN|TP) = \frac{(1 - P(TN|EN)) \cdot P(EN)}{P(TP)} $$Utilizamos al ley de probabilidades totales para calcular la probabilidad de obtener un resultado positivo en el test:
$$
P(TP) = P(TP|EP)  P(EP) + P(TP|EN)  P(EN)
$$
B) Consideramos:
- Sensibilidad y especificidad = 95% 
- La prevalencia de la enfermedad es de 1 en 10,000 = 0.0001

Calculamos:
$$
P(TP) = 0.95 \times 0.0001 + 0.05 \times 0.9999 = 0.05009
$$
Nuestro modelo bayesiano:$$
P(EN|TP) = \frac{P(TP|EN) \times P(EN)}{P(TP)}
$$ Reemplazamos con los valores conocidos:
$$
P(EN|TP) = \frac{0.05 \times 0.9999}{0.05009} \approx 0.9981
$$
Esto significa que aproximadamente el 99.81% de las personas que obtienen un resultado positivo en el test realmente no tienen la enfermedad.

Ahora aplicamos con una sensibilidad de un 50%:

Consideramos:
- Sensibilidad y especificidad = 50%
- La prevalencia de la enfermedad es de 1 en 10,000 = 0.0001

Calculamos:
$$
P(TP) = 0.50 \times 0.0001 + 0.50 \times 0.9999 = 0.50005
$$
Nuestro modelo bayesiano:
$$
P(EN|TP) = \frac{P(TP|EN) \times P(EN)}{P(TP)}
$$
Reemplazamos con los valores conocidos:
$$
P(EN|TP) = \frac{0.50 \times 0.9999}{0.50005} \approx 0.9998
$$
Esto significa que aproximadamente el 99.98% de las personas que obtienen un resultado positivo en el test realmente no tienen la enfermedad cuando la sensibilidad es del 50%.

C) Investigue la diferencia entre el paradigma "frecuentista" y "Bayesiano" al interpretar las probabilidades:

La diferencia principal entre las interpretaciones frecuentista y bayesiana de la probabilidad radica en cómo se percibe la incertidumbre y el conocimiento previo:

Frecuentista: En el enfoque frecuentista, las probabilidades se interpretan como frecuencias a largo plazo de eventos. Se enfoca en la evidencia obtenida a partir de experimentos o estudios repetidos y no incorpora conocimiento previo en el análisis. Es decir, se busca establecer conclusiones a partir de la frecuencia observada de los datos, y se utilizan estimaciones puntuales con intervalos de confianza para inferir parámetros desconocidos.

Bayesiano: El enfoque bayesiano utiliza probabilidades para representar el grado de creencia o confianza en una hipótesis, y actualiza estas creencias a medida que se dispone de nueva información (datos observados). Esto se logra a través del teorema de Bayes, que permite revisar y ajustar las probabilidades previas en base a los datos recientes, proporcionando una distribución posterior. 

La elección entre las interpretaciones frecuentista y bayesiana dependerá de cómo se desea interpretar los resultados.

P2 - MLE con una Bernoulli

Para la distribución de probabilidad de Bernoulli, la probabilidad de obtener un resultado específico es:
$$
P(X = x) = \lambda^x (1 - \lambda)^{1-x}
$$
Donde \(x\) toma el valor de 1 para cara y 0 para sello, y \(\lambda\) es la probabilidad de obtener cara.

A)

Con una muestra de datos (D ={x_1, ..., x_n}), la función de máxima verosimilitud (L(lambda|D)) es:
$$
L(\lambda|D) = \prod_{i=1}^{n} \lambda^{x_i} (1 - \lambda)^{1-x_i}
$$
Aplicando logaritmo para simplificar la multiplicación a suma, obtenemos la log-verosimilitud:
$$
\log(L(\lambda|D)) = \sum_{i=1}^{n} [x_i \log(\lambda) + (1 - x_i) \log(1 - \lambda)]
$$
B)

Derivando esta función con respecto a \(\lambda\) y estableciendo la derivada igual a cero encontramos el MLE de \(\lambda\):
$$
\frac{d}{d\lambda} \log(L(\lambda|D)) = \sum_{i=1}^{n} \left[\frac{x_i}{\lambda} - \frac{1 - x_i}{1 - \lambda}\right] = 0
$$
Simplificando, el estimador de máxima verosimilitud para \( \lambda \) es:
$$
\hat{\lambda} = \frac{\sum_{i=1}^{n} x_i}{n}
$$
Este es el promedio de caras observadas, donde \(x_i\) representa la cantidad de caras en el experimento \(i\), y \(n\) es el número total de experimentos.


