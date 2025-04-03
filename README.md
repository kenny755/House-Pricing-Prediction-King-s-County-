# House Price Prediction

This repository contains the data and code used for a project that aims to predict house prices using machine learning models. By analyzing features such as square footage, number of bedrooms, and location, we explore the factors that influence real estate values.

## Table of Contents

1.  [Project Overview](#project-overview)
2.  [Repository Contents](#repository-contents)
3.  [Data Description](#data-description)
4.  [Project Implementation](#project-implementation)
    * [4.1. Data Loading and Exploration](#41-data-loading-and-exploration)
    * [4.2. Data Wrangling](#42-data-wrangling)
    * [4.3. Pipeline and Model Building](#43-pipeline-and-model-building)
        * [4.3.1. Linear Regression](#431-linear-regression)
        * [4.3.2. Ridge Regression](#432-ridge-regression)
        * [4.3.3. Polynomial Regression (Degree 2)](#433-polynomial-regression-degree-2)
    * [4.4. Model Evaluation](#44-model-evaluation)
    * [4.5. Visualization](#45-visualization)
5.  [Usage](#usage)
6.  [Contributing](#contributing)
7.  [License](#license)

## Project Overview

This project focuses on building predictive models to estimate house prices. The goal is to understand the relationships between various property features and their corresponding prices, enabling us to identify key drivers of real estate value. We implement and compare linear regression, ridge regression, and polynomial regression (degree 2) using a pipeline to streamline the process.

## Repository Contents

* **`House_Sales_King_County_USA.csv`:** The dataset containing house sales information from King County, USA.
* **`IBM project.ipynb`:** A Jupyter Notebook containing the data analysis and model building code.

## Data Description

The `House_Sales_King_County_USA.csv` dataset includes the following features:

* **`id`:** Unique identifier for each house.
* **`date`:** Date of the house sale.
* **`price`:** Price of the house.
* **`bedrooms`:** Number of bedrooms.
* **`bathrooms`:** Number of bathrooms.
* **`sqft_living`:** Square footage of the living space.
* **`sqft_lot`:** Square footage of the lot.
* **`floors`:** Number of floors.
* **`waterfront`:** Whether the house has a waterfront view (0 or 1).
* **`view`:** An index from 0 to 4 of how good the view of the property was.
* **`condition`:** An index from 1 to 5 of the condition of the house.
* **`grade`:** An index from 1 to 13, where 1-3 falls short of building construction and design, 7 has an average level of construction and design, and 11-13 have a high level of construction and design.
* **`sqft_above`:** Square footage of the house apart from the basement.
* **`sqft_basement`:** Square footage of the basement.
* **`yr_built`:** Year the house was built.
* **`yr_renovated`:** Year the house was renovated.
* **`zipcode`:** Zip code of the location.
* **`lat`:** Latitude coordinate.
* **`long`:** Longitude coordinate.
* **`sqft_living15`:** Square footage of the living space in 2015 (implies some renovations).
* **`sqft_lot15`:** Square footage of the lot in 2015 (implies some renovations).

## Project Implementation

The project is implemented in the `IBM project.ipynb` Jupyter Notebook. The notebook includes the following stages:

### 4.1. Data Loading and Exploration

* Loading the dataset using pandas.
* Performing initial exploratory data analysis (EDA) to understand the data's structure and characteristics.
* Visualizing key features using histograms, scatter plots, and box plots.

### 4.2. Data Wrangling

* Handling missing values (imputation or removal).
* Converting data types as needed.
* Removing or transforming outliers.
* Feature engineering: Creating new features or transforming existing ones.

### 4.3. Pipeline and Model Building

* Creating a pipeline to streamline the preprocessing and modeling steps.
* Implementing and comparing the following models:

    #### 4.3.1. Linear Regression

    * Fitting a linear regression model to predict house prices.

    #### 4.3.2. Ridge Regression

    * Fitting a ridge regression model to address potential multicollinearity.
    * Tuning the regularization parameter (alpha) using cross-validation.

    #### 4.3.3. Polynomial Regression (Degree 2)

    * Creating polynomial features (degree 2) to capture non-linear relationships.
    * Fitting a linear regression model on the polynomial features.

### 4.4. Model Evaluation

* Evaluating the performance of each model using metrics such as $R^2$ score and mean squared error (MSE).
* Comparing the models to determine the best-performing one.

### 4.5. Visualization

* Creating visualizations to understand the relationships between features and prices.
* Visualizing model predictions against actual prices.

## Usage

To run the project:

1.  Clone this repository to your local machine.
2.  Ensure you have Jupyter Notebook and the necessary Python libraries installed (pandas, scikit-learn, seaborn, matplotlib).
3.  Open the `IBM project.ipynb` file using Jupyter Notebook.
4.  Run the cells in the notebook sequentially to execute the code.

## Contributing

Contributions to this project are welcome. If you find any issues or have suggestions for improvement, please feel free to submit a pull request or open an issue.

## License

