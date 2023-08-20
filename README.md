# Prediction-using-Visibility-Graphs
Converting time series to visibility graphs using networkx and using it for prediction

The mathematics required to develop the code is obtained from the file "fpy-10-1029600.pdf". It is present in this repository. The code is written in jan recent.ipynb. The data used to do predict is given in 1981-2020 Wet Bulb Temperature. 

Here i have used temperature data over last 20 years(1981-2010) to predict temperature in next 10 years(2010-2020). However, the code needs to changed for every month. For example-if i want to predict the temperature for the month of january, i need to change the code to read the jan data in the pandas dataframe. It can be automated but it is not done here.

Errors range from as low as less than 1% to as high as 14-15%. However there is definite relation as to why that happens. 
![feb 2020](https://github.com/nishantdey12/Prediction-using-Visibility-Graphs/assets/97585193/022d00c1-76c7-44f8-9976-46c5ffae2b62)

Look at this visibility graph for the month of february for 40 years (1981-2020). Can you see the heavy clustering at the node 35? That year had abnormally high temperature as compared to other years. 

![MAY](https://github.com/nishantdey12/Prediction-using-Visibility-Graphs/assets/97585193/9495d818-9c2a-42e7-b812-6317cca78e71)

Now look at this. This doesnot have any such clustering as seen in the previous example. This is the visibility graph for the month of May for last 40 years.
Whenever high density nodes are formed, errors in predictions have sky-rocketed. These features are called communities. Some care must be taken to account for these communities, but i have not done any such thing. You are welcome to try and fix it.

this method can even be used to predict number of cases in pandemic. Based on data of number of daily active cases of coronavirus in state of West bengal, India. it does give sufficiently good results.

The results have been attached in the excel files.
