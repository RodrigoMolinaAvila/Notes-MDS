Aquí está el contenido completo del documento que combina las tres instancias de fórmulas y conceptos de estadística que me has proporcionado:

---

### Fundamentos de Probabilidad
- **Función de Distribución Acumulativa Normal:** \( \Phi\left(\frac{x - \mu}{\sigma}\right) \)
- **Probabilidad de Eventos Independientes:** \( (0.5)^{10} \)
- **Modelo de Regresión Lineal para Esperanza Condicional:** \( E(GPA|SAT) = 0.70 + 0.002 \times SAT \)

### Estimadores y Teoría Asintótica
- **Esperanza y Varianza de Estimadores:**
  - \( E(W_1) = \left(\frac{n-1}{n}\right) \overline{Y} \)
  - \( E(W_2) = \frac{\overline{Y}}{2} \)
  - \( \text{Var}(W_1) = \left(\frac{n-1}{n}\right)^2 \frac{\sigma^2}{n} \)
  - \( \text{Var}(W_2) = \frac{1}{4} \frac{\sigma^2}{n} \)
- **Estimación de Parámetro por Razón:**
  - \( Z = \frac{Y}{X} \)
  - \( E(Z) = \theta \)
  - \( W_1 = \frac{1}{n} \sum_{i=1}^n \frac{Y_i}{X_i} \)
  - \( W_2 = \frac{\overline{Y}}{\overline{X}} \)
- **Estimación de Razón Probabilística:** \( G = \frac{\overline{Y}}{1-\overline{Y}} \)

### Test de Hipótesis
- **Intervalo de Confianza para Proporciones:** \( \hat{p} \pm z \times \sqrt{\frac{\hat{p}(1 - \hat{p})}{n}} \)
- **Estadístico t para Pruebas de Hipótesis:** \( t = \frac{\overline{y} - \mu_0}{s/\sqrt{n}} \)
- **Intervalo de Confianza y Valor-p para Diferencias de Medias:**
  - \( \overline{D} \pm t \times \frac{s_D}{\sqrt{n}} \)
  - \( p\text{-valor} = 2 \times (1 - \Phi(|t|)) \)

### Test de Hipótesis Conjuntas
- **Test de Hipótesis Conjuntas:** \( H_0: \beta_1 = 0 \land \beta_2 + \beta_3 = 1 \)

### Intervalos de Confianza Avanzados
- **Intervalo de Confianza para Diferencias:** \( IC = \frac{\hat{X}_1 - \hat{X}_2}{\sqrt{S^2 \left(\frac{1}{N} + \frac{1}{M}\right)}} \pm t_{\alpha} \cdot SE(\hat{X}_1 - \hat{X}_2) \)

### Test de Diferencia en Varianzas (Test de Fisher)
- **Test de Fisher:** \( H_0: \sigma^2_{X1} = \sigma^2_{X2} \)

### Kolmogorov-Smirnov Score
- **Kolmogorov-Smirnov Score:** \( D_{n,m} = \sup_x |F_{1,n}(x) - F_{2,m}(x)| \)
- **Criterio de Rechazo:** \( D_{n,m} > c_{\alpha} \cdot \sqrt{\frac{n+m}{nm}} \)

### Repaso Test de Hipótesis
- **Trade-off Sesgo-Varianza:** \( MSE = \text{Sesgo}^2 + \text{varianza} + \text{Error} \)
- **Test de Hipótesis General:** \( H_0 : B_x - B_y = c \)

### Diferencia de Medias y Proporciones
- **Test de Diferencia de Medias:** \( E = \frac{({\hat{X} - \hat{Y}) - (\mu_x - \mu_y)}}{\sqrt{\frac{\sigma^2}{n} + \frac{1}{m}}} \)
- **Diferencia de Proporciones:** \( E = \frac{({\hat{p}_x - \hat{p}_y) - (

p_x - p_y)}}{\sqrt{\hat{p}(1-\hat{p})\left (\frac{1}{m} + \frac{1}{n}\right)}} \)

### ANOVA
- **ANOVA Model:** \( Y_{ij} = \mu + \alpha_i + e_{ij} \)

Este documento compendia todas las fórmulas y conceptos que hemos discutido, organizados de manera clara para facilitar la referencia y el estudio.