## EXP-1-Plot-a-time-series-data
## AIM:
Develop a python program to Plot a time series data (population/ market price of a commodity /temperature.
## ALGORITHM:
STEP 1: Import the required packages like pandas and numpy
STEP 2: Read the data using the pandas
STEP 3: Calculate the mean for the respective column.
STEP 4: Plot the data according to need and can be altered monthly, or yearly.
STEP 5: Display the results.
## PROGRAM:
DEVELOPED BY : P SYAM TEJ
REF NO: 212221240056
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
```
https://user-images.githubusercontent.com/93427264/261806643-966e903b-c051-4846-bf0a-278477394d6a.png
```
## CALCULATING MEAN:
```
https://user-images.githubusercontent.com/93427264/261806659-952c90de-b90f-4000-8075-4c973d13bc0e.png
```
## PLOTTING BAR GRAPH(MONTHLY):
```
https://user-images.githubusercontent.com/93427264/261806670-db848b6d-d98d-4f87-829b-d2ba877a3afc.png
```
## PLOTING BAR GRAPH(YEARLY):
```
https://user-images.githubusercontent.com/93427264/261806698-16f7788b-75ec-4dfa-b2b5-80db53d52a09.png
```
## RESULT:
```
Thus we have created the python code for plotting the time series of given data.
```
