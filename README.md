<br />
<div align="center">
  <a href="https://github.com/omar-ammar0/Intern_Final_Project">
    <img src="Sitech.png" alt="logo">
  </a>

<h3 align="center">Pepper Pirate Paradise Price Prediction</h3>
  <p align="center">
    <a href="https://github.com/omar-ammar0/Intern_Final_Project"><strong>Explore the docs »</strong></a>
    <br />

  </p>
</div>


<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#About-The-Project">About The Project</a></li>
    <li><a href="#Built-With">Built With</a></li>
    <li><a href="#Getting-Started">Getting Started</a></li>
    <li><a href="#data-cleaning">Data Cleaning</a></li>
    <li><a href="#Feature-Engineering">Feature Engineering</a></li>
    <li><a href="#Feature-Selection">Feature Selection</a></li>
    <li><a href="#Modelling">Modelling</a></li>
    <li><a href="#Summary">Summary</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

The primary objective of this project is to predict and forecast the selling prices for a company named Pepper Pirate Paradise Ltd. of Bell Peppers of different colors (green, red, yellow) utilizing a wealth of supply and demand data. The model developed will enable producers, suppliers, and retailers to better understand price fluctuations and dynamics, facilitating more informed decision-making. Moreover, the deep analysis conducted on the data will unveil underlying patterns and contributing factors to the observed price trends for each color of Bell Pepper




### Built With
* [![Python][Python.py]][Python-url]
* 
### Libraries Used
* [![Pandas][Pandas]][Pandas-url]
* [![Numpy][Numpy]][Numpy-url]
* [![Seaborn][Seaborn]][Seaborn-url]
* [![Xgboost][Xgboost]][Xgboost-url]
* [![Plotly][Plotly]][Plotly-url]
* [![Hyperopt][Hyperopt]][Hyperopt-url]
* [![Datetime][Datetime]][Datetime-url]
* [![Scikit][Scikit]][Scikit-url]
* [![Matplotlib][Matplotlib]][Matplotlib-url]
* [![Catboost][Catboost]][Catboost-url]



## Getting Started
This project needs python installation


### Prerequisites

* Install python3 on your local machine using the below command:
    ```sh
    brew install python
    ```
* Download the dataset:

[![dataset][dataset]][dataset-link]


* Context

  * This dataset contains 1272 raw x 19 columns


* This dataset consists of the following features:
  * p_color: the different colors of the Bell Pepper.
  * price: the selling price of the Bell Pepper.
  * vietnam: supply of vietnam.
  * vietnam_season: if Vietnam is in the harvesting season or not.



## Data Cleaning
Various Data Cleaning steps were done, such as filling nulls, removing duplicates, fixing data inconsistencies.

## Feature Engineering
* New features were created for each country (Brazil, India, Vietnam, Indonesia, and China) to represent the percentage volume of peppers from that country out of the total volume of peppers.


* New features were created for each country to represent the total price of peppers from that country.


* The original dataset was divided into three separate datasets, each representing one color of pepper (red, green, and yellow).


* Visualizations were created to provide insights into the newly created features.


* New features were created by shifting and taking the rolling mean of existing features.




## Feature Selection
* The lowest 100 important features, as identified by SelectKBest, were dropped from (**df_red**, **df_green**, and **df_yellow**)  to reduce computation time and resource consumption.

## Modelling
* We implemented a data scaling function **data_scale** that applies standard scaling to the features of three different datasets (**df_red**, **df_green**, and **df_yellow**),
excluding the target variable **price**. After scaling the data,
We  carried out a quick comparison between multiple models with default parameters on the three datasets, 
analyzing their performance and accuracy by considering the mean absolute error. 
Lastly, We performed hyperparameter tuning on the XGBRegressor model to optimize its performance.


  
## Summary
* This project provides a clear and effective pipeline for analyzing Pepper Pirate paradise prices, We've cleaned and enriched our data, then used it to train machine learning models, ensuring they're finely tuned for accurate predictions. By integrating data, we're set for in-depth time series forecasting. Overall, our rigorous approach paves the way for insightful findings and reliable predictions about the world's pepper markets.


[Python.py]: https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54
[Python-url]: https://www.python.org

[Pandas-url]: https://pandas.pydata.org/
[Pandas]: https://img.shields.io/badge/Pandas-pd?style=for-the-badge&logo=pandas&logoColor=darkblue&labelColor=white&color=white

[Numpy-url]: https://numpy.org
[Numpy]: https://img.shields.io/badge/Numpy-pd?style=for-the-badge&logo=numpy&logoColor=lightblue&labelColor=white&color=white

[Seaborn-url]: https://seaborn.pydata.org
[Seaborn]: https://img.shields.io/badge/Seaborn-pd?style=for-the-badge&logo=seaborn&logoColor=blue&labelColor=white&color=white

[Plotly-url]: https://plotly.com
[Plotly]: https://img.shields.io/badge/Plotly-pd?style=for-the-badge&logo=plotly&logoColor=white&labelColor=000e39&color=000e39

[Datetime-url]: https://docs.python.org/3/library/datetime.html
[Datetime]: https://img.shields.io/badge/Datetime-pd?style=for-the-badge&logo=clock&logoColor=white&labelColor=blue&color=blue

[Matplotlib-url]: https://matplotlib.org
[Matplotlib]: https://img.shields.io/badge/matplotlib-pd?style=for-the-badge&logo=matplotlib&logoColor=white&labelColor=red&color=red

[Catboost-url]: https://catboost.ai
[Catboost]: https://img.shields.io/badge/Catboost-pd?style=for-the-badge&logo=catboost&logoColor=white&labelColor=FFCD72&color=FFCD72

[Scikit-url]: https://scikit-learn.org/stable/
[Scikit]: https://img.shields.io/badge/Scikit--learn-pd?style=for-the-badge&logo=scikit-learn&logoColor=white&labelColor=orange&color=blue

[Xgboost-url]: https://xgboost.readthedocs.io/en/stable/
[Xgboost]: https://img.shields.io/badge/xgboost-pd?style=for-the-badge&logo=xgboost&logoColor=white&labelColor=orange&color=white

[Hyperopt-url]: http://hyperopt.github.io/hyperopt/
[Hyperopt]: https://img.shields.io/badge/hyperopt-pd?style=for-the-badge&logo=hyperopt&logoColor=white&labelColor=orange&color=lightblue

[dataset-link]: https://github.com/omar-ammar0/Intern_Final_Project/tree/main/Datasets
[dataset]: https://img.shields.io/badge/DataSet-%23150458.svg?style=for-the-badge&logo=data&logoColor=white


