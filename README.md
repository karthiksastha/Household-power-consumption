# Household-power-consumption
Power outage accidents will cause huge economic loss to the social economy. Therefore, it is very important to predict power consumption.
Given the rise of smart electricity meters and the wide adoption of electricity generation technology like solar panels, there is a wealth of electricity usage data available.

Download dataset:
https://archive.ics.uci.edu/ml/machine-learning-databases/00235/household_power_consumption.zip

Problem Statement :
Given that power consumption data for the previous week, we have to predict the power consumption for the next week.

Dataset Description:
The data was collected between December 2006 and November 2010 and observations of power consumption within the household were collected every minute.

It is a multivariate series comprised of seven variables
global_active_power: The total active power consumed by the household (kilowatts).
global_reactive_power: The total reactive power consumed by the household (kilowatts).
voltage: Average voltage (volts).
global_intensity: Average current intensity (amps).
sub_metering_1: Active energy for kitchen (watt-hours of active energy).
sub_metering_2: Active energy for laundry (watt-hours of active energy).
sub_metering_3: Active energy for climate control systems (watt-hours of active energy).
This data represents a multivariate time series of power-related variables that in turn could be used to model and even forecast future electricity consumption

Time-series predictions play a major role in machine learning which is often neglected. Nonetheless, there are lots of machine learning algorithms we could use for these problems. The major machine learning algorithms involving Statsmodels and Econometric models etc. Today we will take a look at how to use and apply Deep learning algorithms to predict the time series Data

Why use a Deep Learning Algorithm?
With the data volume growing enormous day by day we shouldn’t confine ourselves to only the standard ML algorithms. Deep learning algorithms help us to handle large volumes of data and without leaving the key insights and by tuning the model within the right way gives us the maximum yield i.e., in our cause maximum accuracy . The model also determines if our prediction is better or worse from its own neural network architecture.

For this Time series forecasting we will use Long- Short Term Memory unit (LSTM).

Recurrent Neural Network (RNN)
To understand an LSTM Network, we need to understand a Recurrent Neural Network first. This kind of network is used to recognize patterns when past results have influence on the present result. An example of RNN usage is the time-series functions, in which the data order is extremely important. In this network architecture, the neuron uses as input not only the regular input (the previous layer output), but also its previous state.

It is important to notice that H represents the neuron state. Therefore, when in state H_1, the neuron uses as input the parameter X_1 and H_0 (its previous state). The main problem of this model is the memory loss. The network older states are fast forgotten. In sequences where we need to remember beyond the immediate past, RNNs fail to remember.

Long Short Term Memory unit(LSTM) was typically created to overcome the limitations of a Recurrent neural network (RNN). The Typical long data sets of Time series can actually be a time-consuming process which could typically slow down the training time of RNN architecture. We could restrict the data volume but this a loss of information. And in any time-series data sets, there is a need to know the previous trends and the seasonality of data of the overall data set to make the right predictions.

