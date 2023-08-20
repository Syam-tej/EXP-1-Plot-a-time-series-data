## EXP-1-Plot-a-time-series-data
## AIM:
Develop a python program to Plot a time series data (population/ market price of a commodity /temperature.
## ALGORITHM:
## STEP 1: 
Import the required packages like pandas and numpy
## STEP 2: 
Read the data using the pandas
## STEP 3: 
Calculate the mean for the respective column.
## STEP 4: 
Plot the data according to need and can be altered monthly, or yearly.
## STEP 5: 
Display the results.
## PROGRAM:
## DEVELOPED BY : P SYAM TEJ
## REF NO: 212221240056
```
import matplotlib.pyplot as plt
import pandas as pd
df=pd.read_csv("Dataset.csv",parse_dates=["Date"],index_col="Date")
df.head()
df["2022-01"]
df["2022-01"].Close.mean()
df["2022-04-01":"2022-07-31"]
df.Close.resample('M').mean()
mean=df.Close.resample('M').mean().plot(kind="bar")
mean=df.Close.resample('Y').mean().plot(kind="bar")
```
## OUTPUT:
## FIRST FIVE ROWS:
![image](https://github.com/Syam-tej/EXP-1-Plot-a-time-series-data/assets/93427224/a683d975-99a1-4492-8c49-4dc55e2a97bf)
## CALCULATING MEAN:
![image](https://github.com/Syam-tej/EXP-1-Plot-a-time-series-data/assets/93427224/8ecf6d96-3a31-455a-b79d-06b7186a5e1e)
## PLOTTING BAR GRAPH(MONTHLY):
![image](https://github.com/Syam-tej/EXP-1-Plot-a-time-series-data/assets/93427224/6ec20103-4a67-40b8-9eb6-c61b009db030)
## PLOTING BAR GRAPH(YEARLY):
![image](https://github.com/Syam-tej/EXP-1-Plot-a-time-series-data/assets/93427224/e34d281f-9228-443b-a413-dd7973a20966)

## RESULT:
Thus we have created the python code for plotting the time series of given data.
