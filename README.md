# Project Description

This project aims to select the most profitable region for drilling new oil wells among three possible regions. It involves analyzing the quality and volume of oil reserves in these regions, building machine learning models, and assessing the risks and potential profits associated with each region.

## Project Goal

The primary goal of this project is to identify the region with the highest potential profit for oil extraction, taking into account the budget constraints and risk factors. We will achieve this by training and evaluating machine learning models on historical data from three oil-rich regions.

## Tools and Libraries

The following tools and libraries were used for this project:

- Python
- Pandas
- Matplotlib
- Scikit-Learn
- NumPy

## Project Steps

### Step 1: Loading and Preparing Data

#### 1.1 Importing the necessary libraries and modules
In this step, we import the required Python libraries and modules for data analysis and modeling.

#### 1.2 Let's open files
We load data from three different regions into dataframes.

#### 1.3 View basic information about files
We perform exploratory data analysis (EDA) to understand the structure and characteristics of the datasets, including data types, missing values, and basic statistics.

### Step 2: Training and Checking Models

In this step, we train machine learning models for each region and evaluate their performance.

#### 2.1 Let's write a function that will:

##### 2.1.1 split the data into training and validation samples in the ratio of 75:25
We split the data into training and validation sets.

##### 2.1.2 train the model and make predictions on the validation set
We train a linear regression model and use it to make predictions on the validation set.

##### 2.1.3 store predictions and correct answers on the validation set
We store the model's predictions and the correct answers (target values) on the validation set.

##### 2.1.4 print on the screen the average stock of predicted raw materials and the RMSE of the model
We calculate and display the average predicted stock of raw materials and the root mean squared error (RMSE) of the model.

#### 2.2 Conclusion
We summarize the results and observations from training and evaluating the models for each region.

### Step 3: Preparation for Profit Calculation

In this step, we prepare for calculating the potential profit from drilling wells.

#### 3.1 All key values for calculations will be saved in separate variables.
We define key constants and variables needed for profit calculations, including the budget, income per unit of product, probability of loss, and number of drilling points.

#### 3.2 Let's calculate a sufficient volume of raw materials for break-even development of a new well. Let's compare the received volume of raw materials with the average stock in each region.
We calculate the minimum volume of raw materials required for a well to break even and compare it to the average stock of raw materials in each region.

#### 3.3 Write conclusions on the stage of preparing the profit calculation.
We provide conclusions and insights based on the calculations and comparisons made in this step.

### Step 4: Calculate Profit for Selected Wells and Model Predictions

In this step, we calculate the potential profit by selecting wells with the highest predicted values.

#### 4.1 Let's select wells with maximum prediction values.
We identify the wells with the highest predicted values.

#### 4.2 Sum up the target volume of raw materials corresponding to these predictions.
We calculate the total volume of raw materials corresponding to the selected wells.

#### 4.3 Calculate the profit for the received volume of raw materials.
We calculate the potential profit based on the total volume of raw materials and the income per unit of product.

### Step 5: Calculate Risks and Rewards for Each Region

In this step, we assess the risks and rewards associated with each region.

#### 5.1 Let's use the Bootstrap technique with 1000 samples to find the profit distribution.
We employ the Bootstrap technique to simulate profit distributions.

#### 5.1.1 Write a function
We write a function to perform the Bootstrap sampling and calculate profits.

#### 5.2 Let's find the average profit, 95% confidence interval, and risk of loss. Loss is negative profit.
We calculate key statistics, including the average profit, 95% confidence interval, and the risk of loss for each region.

#### 5.3 Write your conclusions: suggest a region for well development and justify your choice.
Based on the calculated risks and rewards, we make a recommendation for the region with the highest potential profit and provide justification for our choice.

## Data Description

The project involves three regions, each with data on oil reserves:

- Region 0
- Region 1
- Region 2

Each dataset contains the following columns:

- id: Unique well identifier
- f0, f1, f2: Features of the well (numerical values)
- product: Volume of reserves in the well (thousand barrels)

Conditions and constraints:

- A drilling budget of $100 million
- Income from one unit of product: $4.5 million
- The company risks no more than 2.5% of the budget on one well
- 500 wells will be selected for development

## Usage

To run this project and reproduce the results, follow these steps:

1. Clone the repository to your local machine.
2. Install the required libraries and dependencies (Python, Pandas, Matplotlib, Scikit-Learn).
3. Open the Jupyter Notebook or Python script provided.
4. Follow the code and comments in the notebook/script to execute each step of the project.
5. Review the results, conclusions, and recommendations provided in the notebook/script.
