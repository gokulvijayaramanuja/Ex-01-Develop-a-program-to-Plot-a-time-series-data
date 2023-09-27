# Ex 01 Develop a program to Plot a time series data (population/ market price of a commodity /temperature .
## AIM:
To Write a Program to Plot a timeseries data market price of a commodity

## Equipments Required:
Hardware – PCs
Anaconda – Python 3.7 Installation / Jupyter notebook
## Procedure:
import the matplotlib.pyplot and pandas
read the datasets using pandas
calculate the mean for dataset
Plot the data according to need and can be altered monthly, or yearly.
## Program:
```
/*
Plot a timeseries data  market price of a commodity 
Developed by: GOKUL VIJAYA RAMANUJA P
RegisterNumber:  212222240030
*/

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
## Output:

### df.head()
![261832324-a683d975-99a1-4492-8c49-4dc55e2a97bf](https://github.com/gokulvijayaramanuja/Ex-01-Develop-a-program-to-Plot-a-time-series-data/assets/119577543/96113f7c-2ce7-4298-8e38-3797d23bb35e)

### Mean
![261832330-8ecf6d96-3a31-455a-b79d-06b7186a5e1e](https://github.com/gokulvijayaramanuja/Ex-01-Develop-a-program-to-Plot-a-time-series-data/assets/119577543/0aa992ac-d195-4b03-9a14-4ba4c06e52f5)

### Monthly Graph
![261832342-6ec20103-4a67-40b8-9eb6-c61b009db030](https://github.com/gokulvijayaramanuja/Ex-01-Develop-a-program-to-Plot-a-time-series-data/assets/119577543/e293781e-9b30-43c0-ab15-31350c493bc4)

### Yearly Graph
![261832269-e34d281f-9228-443b-a413-dd7973a20966](https://github.com/gokulvijayaramanuja/Ex-01-Develop-a-program-to-Plot-a-time-series-data/assets/119577543/d76fbbc3-605c-4641-9e2e-7c289b480616)

## Result:
Thus the program to implement to Plot a timeseries data market price of a commodity is written and verified using python programming.
