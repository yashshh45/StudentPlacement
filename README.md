# Student Placement Prediction Model

This repository contains code for building and deploying a Student Placement Prediction Model. The model is designed to predict the placement status of students based on provided training and testing datasets.

## Problem Statement

The problem statement for this project is to predict the Placement Status of students based on the training and testing datasets provided.

## Data Preparation

### Training Data
- The training data is loaded from an Excel file (`01 Train Data.xlsx`) and processed to remove duplicate records based on the 'Email ID' column.
- Irrelevant columns are removed from the dataset to clean it for modeling.
- The 'Placement Status' column is mapped to binary values ('Placed' as 1 and 'Not placed' as 0) and any missing values are filled with 2 (indicating unknown status).
- Some specific values in the 'Year of Graduation' column are removed, and custom mappings are applied to standardize values.
- The 'Year of Graduation' column is converted to integers.

### Testing Data
- The testing data is loaded from an Excel file (`02 Test Data.xlsx`) and processed in a similar manner as the training data.

## Model Building and Evaluation

- The training dataset is split into training and testing sets using a 80/20 split ratio.
- A Random Forest Classifier is used as an example machine learning model for prediction.
- The model is trained on the training data, and predictions are made on the testing data.
- The accuracy of the model is calculated and printed.

## Prediction on Test Data

- The trained model is used to make predictions on the testing data.
- The unique predicted values are printed.
- The counts of each predicted value are printed.

## Saving Results

- The testing data with placement predictions is saved to an Excel file (`test_data_with_predictions.xlsx`) for further analysis.

## How to Use

1. Clone this repository.
2. Place your training data in an Excel file named `01 Train Data.xlsx` with the same structure as the provided dataset.
3. Place your testing data in an Excel file named `02 Test Data.xlsx` with the same structure as the provided dataset.
4. Run the provided code to train the model and make predictions.
5. Retrieve the results from the `test_data_with_predictions.xlsx` file.

Feel free to replace the model with other machine learning algorithms for experimentation and improvement.

## Dependencies

Make sure you have the following Python libraries installed:

- pandas
- numpy
- scikit-learn

You can install them using pip:

```bash
pip install pandas numpy scikit-learn
```

## Author

Yash Gandhi
