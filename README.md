# DATA_3402!
# USED CAR PRICE PREDICTION

# Overview
Link: https://www.kaggle.com/datasets/ayaz11/used-car-price-prediction

The dataset in question, meticulously collected via the process of web scraping from the widely recognized U.S. platform dedicated to pre-owned automobiles, Truecars.com, embodies a comprehensive arrangement of information encapsulated within six distinct columns. These columns, upon thorough analysis and manipulation, possess the potential to be transformed and expanded into an array of additional features through the process known as feature engineering. This dataset stands out as exceptionally conducive for the construction and refinement of regression models, owing to its rich and diverse content, which offers ample opportunities for exploring correlations, patterns, and predictive insights within the realm of automotive market dynamics.

The machine learning algorithm that I used  for this dataset is GRADIENT BOOST model.

<img width="730" alt="Screenshot 2024-05-03 at 11 37 47 AM" src="https://github.com/sashisoni01/DATA_3402/assets/143819869/2341afcc-70f5-4a54-b705-aa724bc124b6">

## Summary of Workdone

### Data
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

### Training

* Description the training:
  * Training was done through sklearn and Jupyter Notebook on a laptop.
  * Training each model individually took only a few seconds. 
  * The greatest challenge was handling the categorical features of interest.
  * I used Label Encoding to deal with Brand, Model, Exterior_Color and Interior_Color to make more good for model performance.

 ### Performance Comparison
 
  * Models:
    * LinearRegression: 53.9%
    * SVR: 49.9%
    * DecisionTreeRegressor: 51.7%
    * XGBRegressor: 72.9%
    * RandomForestRegressor: 70.2%
    * GradientBoostingRegressor: 80.3%
<img width="728" alt="Screenshot 2024-05-03 at 11 39 07 AM" src="https://github.com/sashisoni01/DATA_3402/assets/143819869/73b12d3f-5a6e-45a1-bf49-b1e7f0ac5add">

### Conclusions
* I used of the machine learning model to see which one can predict the best results and I found GradientBoost was the best model among all.

### Future Work

* I want to work more on the categorical variable and make it more easier to use for machine learning.
* Model Selectors and cross validation.
*  Future studies could further research the features used for the model to confirm which features tend to have the highest correlation with the price.
*  Work more on Label Encoding because it was the tough part of problem foundation.

## How to reproduce results
* To fully reproduce my results:
   * Download the dataset from Kaggle.
   * Ensure the necessary libraries are installed.
   * Download and run the Kaggle_Project notebook attached in the directory.
* Useful Resources:
  * Sklearn website; the sklearn website is a great place to find detailed explainations of the models and tools used in this project.

### Overview of files in repository

* Directory Structure: the directory contains this README.md and the code for my Kaggle project
* Relevent Files:
  * Kaggle_Project.ipynb: this notebook contains all of the code for the final submission of my Kaggle project.

### Software Setup
* Required Packages:
  * Numpy
  * Pandas
  * Sklearn
* Installation Process:
  * All packages were installed via the Linux subsystem for Windows.
  * All packages were installed via Ubuntu.
  * pip3 install numpy
  * pip3 install pandas
  * pip3 install -U scikit-learn
 
### Data

* The data can be downloaded here: [ https://www.kaggle.com/datasets/ayaz11/used-car-price-prediction]
*  Click "Download All" at the bottom of the page.

### Training

* These models can be trained by running the Kaggle_Project notebook in the repository.
* You can also refer to the official sklearn website to find the required parameters for each model.
* Sklearn website: [scikit-learn.org](https://scikit-learn.org/stable/)

#### Performance Evaluation

* The performace evaluation can be done by running the Kaggle_Project notebook in the repository.
* The training section for each model is immediately followed by performance evaluation.

  





