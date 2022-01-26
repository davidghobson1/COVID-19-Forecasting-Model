# COVID-19-Forecasting-Model

An LSTM Model for forecasting COVID-19 cases, deaths, and recoveries in Ontario as a time series.

I developed this model as a part of the Carleton University AI Society's [Kaggle competition](https://www.kaggle.com/c/cais-x-t1-2021/overview) modelling COVID-19 data in Canada.

Although the datasets are rather small to properly train the NNs, this serves as an exploratory model to investigate LSTMs.

In addition to the competition datasets, I also added some more data to help with feature selection, including hospitalization rates and ICU admissions. That data can be found and downloaded freely from ESRI Canada [here](https://resources-covid19canada.hub.arcgis.com/datasets/provincial-daily-totals).

Many aspects of the notebook, especially setting up the time indows through the `WindowsGenerator` class are from [TensorFlow's tutorial on Time Series](https://www.tensorflow.org/tutorials/structured_data/time_series).
