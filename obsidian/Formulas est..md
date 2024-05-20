Fundamentos de Probabilidad
- **Función de Distribución Acumulativa Normal:** `Φ((x - μ)/σ)`
- **Probabilidad de Eventos Independientes:** `(0.5)^10`
- **Modelo de Regresión Lineal para Esperanza Condicional:** `E(GPA|SAT) = 0.70 + 0.002 * SAT`
 Estimadores y Teoría Asintótica
 Esperanza y Varianza de Estimadores
- `E(W₁) = ((n-1)/n) * Ȳ`
- `E(W₂) = Ȳ / 2`
- `Var(W₁) = ((n-1)/n)^2 * (σ²/n)`
- `Var(W₂) = 1/4 * (σ²/n)`
Estimación de Parámetro por Razón
- `Z = Y / X`
- `E(Z) = θ`
- `W₁ = (1/n) * Σ (Yᵢ / Xᵢ) from i=1 to n`
- `W₂ = Ȳ / X̄`
Estimación de Razón Probabilística
- `G = Ȳ / (1 - Ȳ)`
Test de Hipótesis
Intervalo de Confianza para Proporciones
- `p̂ ± z * sqrt((p̂(1 - p̂))/n)`
Estadístico t para Pruebas de Hipótesis
- `t = (ȳ - μ₀) / (s/√n)`
Intervalo de Confianza y Valor-p para Diferencias de Medias
- `D̄ ± t * (s_D/√n)`
- `p-value = 2 * (1 - Φ(|t|))`
Test de Hipótesis Conjuntas
- `H₀: β₁ = 0 ∧ β₂ + β₃ = 1`
Intervalos de Confianza Avanzados
- `IC = ((X̂₁ - X̂₂) / √(S² * (1/N + 1/M))) ± tᵦ * SE(X̂₁ - X̂₂)`
Test de Diferencia en Varianzas (Test de Fisher)
- `H₀: σ²ₓ₁ = σ²ₓ₂ ↔ σ²ₓ₁/σ²ₓ₂ = 1`
Kolmogorov-Smirnov Score
- `Dₙ,ₘ = supₓ |F₁,ₙ(x) - F₂,ₘ(x)|`
- `Reject H₀ if: Dₙ,ₘ > cᵦ * √((n+m)/nm)`
Repaso Test de Hipótesis
- **Trade-off Sesgo-Varianza:** `MSE = Bias² + Variance + Error`
- **Test de Hipótesis General:** `H₀: Bₓ - Bᵧ = c`
Diferencia de Medias y Proporciones
- **Test de Diferencia de Medias:** `E = ((X̂ - Ŷ) - (μₓ - μᵧ)) / √(σ²/n + 1/m)`
- **Diferencia de Proporciones:** `E = ((p̂ₓ - p̂ᵧ) - (pₓ - pᵧ)) / √(p̂(1-p̂)(1/m + 1/n))`
ANOVA
- **ANOVA Model:** `Yᵢⱼ = μ + αᵢ + eᵢⱼ`
