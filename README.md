# Bronze Solution (top 9%) for Kaggle M5 Forecasting Competition

The Competition Page <https://www.kaggle.com/c/m5-forecasting-accuracy/>

## Summary

+ Horizon: future 28 days (1942 - 1969)

+ FE
    + date-related features
    + price features
    + target encoding
    + lag and rolling mean

+ CV strategy
    + time series split 3 fold cv
        + last 56 days in the training set (1886 - 1941)
        + 28 days in the historical period (1578 - 1605)
    + recursive predicting score as real valid score; avoid data leak
    + feature selection when the scores improve simultaneously and have the minimal STD

+ To be improved
    + ensemble from different models
    + post-processing based on historical trend
    + custom loss

# Thank you!
