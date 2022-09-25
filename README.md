# ClimatePrediction
A model that can predict the weather from each street in the metropolitan zone of Monterrey


## The input format is

['CO', 'DV', 'HR', 'NO', 'NO2', 'NOx', 'O3', 'PB', 'PM10', 'PM2.5', 'PP',
       'RS', 'SO2', 'TMP', 'VV']
       
These are the rows for the input, so you enter the input
```{python}
input = ['CO', 'DV', 'HR', 'NO', 'NO2', 'NOx', 'O3', 'PB', 'PM10', 'PM2.5', 'PP',
       'RS', 'SO2', 'TMP', 'VV']
       
pred = model(input, future= 100)
```

The future is the petition to have the next N hours of weather.
