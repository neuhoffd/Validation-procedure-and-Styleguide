# Reversible Jump Markov Chain Monte Carlo (RJMCMC) Sampler for Autoregressive Moving Average (ARMA) Time Series Models

This quantlet contains a small suite enabling the user to estimate ARMA time series models using Reversible Jump Markov Chain Monte Carlo (RJMCMC) (See e.g. Green 1995, Brooks and Ehlers 2003). RJMCMC enables the sampling from posteriors over not only the parameter space for a particular model, but also several models.

The sampler provided here assumes zero-mean stationary ARMA models with normal disturbances as in Neuhoff (2015) or Meyer-Gohde and Neuhoff (2015). The sampler settings and data source can be set in the file "getSettings.m". It is also possible to replace all prior distributions, proposal distributions, as well as the Likelihood functions via setting the appropriate function handles in this file. This framework can thus be also employed to estimate ARMA models with non-normal disturbances. Furthermore, any proposal distribution can be used. For further information please refer to the comments in "getSettings.m".

