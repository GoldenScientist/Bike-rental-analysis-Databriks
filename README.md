# Bike-rental-analysis-Databriks
Pypsark Databriks
run on https://community.cloud.databricks.com/login.html
dataset link : https://archive.ics.uci.edu/ml/datasets/Bike+Sharing+Dataset


2. Attributes on original data
-  season : season (1:springer, 2:summer, 3:fall, 4:winter)
- yr : year (0: 2011, 1:2012)
- mnth : month ( 1 to 12)
-  hr : hour (0 to 23)
- holiday : weather day is holiday or not (extracted from [Web Link])
- weekday : day of the week
-  workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
-  weathersit :
o 1: Clear, Few clouds, Partly cloudy, Partly cloudy
o 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
o 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain +
Scattered clouds
o 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
temp : Normalized temperature in Celsius. The values are derived via (tt_min)/(t_max-t_min), t_min=-8, t_max=+39 (only in hourly scale)
hum: Normalized humidity. The values are divided to 100 (max)
windspeed: Normalized wind speed. The values are divided to 67 (max)


You have been contacted to build a predictive model to help Bike Rental companies in
predicting the hourly and daily demand on bikes.
- Build a first linear model to predict the ‘demands’ and evaluate it (display
meanAbsoluteError and r2)
- Improve your model by doing cross validation. You shall tune and cross-validate the
model using:
pyspark.ml.Pipeline
pyspark.ml.tuning.ParamGridBuilder
pyspark.ml.tuning.CrossValidator
- Try to get some insights from the results you obtained:
o Display, for instance, the average real demand versus the average predicted
demand and the standard deviation of both by grouping your data by:
- hour
- season
other features that you think useful
- Add dummy variables to improve the accuracy of your model.
- Try other machine learning algorithms and compare. 
