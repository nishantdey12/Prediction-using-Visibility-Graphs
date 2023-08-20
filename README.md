# Prediction-using-Visibility-Graphs
Converting time series to visibility graphs using networkx and using it for prediction

The mathematics required to develop the code is obtained from the file "fpy-10-1029600.pdf". It is present in this repository. The code is written in jan recent.ipynb. The data used to do predict is given in 1981-2020 Wet Bulb Temperature. 

Here i have used temperature data over last 20 years(1981-2010) to predict temperature in next 10 years(2010-2020). However, the code needs to changed for every month. For example-if i want to predict the temperature for the month of january, i need to change the code to read the jan data in the pandas dataframe. It can be automated but it is not done here.

Errors range from as low as less than 1% to as high as 14-15%. However there is definite relation as to why that happens. 
