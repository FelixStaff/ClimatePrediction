# ClimatePrediction
A model that can predict the weather from each street in the metropolitan zone of Monterrey

## Load the model

First, you need to have the ModelApodaca4.2.pt in the path Model/ModelApodaca4.2.pt
And have the architecture of the Net, then specify the arguments and make the comand
```{python}
model = Net(arguments**)
model.load_state_dict(torch.load("Model/ModelApodaca4.2.pt))
```
And the model will be charged
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
