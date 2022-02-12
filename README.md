# Avocado-data-price-prediction

## Problem Statement:-
We're using the Avocado dataset from 2015, 2016, 2017, and 2018 to categorize Organic & Conventional Types and forecast the average price using a regression model.



Introduction
Avocado consumption data is included in the Avocado dataset, which spans the years 2015 to 2018. Avocados are offered in two varieties.




### <center>Data
| COLUMN | DATA TYPES |
| --- | --- |
| `DATE`            |   OBJECT |
| `AVERAGEPRICE`    |   FLOAT64 | 
| `TOTALVOLUME`     |   FLOAT64 |
| `SMALL`           |   FLOAT64 |
| `LARGE`           |   FLOAT64 |
| `XLARGE`          |   FLOAT64 |
| `TOTALBAGS`       |   FLOAT64 |
| `SMALLBAGS`       |   FLOAT64 |
| `LARGEBAGS`       |   FLOAT64 |
| `XLARGEBAGS`      |   FLOAT64 |
| `TYPE`            |   OBJECT |
| `YEAR`            |   INT64 |
| `REGION`	         |   OBJECT |

![Averageprice1.png](image/Averageprice1.png)

<b>Observations</b><br>
* There is a strong co-relation between TotalVolume Vs Small and TotalBags Vs SmallBags.
* We can say weak co-relation between TotalVolume Vs XLarge and TotalBags Vs XLargeBags.
* Large and LargeBags comes in the middle.

![3.png](image/3.png)

![7.JPG](image/7.JPG)

<b>Conclusion</b><br>
* Columns like Type of avocado, size and bags have impact on Average Price, __lesser the RMSE value__ accurate the model is, when we consider Small Hass in Small Bags.
* __Random forest Classifier__ has more accuracy than __Logistic regression__ model for this dataset , __accuracy is 0.99__ it may also denote it is overfitting as it even classifies the outliers perfectly.
* __Random forest classifier__ model predicts the type of Avocado more accurately than __Logistic regression__ model.
* __Random Forest Regressor__ model predicts the average price more accurately than __Linear regression__ model.<br>

[Notebook](AvocadoDataset.ipynb)

