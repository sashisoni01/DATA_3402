# DATA_3402!
# USED CAR PRICE PREDICTION

# Overview
Link: https://www.kaggle.com/datasets/ayaz11/used-car-price-prediction

The dataset in question, meticulously collected via the process of web scraping from the widely recognized U.S. platform dedicated to pre-owned automobiles, Truecars.com, embodies a comprehensive arrangement of information encapsulated within six distinct columns. These columns, upon thorough analysis and manipulation, possess the potential to be transformed and expanded into an array of additional features through the process known as feature engineering. This dataset stands out as exceptionally conducive for the construction and refinement of regression models, owing to its rich and diverse content, which offers ample opportunities for exploring correlations, patterns, and predictive insights within the realm of automotive market dynamics.

The machine learning algorithm that I used  for this dataset is GRADIENT BOOST model.

<img width="730" alt="Screenshot 2024-05-03 at 11 37 47 AM" src="https://github.com/sashisoni01/DATA_3402/assets/143819869/2341afcc-70f5-4a54-b705-aa724bc124b6">

## Summary of Workdone

### Data
  *Data:
    *Type:
      * Input: CSV file of features; categorical and numerical data describing year, 
      miles, condition, color, name and price.
    * Output: success/failure; what affect the price of the used car.
  * Size: 2840 observations/rows; 6 features/columns
  * Instances (Train, Validation, Test; Split): 80% for training 20% for testing

#### Preprocessing / Clean up

* Filtered out unneccessary features, and created new features that gives better results.
* Features Used: Year, Miles, Brand, Model, Exterior, Interior, Num of Accident, Num of Owner, and Price.
* Only color columns contains some unknown values.
* The categorical features were encoded using OneHotEncoder() and Label Encoding. 

#### Data Visualization

<img width="725" alt="Screenshot 2024-05-03 at 11 38 33 AM" src="https://github.com/sashisoni01/DATA_3402/assets/143819869/a6227ced-cef1-4d95-90b7-1450b096e3c5">

### Problem Formulation

* Define:
  * Input: selected features mentioned above.
  * Output: 80% with GradientBoost.
  * Models:
    * LinearRegression: 53.9%
    * SVR: 48.9%
    * DecisionTreeRegressor: 47.4%
    * XGBRegressor: 68.8%
    * RandomForestRegressor: 68.2%
    * GradientBoostingRegressor: 78.6
<img width="728" alt="Screenshot 2024-05-03 at 11 39 07 AM" src="https://github.com/sashisoni01/DATA_3402/assets/143819869/73b12d3f-5a6e-45a1-bf49-b1e7f0ac5add">

