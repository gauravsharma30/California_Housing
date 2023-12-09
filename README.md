# California Housing Price Prediction 🏠

This Python project aims to analyze California housing data and predict housing prices using linear regression as the machine learning technique. The project utilizes the popular scikit-learn library for implementing linear regression and handling the machine learning aspects of the analysis.


## Implementation Details

- Dataset: California Housing Dataset (view below for more details)
- Model: [Linear Regressor](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html)
- Input: 8 features - Median Houshold income, House Area, ...
- Output: House Price

## Dataset Details

This dataset was obtained from the StatLib repository ([Link](https://www.dcc.fc.up.pt/~ltorgo/Regression/cal_housing.html))

This dataset was derived from the 1990 U.S. census, using one row per census block group. A block group is the smallest geographical unit for which the U.S. Census Bureau publishes sample data (a block group typically has a population of 600 to 3,000 people).

A household is a group of people residing within a home. Since the average number of rooms and bedrooms in this dataset are provided per household, these columns may take surprisingly large values for block groups with few households and many empty houses, such as vacation resorts.

It can be downloaded/loaded using the sklearn.datasets.fetch_california_housing function.

- [California Housing Dataset in Sklearn Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_california_housing.html)
- 20640 samples
- 8 Input Features: 
    - MedInc median income in block group
    - HouseAge median house age in block group
    - AveRooms average number of rooms per household
    - AveBedrms average number of bedrooms per household
    - Population block group population
    - AveOccup average number of household members
    - Latitude block group latitude
    - Longitude block group longitude
- Target: Median house value for California districts, expressed in hundreds of thousands of dollars ($100,000)


## Evaluation and Results
![alt text](https://github.com/123ofai/Demo-Project-Repo/blob/main/results/test.png)

As you can see from the above image, the model has signifcant amount of error in <x, y, z regions>

| Metric        | Value         |
| ------------- | ------------- |
| R2 Score      | 0.59          |
| MSE           | 0.53          | 


## How to Run

The code is built on Google Colab on an iPython Notebook. 

```bash
Simply download the repository, upload the notebook and dataset on colab, and hit play!
```


## Roadmap

What are the future modification you plan on making to this project?

- Try more models

- Try to do feature selection

- Wrapped Based Feature Selection


## Libraries 

**Language:** Python

**Packages:** Sklearn, Matplotlib, Pandas, Seaborn


## FAQ

#### How does the linear regression model work?

Linear Regression relationship between the independent variable X and the dependent variable (response) y is assumed to be linear. The linear relationship is represented by the equation: y=mx+b, where m is the slope (coefficient) and b is the intercept.

Linear relationship is extended to multiple Features (X1, X2, X3... Xn) y = b0+ b1X1+b2X2+...+bnXn. where b0 is intercept , b1,b2,b3...bn are the coefficient of Features X1, X2, X3, X4 .. Xn

The objective is to find the values of b0,b1,b2,b3...bn, hat minimize the difference between the predicted y and the actual y for each data point.



## License

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)

