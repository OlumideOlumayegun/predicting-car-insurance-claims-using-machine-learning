# Predicting Car Insurance Claims Using Machine Learning

![image](banner_image.png)

## Project Overview

Insurance companies rely heavily on predictive analytics to estimate customer risk and forecast the likelihood of insurance claims. Accurate prediction models help insurers improve pricing strategies, reduce financial risk, and support better business decision-making.

This project develops a simple machine learning solution for predicting whether a customer will make a car insurance claim during the policy period. The primary objective is to identify the **single best feature** that predicts insurance claims while maintaining a lightweight and interpretable model suitable for organisations with limited machine learning infrastructure.

The project uses logistic regression models built with Python and evaluates the predictive accuracy of each feature independently.

---

## Objectives

The main objectives of this project are to:

* Explore and understand the insurance dataset
* Handle missing data appropriately
* Build one logistic regression model per feature
* Evaluate the predictive performance of each model
* Identify the feature with the highest prediction accuracy
* Store the best-performing feature and its accuracy in a pandas DataFrame

---

## Dataset Description

The dataset (`car_insurance.csv`) contains customer demographic, financial, behavioural, and vehicle-related information.

### Features Included

| Column                | Description                               |
| --------------------- | ----------------------------------------- |
| `id`                  | Unique customer identifier                |
| `age`                 | Age category                              |
| `gender`              | Gender                                    |
| `driving_experience`  | Years of driving experience               |
| `education`           | Education level                           |
| `income`              | Income category                           |
| `credit_score`        | Credit score                              |
| `vehicle_ownership`   | Vehicle ownership status                  |
| `vehicle_year`        | Vehicle registration year                 |
| `married`             | Marital status                            |
| `children`            | Number of children                        |
| `postal_code`         | Postal code                               |
| `annual_mileage`      | Annual mileage                            |
| `vehicle_type`        | Vehicle type                              |
| `speeding_violations` | Number of speeding violations             |
| `duis`                | Number of DUI offences                    |
| `past_accidents`      | Number of previous accidents              |
| `outcome`             | Insurance claim outcome (target variable) |

### Target Variable

| Value | Meaning       |
| ----- | ------------- |
| 0     | No claim made |
| 1     | Claim made    |

---

## Technologies Used

* Python
* pandas
* NumPy
* statsmodels
* Jupyter Notebook

---

## Project Workflow

The project was completed in the following stages:

### Task 1 — Reading and Exploring the Dataset

* Load the dataset using pandas
* Inspect data types
* Check missing values
* Explore feature distributions

### Task 2 — Filling Missing Values

* Identify columns with missing values
* Replace missing values using the column mean

### Task 3 — Preparing for Modelling

* Create feature and target variables
* Create storage structures for models and results

### Task 4 — Building and Storing the Models

* Build one logistic regression model per feature
* Store each model in a list

### Task 5 — Measuring Performance

* Generate confusion matrices
* Calculate classification accuracy for each model

### Task 6 — Finding the Best Performing Model

* Identify the feature with the highest accuracy
* Store the result in `best_feature_df`

---

## Example Result

The analysis identified:

* **Best Feature:** `driving_experience`
* **Best Accuracy:** ~77.7%

This indicates that driving experience is the strongest single predictor of whether a customer is likely to make an insurance claim.

---

## Project Structure

```text
├── car_insurance.csv
├── Predicting_Car_Insurance.ipynb
├── README.md
├── requirements.txt
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/OlumideOlumayegun/predicting-car-insurance-claims-using-machine-learning.git
```

Navigate into the project directory:

```bash
cd predicting-car-insurance-claims-using-machine-learning
```

Install required libraries:

```bash
pip install -r requirements.txt
```

---

## Running the Project

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
Predicting_Car_Insurance.ipynb
```

Run all notebook cells sequentially.

---

## Key Learning Outcomes

This project demonstrates:

* Data exploration using pandas
* Missing value handling
* Logistic regression modelling
* Model evaluation using confusion matrices
* Feature selection using accuracy metrics
* Building simple and interpretable machine learning workflows

---

## Future Improvements

Potential future enhancements include:

* Using train/test split validation
* Applying cross-validation techniques
* Evaluating additional metrics such as precision, recall, and F1-score
* Building multivariable models
* Comparing multiple machine learning algorithms
* Deploying the model as a web application or API

---

## Author

**Olumide Olumayegun (PhD)**

Process Engineer | Data Scientist | AI & Machine Learning Enthusiast

---
