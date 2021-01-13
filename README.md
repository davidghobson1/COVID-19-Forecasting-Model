# COVID-19-Forecasting-Model

An LSTM Model for forecasting COVID-19 cases, deaths, and recoveries in Ontario as a time series.

I developed this model as a part of the Carleton AI Society's [Kaggle competition](https://www.kaggle.com/c/cais-x-t1-2021/overview) modelling COVID-19 data in Canada.

I originally started off working wiht models based on scikit-learn's DecisionTrees... That is, until I realized 
1. scikit-learn's DecisionTree implementation can't handle categorical data...

but more importantly 

2. [Decision trees aren't good at data extrapolation](https://www.kaggle.com/c/web-traffic-time-series-forecasting/discussion/38352) anyways...

So this is my attempt to apply a more suitable model framework to the problem. 

**Please note** that the **overall framework I use** to deal with time lags and input windows is **directly based on [TensorFlow's tutorial on Time Series](https://www.tensorflow.org/tutorials/structured_data/time_series)**! It is not my original work and nor do I take credit for it! But it's suitability for the problem, not to mention its elegance and ease of use were the reasons I choose to use it. (Instead of having to re-invent the wheel... Plus, it's one heck of a great tutorial!). For the full code from the original tutorial please see the link above.

In addition to the competition datasets, I also added some more data to help with feature selection, including hospitalization rates and ICU admissions.
That data can be found and downloaded freely from ESRI Canada [here](https://resources-covid19canada.hub.arcgis.com/datasets/provincial-daily-totals).
