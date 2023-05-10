# Bayesian-Linear-Regression-Real-estate-valuations-in-Taiwan

This is a project(in progress)


$\text{data: }$ $Y_i | \beta_0^C, \beta_1^C, \beta_2^C, \beta_3^C$  $\stackrel{ind}{\sim} N(\mu_i,\sigma^2 )$ \\


$\text{ with }$ $\mu_i = \beta_0 + \beta_1^C*age_i + \beta_2^C*dMRT_i$ + $\beta_3^C*NCStore_i$

The priors:


$\beta_0 \sim N(m_0, s_0^2) = N(37.98,13.60649^2 )$

$\beta_1 \sim N(m_1, s_1^2) =  N(0, 0.2986^2)$

$\beta_2 \sim N(m_1, s_1^2) =  N(0, 0.0.0027^2)$


$\beta_3 \sim N(m_3, s_3^2) =  N(0, 1.1548^2)$


$\sigma \sim Exp(l) = Exp(0.073)$

