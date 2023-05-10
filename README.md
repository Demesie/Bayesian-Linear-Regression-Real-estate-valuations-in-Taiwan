# Bayesian-Linear-Regression-Real-estate-valuations-in-Taiwan

This is a project(in progress)



## Abstract or Executive Summary

The goal of the project is to build a Bayesian linear regression predictive model that is able to predict price of real estate valuations properties in Taiwan. The unit of measurement for price of real estate valuations per unit area is given by  0000 New Taiwan Dollar/Ping where 1 Ping = $3.3m^2$. The projects aims to predict valuation of a house per unit area after accounting for age of the house(in years), distance to the nearest MRT station (in meter) and number of convenience stores in the living circle on foot (integer). Specifically, we are interested in if increasing any of the explanatory variables leads to the appreciation of the value of the property(both statistically and practically). To measure this, we will be performing one-sided hypothesis testing. Such a model is ideal for investors to determine appropriate valuations for investors interested in buying new properties in the Sindian District, New Taipei City. Additionally, the ability to predict price of real estate valuations per unit area allows renters to make informed decision on whether to hold or sell the property , rent or own a property. This project used 10-fold cross validation technique to measure the predictive accuracy of valuation of properties using weakly informative priors. We used mean absolute error(MAE) to measure model predictive accuracy. Using 10-fold CV estimates of posterior predictive accuracy model we found that the model mean absolute error is 4.90852. This means each of our prediction was with in 4.9 thousands of Taiwan dollar per unit area.  Hence, it tells how far off we are in-terms of predicting valuation of a house per unit area from the true valuation of a house per unit area. This mae  of 4.90852is quite well compared to mae of 10.7 by predicting average price for all observations.  The paper discusses in detail how the results were obtained, prior assumptions and posterior predictive accuracy and hypothesis testing for each of estimates in increasing evaluation of properties price per unit area in Taiwan. 



$\text{data: }$ $Y_i | \beta_0^C, \beta_1^C, \beta_2^C, \beta_3^C$  $\stackrel{ind}{\sim} N(\mu_i,\sigma^2 )$ \\


with  $\mu_i$ = $\beta_0$ + $\beta_1^C * age_i$ + $\beta_2^C * dMRT_i$ + $\beta_3^C * NCStore_i$

The priors:


$\beta_0 \sim N(m_0, s_0^2) = N(37.98,13.60649^2 )$

$\beta_1 \sim N(m_1, s_1^2) =  N(0, 0.2986^2)$

$\beta_2 \sim N(m_1, s_1^2) =  N(0, 0.0.0027^2)$


$\beta_3 \sim N(m_3, s_3^2) =  N(0, 1.1548^2)$


$\sigma \sim Exp(l) = Exp(0.073)$

