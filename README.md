# Predicting Bike-Sharing Patterns

![Bikes](https://user-images.githubusercontent.com/68460588/178815585-a0423037-ec0e-49cb-a5e0-35539d152c5a.png)

--- 

## Overview
This project was made by me during Udacity Deep Learning Nanodegree at Udacity. I build a Neural Network from scratch using NumPy and train for regression problem.
The problem is to predict of bike rental count hourly or daily based on the environmental and seasonal settings, to prepare enough amount of bike for rider in the future.

---

## Dataset
I trained the NN on Bike-Sharing dataset. This dataset has the number of riders for each hour of each day from January 1 2011 to December 31 2012.
The number of riders is split between casual and registered, summed up in the cnt column. 
Bike-sharing rental process is highly correlated to the environmental and seasonal settings. 
For instance, weather conditions, precipitation, day of week, season, hour of the day, etc. can affect the rental behaviors. 
The core data set is related to the two-year historical log corresponding to years 2011 and 2012 from Capital Bikeshare system.<br>

Files:<br>
- hour.csv : bike sharing counts aggregated on hourly basis. Records: 17379 hours
- day.csv - bike sharing counts aggregated on daily basis. Records: 731 days<br>

Features and Target variable:<br><br>
Both hour.csv and day.csv have the following fields, except hr which is not available in day.csv
	
	- instant: record index
	- dteday : date
	- season : season (1:springer, 2:summer, 3:fall, 4:winter)
	- yr : year (0: 2011, 1:2012)
	- mnth : month ( 1 to 12)
	- hr : hour (0 to 23)
	- holiday : weather day is holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
	- weekday : day of the week
	- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
	+ weathersit : 
		- 1: Clear, Few clouds, Partly cloudy, Partly cloudy
		- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
		- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
		- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
	- temp : Normalized temperature in Celsius. The values are divided to 41 (max)
	- atemp: Normalized feeling temperature in Celsius. The values are divided to 50 (max)
	- hum: Normalized humidity. The values are divided to 100 (max)
	- windspeed: Normalized wind speed. The values are divided to 67 (max)
	- casual: count of casual users
	- registered: count of registered users
	- cnt: count of total rental bikes including both casual and registered

---

## Requirements	
- Python 3.7
- Numpy 
- Pandas 
- Matplotlib 
- Jupyter Notebook

---

## Running the project
The whole project is located in the jupyter notebook file ```Your_first_neural_network.ipynb```
and it's include the training and the prediction part. The neural network is implemented in the file 
```my_answer.py``` and used from the jupyter notebook.

--- 


## Hyperparameters of training
To change the number of epochs, the amount of hidden notes and some other parameters for the neural network, 
you can adapt these global variable at the end of the python file ```my_answer.py```.

