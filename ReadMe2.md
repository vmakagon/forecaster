# Predict rain in 49 regions in Australia.

## Abstract.
This dataset contains daily weather observations from numerous Australian weather stations.
Predict whether or not it will rain tomorrow by training a binary classification model.
The target variable RainTomorrow means: Did it rain the next day? Yes (1) or No (0).

Numerical Weather Prediction (NWP) data are the form of weather model data we are most familiar with on a day-to-day basis. NWP focuses on taking current observations of weather and processing these data with computer models to forecast the future state of weather.

## Features in dataset:
    Date: The date of observation
    Location: The common name of the location of the weather station
    MinTemp: The minimum temperature in degrees celsius
    MaxTemp: The maximum temperature in degrees celsius
    Rainfall: The amount of rainfall recorded for the day in mm
    Evaporation: The so-called Class A pan evaporation (mm) in the 24 hours to 9am
    Sunshine: The number of hours of bright sunshine in the day.
    WindGustDir: The direction of the strongest wind gust in the 24 hours to midnight
    WindGustSpeed: The speed (km/h) of the strongest wind gust in the 24 hours to midnight
    WindDir9am: Direction of the wind at 9am
    WindDir3pm: Direction of the wind at 3pm
    WindSpeed9am: Wind speed (km/hr) averaged over 10 minutes prior to 9am
    WindSpeed3pm: Wind speed (km/hr) averaged over 10 minutes prior to 3pm
    Humidity9am: Humidity (percent) at 9am
    Humidity3pm: Humidity (percent) at 3pm
    Pressure9am: Atmospheric pressure (hpa) reduced to mean sea level at 9am
    Pressure3pm: Atmospheric pressure (hpa) reduced to mean sea level at 3pm
    Cloud9am: Fraction of sky obscured by cloud at 9am. This is measured in "oktas", which are a unit of eigths. It records how many eigths of the sky are obscured by cloud. A 0 measure indicates completely clear sky whilst an 8 indicates that it is completely overcast.
    Cloud3pm: Fraction of sky obscured by cloud (in "oktas": eighths) at 3pm. See Cload9am for a description of the values
    Temp9am: Temperature (degrees C) at 9am
    Temp3pm: Temperature (degrees C) at 3pm
    RainToday: Boolean: 1 if precipitation (mm) in the 24 hours to 9am exceeds 1mm, otherwise 0
    RISK_MM: The amount of next day rain in mm.
    RainTomorrow: The target variable. Did it rain tomorrow?

## Questions&problems:
+ There are a lot of missing values for some important features. How to fill them?
+ We need to group in regions, find clusters and add as variable. We can not treat all regions as one.
+ RISK_MM needs to be dropped? It is the same as RainTomorrow
+ Global warming affect. Does we have it over 7 years observations?
+ We need to formulate the conditions for hight probability of rain with most important features.
+ It is good to  predict temperature, rain in mm, wind speed, Sunshine for each region/cluster
+ How well we predict rain for 1 day, 3 days or 1 week time (probability)? Byes method for next day

## Further exploration

+
