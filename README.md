# New York Taxi Dataset Analysis:
- This repo is attempting to use New York Taxi Dataset from Google's Big Query to derive some insights.
- All notebooks are using Anaconda Python2

## Summary Report of findings: [Summary_Report.pdf](https://github.com/stephenleo87/nyc-taxi/blob/master/Summary_Report.pdf)

## Instructions:
1. git clone https://github.com/stephenleo87/nyc-taxi.git
2. pip install -r requirements.txt

## Details:
There are 4 Jupyter Notebooks in this repo

1. [01_SQL Query.ipynb](https://github.com/stephenleo87/nyc-taxi/blob/master/01_SQL%20Query.ipynb)
	- All SQL queries are run from Google Cloud's Datalab platform and the data is stored as csv files for use by subsequent notebooks
	- This notebook is included for reference purposes only
	
2. [02_Fare Prediction.ipynb](https://github.com/stephenleo87/nyc-taxi/blob/master/02_Fare%20Prediction.ipynb)
	- Attempting to predict the fare amount from the available data such as trip distance, pickup locations, etc
	- TL;DR: Best prediction model achieved RMSE of $3.5
	
3. [03_Tip Prediction.ipynb](https://github.com/stephenleo87/nyc-taxi/blob/master/03_Tip%20Prediction.ipynb)
	- Attempting to predict the tip percentage (tip_amount/fare_amount) from the available data such as trip distance, pickup locations, etc
	- TL;DR: Best prediction model could only achieve accuracy of 60% indicating the available dataset is not sufficient to accurately predict tip percentage

4. [04_Destination Prediction.ipynb](https://github.com/stephenleo87/nyc-taxi/blob/master/04_Destination%20Prediction.ipynb)
	- Attempting to predict the destination location from the available data such as pickup time, pickup location
	- TL;DR: No good prediction model could be found indicating the available dataset is not sufficient to predict dropoff location
